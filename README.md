# 📦 ROM Mirror Automation (Gofile → SourceForge)

This repository contains a **GitHub Actions workflow** that automatically mirrors your custom ROM builds from **Gofile to SourceForge**, while:

✅ Preserving the **original filename**  
✅ Allowing **dynamic SourceForge folders**  
✅ Requiring **no local uploads**  
✅ Working fully in GitHub Actions  

This is especially useful for ROM developers who host builds on Gofile but also want a reliable mirror on SourceForge.

---

## 🚀 Features

- 🔄 One-click upload via GitHub Actions  
- 📁 Dynamic SourceForge folder selection per build  
- 📛 Keeps the **exact same filename** from Gofile  
- 🤖 Fully automated (no manual upload needed)  
- 🧩 Works for any ROM, device, or project  

---

## 📂 How It Works (Overview)

The workflow does three simple things:

1. **Downloads** your ROM from a provided Gofile link  
2. Detects and preserves the **original filename**  
3. **Uploads** the file to your chosen SourceForge folder via SFTP  

---

## ⚙️ Setup Instructions

### **Step 1 — Add GitHub Secrets**

Go to your repository:

Add these secrets:

| Secret Name   | Value |
|---------------|-------|
| `SF_USER`     | Your SourceForge username |
| `SF_PASSWORD` | Your SourceForge password |
| `SF_PROJECT`  | Munch roms |

> 📌 **Note:**  
> You do **NOT** need to store the Gofile link or folder name as secrets.
> Now simply run the workflow.
