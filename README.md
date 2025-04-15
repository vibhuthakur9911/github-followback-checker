# GitHub Follow-Back Checker 🚀

## Introduction

This script helps you identify GitHub users you follow who aren’t following you back. By leveraging GitHub’s API, it retrieves your **followers** and **following** lists, compares them, and highlights the accounts that haven’t returned the follow. It’s a simple way to keep track of one-way connections on your GitHub network..

## Requirements

* A **GitHub Personal Access Token (PAT)**
* **Node.js** installed (for running the script locally)

## Step 1: Generate a GitHub Personal Access Token

1. Go to [GitHub Token Settings](https://github.com/settings/tokens)
2. Click on **"Generate new token"**
3. Select **"read:user"** permission
4. Copy and save the token (it will be visible only once)

## Step 2: Clone the Repository

```sh
git clone https://github.com/your-username/github-follow-checker.git
cd github-follow-checker
```

## Step 3: Install Dependencies

```sh
npm install
```

*(No additional dependencies required for this script, but `node-fetch` can be used if needed.)*

## Step 4: Update Credentials

Open `github-follow-check.js` and update the following variables:

```javascript
const GITHUB_USERNAME = "your-username"; // Replace with your GitHub username
const GITHUB_TOKEN = "your-personal-access-token"; // Replace with your GitHub token
```

## Step 5: Run the Script

```sh
node github-follow-check.js
```

## Expected Output

If some users haven't followed you back:

```
✅ These users have followed you back:
- user1
- user2
- user3

❌ These users haven't followed you back:
- user4
- user5
- user6
```

If everyone has followed you back:

```
✅ These users have followed you back:
- user1
- user2
- user3
- user4

Everyone you follow has followed you back!
```

## Alternative: Run in Browser Console

1. Open GitHub and press `F12` to open the Developer Console.
2. Copy-paste the script from `github-follow-check.js`.
3. Press `Enter` to execute.

---

>[!NOTE]
>
>In browser console Output may take some time to reflect

### 🔥 Contributing

Feel free to submit issues or PRs if you find improvements!

### 🛡️ License

This project is licensed under the MIT License.
