# BackupBuddy

Backup Buddy is a simple, single-file HTML utility designed to help developers quickly generate shell commands for backing up and restoring files. It is particularly useful when dealing with raw file lists or git status outputs, automating the tedious process of writing `mv` commands for each file.

## Live Demo

[Live Demo](https://ronaldtdas.github.io/BackupBuddy/)

## ✨ Features

- **Smart Parsing:** Automatically strips out git status prefixes (like `modified:`, `new file:`, `deleted:`, `Untracked files:`) to extract clean file paths.
- **Space Handling:** Automatically wraps file paths containing spaces in quotes to ensure valid shell commands.
- **One-Click Copy:** Easily copy the generated backup or restore commands to your clipboard with a built-in toast notification.
- **Local History:** Automatically saves your recently generated commands locally in your browser, complete with timestamps.
- **History Management:** Reload past inputs into the editor, delete individual history records, or clear all history (protected by a sleek confirmation modal).
- **Single File:** Zero dependencies to install. It's just one HTML file utilizing Tailwind CSS via CDN.

## 🚀 How to Use

1. Copy a list of files (e.g., the output from `git status`).
2. Paste the list into the input area.
3. Click **Generate Commands**.
4. Copy the `.backup` commands to back up your files before running scripts or making drastic changes.
5. Copy the **Restore** commands if you need to revert the files back to their original state.

## 🛠 Tech Stack

- HTML5
- JavaScript (Vanilla)
- Tailwind CSS (via CDN)
