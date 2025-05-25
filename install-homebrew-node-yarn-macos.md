
# 🛠 Install Homebrew, Node.js, and Yarn on macOS

This guide walks you through installing **Homebrew**, **Node.js**, and **Yarn** on **macOS** using the terminal.

---

## ✅ Prerequisites

- macOS 10.14 or later
- Command Line Tools for Xcode
- Admin access (you may be prompted for your password)

---

## 🔹 Step 1: Open Terminal

- Press `Command + Space`, type `Terminal`, and press **Enter**.

---

## 🔹 Step 2: Install Command Line Tools (if not already installed)

```bash
xcode-select --install
```

- A popup will appear. Click **Install**.
- If already installed, you may see:  
  `xcode-select: error: command line tools are already installed`

---

## 🔹 Step 3: Install Homebrew

Paste this into your Terminal:

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

---

## 🔹 Step 4: Add Homebrew to Your Shell Profile (if prompted)

For ZSH (default in macOS):

```bash
echo 'eval "$(/opt/homebrew/bin/brew shellenv)"' >> ~/.zprofile
eval "$(/opt/homebrew/bin/brew shellenv)"
```

---

## 🔹 Step 5: Verify Homebrew Installation

```bash
brew --version
```

You should see something like: `Homebrew 4.x.x`

---

## 🔹 Step 6: Install Node.js (LTS Version)

Use Homebrew to install Node.js:

```bash
brew install node
```

---

## 🔹 Step 7: Check Node and npm Versions

```bash
node -v
npm -v
```

This confirms Node.js and npm were installed correctly.

---

## 🔹 Step 8: Install Yarn (without using Node installer)

```bash
brew install yarn
```

> This method does not install Node again, which avoids duplication.

---

## 🔹 Step 9: Check Yarn Version

```bash
yarn -v
```

You should see something like: `1.x.x` or `berry (3.x.x)` depending on version.

---

## ✅ Optional Maintenance

Update Homebrew:

```bash
brew update
```

Check for problems:

```bash
brew doctor
```

You should see:  
`Your system is ready to brew.`

---
