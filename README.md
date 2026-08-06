## Instructions

1. Fork the repo.
2. Clone the repo in your account to your Ubuntu VM.
3. Inside the `students` folder create a folder with your roll number in **ALL CAPS LETTERS**.
4. Inside the folder add two files. One is an `index.html` file, which you design the way you want it. The second file must follow the given JSON format, and must contain your roll number, your name, and your GitHub photo URL like `https://github.com/<your-github-user-name>.png`.
5. Once this is done, commit the changes.
6. Push the changes to the repo in your account.
7. Create a Pull Request to the original forked repo.
8. Check that your pull request is accepted and merged.

---

## Step by Step

Each step below explains one of the instructions above in detail.

---

### Step 1: Fork This Repository

Forking creates your own personal copy of this repo on your GitHub account.

1. Make sure you are logged into [GitHub](https://github.com)
2. Go to the top-right of this repo page and click the **Fork** button
3. GitHub will create a copy at `https://github.com/YOUR-USERNAME/kiet-bootcamp`

---

### Step 2: Clone the Repo to Your Ubuntu VM

Cloning downloads your fork to your Ubuntu VM so you can edit files locally.

Open a terminal on your Ubuntu VM and run:

```bash
git clone https://github.com/YOUR-USERNAME/kiet-bootcamp.git
```

Then move into the folder:

```bash
cd kiet-bootcamp
```

---

### Step 3: Create Your Folder Inside `students`

Create a folder named with your roll number in **ALL CAPS LETTERS**:

```bash
mkdir students/21BCE1099
```

Replace `21BCE1099` with your actual roll number. It must be in capital letters — `21bce1099` is not accepted.

---

### Step 4: Add Your Two Files

Inside your folder, create two files.

**1. `index.html`** — design it however you want. It is your page, so style it your way. A very simple starting point:

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>Your Name - KIET Git Bootcamp</title>
</head>
<body>
  <img src="https://github.com/YOUR-USERNAME.png" alt="Your Name" width="120" />
  <h1>Your Full Name</h1>
  <p>Roll No: 21BCE1099</p>
</body>
</html>
```

**2. `info.json`** — this one must follow the given format exactly:

```json
{
  "roll": "21BCE1099",
  "name": "Your Full Name",
  "photo": "https://github.com/YOUR-USERNAME.png"
}
```

**Example:**

```json
{
  "roll": "21BCE1099",
  "name": "Priya Nair",
  "photo": "https://github.com/priyanair.png"
}
```

Use your GitHub profile photo URL for the `photo` field — it is always `https://github.com/<your-github-user-name>.png`.

---

### Step 5: Commit Your Changes

Check what files you changed:

```bash
git status
```

Add your new folder to Git:

```bash
git add students/21BCE1099/
```

Commit with a message describing what you did:

```bash
git commit -m "Add student: 21BCE1099 Your Name"
```

---

### Step 6: Push to Your Fork on GitHub

Upload your commit to your GitHub fork:

```bash
git push origin main
```

If Git asks for your username and password, use your GitHub username and a **Personal Access Token** (not your GitHub password). You can create one at: GitHub → Settings → Developer Settings → Personal Access Tokens.

---

### Step 7: Create a Pull Request

A Pull Request (PR) asks the maintainers of the original repo to review and merge your changes.

1. Go to your fork on GitHub: `https://github.com/YOUR-USERNAME/kiet-bootcamp`
2. You will see a yellow banner saying **"Compare & pull request"** — click it
3. Add a title like: `Add student: 21BCE1099 Your Name`
4. Click **"Create pull request"**

---

### Step 8: Check That Your PR Is Merged

Open the **Pull requests** tab on the original repo and find your PR. Once a maintainer reviews it, it will be marked as **Merged**. If a maintainer leaves comments asking for changes, make the changes locally, commit, and push again — the PR updates automatically.

---

## Folder Structure

This is what the repo looks like:

```
kiet-bootcamp/
├── README.md
└── students/
    ├── 21BCE1001/        (sample)
    │   ├── index.html
    │   └── info.json
    ├── 21BCE1042/        (sample)
    │   ├── index.html
    │   └── info.json
    └── 21BCE1099/        <-- your folder goes here (use your roll number)
        ├── index.html
        └── info.json
```

Your folder name must be exactly your roll number in ALL CAPS — nothing else.

---

## Rules

- Only add files inside your own folder. Do not touch anyone else's folder.
- Your folder name must match your actual roll number, in ALL CAPS LETTERS.
- `info.json` must be valid JSON (no missing commas or quotes) and follow the given format.
- One student per folder. Do not submit more than once.
- Keep your `index.html` clean — no harmful or inappropriate content.

---

## Need Help?

If you are stuck at any step, ask a mentor during the bootcamp session or open a GitHub Issue on this repo describing your problem.

Happy committing!
