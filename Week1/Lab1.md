# 📘 ICT Lab Notes — Introduction to Computers Course

This document contains self-explanatory notes for the **Introduction to Computers (ICT)** lab course, covering multiple weeks/lectures.

---

## 📑 Table of Contents

### 🖥️ Week 1: Introduction to Computers
1. [How to Check System (PC) Specifications](#1-how-to-check-system-pc-specifications)
2. [Introduction to Computers](#2-introduction-to-computers)
3. [Identify Computer Components](#3-identify-computer-components)
4. [Explore Storage Devices](#4-explore-storage-devices)
5. [Capacity and Speed Considerations](#5-capacity-and-speed-considerations)
6. [Steps to Install a Hard Drive](#6-steps-to-install-a-hard-drive)
7. [Quick Recap](#7-quick-recap)

### ✍️ Week 2: Overleaf (LaTeX) & GitHub Version Control
8. [Introduction to Overleaf & LaTeX](#8-introduction-to-overleaf--latex)
9. [Basic LaTeX Document Structure](#9-basic-latex-document-structure)
10. [Introduction to Version Control & Git](#10-introduction-to-version-control--git)
11. [GitHub Basics](#11-github-basics)
12. [Essential Git Commands](#12-essential-git-commands)
13. [Typical Git Workflow](#13-typical-git-workflow)
14. [Week 2 Quick Recap](#14-week-2-quick-recap)

### 📝 Week 3: Word Processing Tools – Basics (MS Word / Google Docs)
15. [Introduction to Word Processing Tools](#15-introduction-to-word-processing-tools)
16. [Creating Business Documents](#16-creating-business-documents)
17. [Formatting Tools](#17-formatting-tools)
18. [Page Setup, Header/Footer](#18-page-setup-headerfooter)
19. [Working with Tables](#19-working-with-tables)
20. [Working with Images](#20-working-with-images)
21. [Week 3 Quick Recap](#21-week-3-quick-recap)

---

# 🖥️ Week 1: Introduction to Computers

Welcome to the first lab of **Introduction to Computers (ICT)**. This lecture covers the basics of what a computer is, its core components, storage devices, and how to check your system's specifications.

---

## 1. How to Check System (PC) Specifications

Before working with any computer, it's important to know **what hardware you have**. Windows gives you two easy built-in tools for this: **Task Manager** and **DXDIAG**.

### 🔧 Method 1: Task Manager

Open Task Manager (`Ctrl + Shift + Esc`) and go to the **Performance** tab. Each section on the left shows live stats for a different component:

| Component | What You'll See | Why It Matters |
|---|---|---|
| **CPU** | Model name, utilization %, cores, threads, cache size | Tells you how powerful and fast your processor is |
| **Memory (RAM)** | Total size, speed (MHz), slots used | More RAM = smoother multitasking |
| **Disk (SSD/HDD)** | Model, capacity, read/write speed | SSDs are much faster than HDDs |
| **Ethernet/WiFi** | Adapter name, IP address, signal strength | Shows your network connection details |
| **GPU** | Model, driver version, dedicated/shared memory | Important for gaming, video editing, and graphics tasks |

> 💡 **Tip:** You can also check running apps and background processes under the **Processes** tab — useful for spotting what's slowing your PC down.

### 🔧 Method 2: DXDIAG (DirectX Diagnostic Tool)

1. Press `Windows + R`, type `dxdiag`, and hit Enter.
2. The **System** tab shows: OS version, manufacturer, model, processor, and installed RAM.
3. The **Display** tab shows your graphics card details and driver info.
4. The **Sound** and **Input** tabs show audio devices and connected input hardware (mouse, keyboard, etc.)

> ✅ **Why this matters:** Knowing your specs helps you decide if your PC can run certain software/games, and helps with troubleshooting.

---

## 2. Introduction to Computers

### What is a Computer?
A **computer** is an electronic device that follows programmed instructions to perform tasks. Its main job is to **turn raw data into useful information**, and it can do this millions of times per second.

### The Four Basic Operations

Every computer works using this simple cycle:

```
INPUT  →  PROCESSING  →  OUTPUT  →  STORAGE
```

| Stage | Description | Examples |
|---|---|---|
| **Input** | Data enters the system from the user | Keyboard, mouse, scanner, microphone |
| **Processing** | The CPU follows instructions to calculate/decide | Central Processing Unit (CPU) |
| **Output** | Processed data is shown to the user | Monitor, printer, speaker, headphones |
| **Storage** | Data is saved for later use | Hard drive, SSD, USB drive |

### Types of Computers

| Type | Description |
|---|---|
| **Personal Computers (PCs)** | Desktops & laptops used for everyday personal tasks |
| **Servers** | Powerful machines that manage websites, databases, and network resources |
| **Mobile Devices** | Smartphones & tablets — portable and optimized for mobility |
| **Embedded Systems** | Small computers built into cars, appliances, and medical devices for specific tasks |

---

## 3. Identify Computer Components

If you open up a desktop PC, here are the main parts you'll find:

### 🧠 CPU (Central Processing Unit)
- Known as the **"brain"** of the computer.
- Executes instructions and performs calculations.
- Has multiple **cores** to handle several tasks at once.
- Popular brands: **Intel, AMD Ryzen**.

### 🧩 RAM (Random Access Memory)
- **Temporary** storage for data currently in use.
- More RAM = better multitasking.
- **Volatile** — all data is erased when the power turns off.
- Comes in generations: DDR, DDR2, DDR3, DDR4, DDR5 (each newer version is faster).

### 🖥️ Motherboard
- The **main circuit board** that connects everything together.
- Hosts the CPU, RAM, and expansion slots (like for a GPU).
- Manages communication between all components.

### ⚡ Power Supply Unit (PSU)
- Converts wall electricity into usable power for the PC.
- Delivers different voltages to different parts.
- Rated in **watts** — higher wattage supports more powerful systems.

### 🎮 GPU (Graphics Processing Unit)
- Handles rendering of images, videos, and graphics.
- Essential for gaming, video editing, and design (CAD) work.
- Can be **integrated** (built into the CPU/motherboard) or **dedicated** (a separate card).

### ❄️ Cooling System (Fans & Heatsinks)
- Prevents the CPU/GPU from overheating.
- Fans push hot air out and pull cool air in.
- Heatsinks absorb and spread out heat.

---

## 4. Explore Storage Devices

### HDD vs SSD

| Feature | HDD (Hard Disk Drive) | SSD (Solid State Drive) |
|---|---|---|
| Technology | Spinning magnetic disks | Flash memory chips (no moving parts) |
| Speed | Slower | Much faster |
| Price | Cheaper per GB | More expensive per GB |
| Durability | More prone to damage from drops | More shock-resistant |
| Best for | Bulk storage (large files, backups) | OS installation, faster boot & load times |

### Other Storage Types
- **USB Flash Drive:** Small, portable, used for quick file transfers and backups.
- **Optical Drive (CD/DVD/Blu-ray):** Reads/writes discs — becoming rare due to cloud storage and downloads.

### Internal vs External Storage

| Type | Description |
|---|---|
| **Internal Storage** | Built into the PC (main HDD/SSD) — stores the OS, programs, and files |
| **External Storage** | Connected via USB/Thunderbolt — used for backups or transferring large files |

---

## 5. Capacity and Speed Considerations

- **Capacity** is measured in **Gigabytes (GB)** or **Terabytes (TB)**. Higher capacity = more room for files, apps, and games.
- **Speed** is measured in **MB/s** or **GB/s**. SSDs are significantly faster than HDDs, which means:
  - Faster boot times
  - Quicker file access
  - Snappier overall performance

> 📌 **Rule of thumb:** Choose SSD for speed (OS + frequently used apps), HDD for cheap bulk storage.

---

## 6. Steps to Install a Hard Drive

Follow these steps carefully when installing a new HDD or SSD:

1. **Shut down and unplug the PC** — avoids electrical damage or short circuits.
2. **Open the case** — use a screwdriver to remove the side panel.
3. **Locate an available drive bay** — find a free slot for the new drive.
4. **Connect the SATA cable and power connector** — SATA transfers data to the motherboard; the power cable comes from the PSU.
5. **Secure the drive** — use screws or clips so it doesn't move during use.
6. **Close the case and power on** — plug the PC back in and boot it up.
7. **Verify installation** — check that the drive appears under **Storage Management** in the OS.

---

## 7. Quick Recap

✅ A computer works in a cycle: **Input → Processing → Output → Storage**
✅ Core components: **CPU, RAM, Motherboard, PSU, GPU, Cooling System**
✅ **SSD = faster & pricier**, **HDD = slower & cheaper, more capacity**
✅ Use **Task Manager** or **DXDIAG** to check your PC's specs
✅ Installing a drive is a simple 6-step hardware process

---

### 📚 Recommended Next Step
Try opening Task Manager and DXDIAG on your own PC, and identify each component listed above to reinforce what you've learned!

---
---

# ✍️ Week 2: Overleaf Introduction & GitHub Version Control Basics

This lecture introduces two essential tools for technical/academic work: **Overleaf** (for writing professional documents using LaTeX) and **Git/GitHub** (for tracking and managing changes to your projects).

---

## 8. Introduction to Overleaf & LaTeX

### What is LaTeX?
**LaTeX** (pronounced "Lay-tech") is a document preparation system used to create professional, well-formatted documents — especially ones with lots of **math equations, references, and structured formatting** (like research papers, theses, and reports).

Unlike Microsoft Word (a **WYSIWYG** editor — "What You See Is What You Get"), LaTeX works differently:
- You write **plain text with special commands** (called "markup").
- The system then **compiles** that text into a beautifully formatted PDF.

| Word Processor (e.g., MS Word) | LaTeX |
|---|---|
| Format visually as you type | Write code, then compile to see result |
| Easy for short/simple documents | Best for long, structured, technical documents |
| Manual formatting (headings, spacing) | Automatic, consistent formatting |
| Manual reference/citation management | Automatic numbering of equations, figures, citations |

### What is Overleaf?
**Overleaf** is a free, **online LaTeX editor** that lets you write and compile LaTeX documents directly in your web browser — no software installation required.

**Key features of Overleaf:**
- 🌐 **Cloud-based:** Access your documents from any device with internet.
- 👥 **Real-time collaboration:** Multiple people can edit the same document simultaneously (like Google Docs, but for LaTeX).
- 📄 **Live preview:** See the compiled PDF update as you type.
- 📚 **Templates:** Tons of ready-made templates for resumes, papers, presentations, and reports.
- 🔄 **Version history:** Track changes to your document over time.

> 💡 **Why learn this?** Many universities, research journals, and conferences require papers to be submitted in LaTeX format because of its clean, professional, and consistent output.

### Getting Started with Overleaf
1. Go to **overleaf.com** and create a free account.
2. Click **"New Project"** → choose **"Blank Project"** or a template.
3. You'll see two panels:
   - **Left panel:** Your `.tex` source code (where you write).
   - **Right panel:** The live-compiled PDF preview.
4. Click **"Recompile"** to update the preview after making changes.

---

## 9. Basic LaTeX Document Structure

Every LaTeX document follows this basic skeleton:

```latex
\documentclass{article}

\begin{document}

Hello, World! This is my first LaTeX document.

\end{document}
```

### Breaking it down:

| Line | Purpose |
|---|---|
| `\documentclass{article}` | Defines the type of document (article, report, book, letter, etc.) |
| `\begin{document}` | Marks the **start** of the visible content |
| `\end{document}` | Marks the **end** of the document |
| Everything in between | The actual content that will appear in the PDF |

### Common LaTeX Commands

| Command | Purpose | Example |
|---|---|---|
| `\title{}` | Sets the document title | `\title{My First Paper}` |
| `\author{}` | Sets the author name | `\author{John Doe}` |
| `\section{}` | Creates a numbered section heading | `\section{Introduction}` |
| `\subsection{}` | Creates a sub-heading | `\subsection{Background}` |
| `\textbf{}` | Bold text | `\textbf{important}` |
| `\textit{}` | Italic text | `\textit{emphasis}` |
| `\begin{itemize}` | Starts a bullet-point list | See below |
| `\begin{equation}` | Inserts a numbered math equation | See below |

### Example: A Small Document with Sections and a List

```latex
\documentclass{article}
\title{Introduction to LaTeX}
\author{Jane Student}

\begin{document}
\maketitle

\section{Introduction}
LaTeX is great for writing \textbf{technical documents}.

\subsection{Why use it?}
\begin{itemize}
    \item Clean formatting
    \item Great for math
    \item Free and open source
\end{itemize}

\end{document}
```

> 📌 **Tip:** LaTeX is *whitespace-insensitive* — extra spaces and blank lines in your code usually don't affect the output. Formatting is controlled by commands, not spacing.

---

## 10. Introduction to Version Control & Git

### What is Version Control?
**Version control** is a system that records changes to files over time, so you can:
- See what changed, when, and who changed it.
- Revert back to an older version if something breaks.
- Work on the same project with multiple people **without overwriting each other's work**.

Think of it like an infinite "undo" history combined with a collaboration tool.

### What is Git?
**Git** is the most popular **version control system**, created by Linus Torvalds (the creator of Linux). It runs locally on your computer and tracks changes to your project files.

### Key Git Concepts

| Term | Meaning |
|---|---|
| **Repository (Repo)** | A folder that Git is tracking — contains your project files and full history |
| **Commit** | A "snapshot" or save-point of your project at a specific time, with a message describing the change |
| **Branch** | A separate line of development — lets you work on new features without affecting the main project |
| **Merge** | Combining changes from one branch into another |
| **Clone** | Downloading a copy of a repository to your own computer |
| **Push** | Uploading your local commits to an online repository (like GitHub) |
| **Pull** | Downloading the latest changes from an online repository to your computer |

---

## 11. GitHub Basics

### What is GitHub?
**GitHub** is a **cloud-based hosting service** for Git repositories. While Git is the tool that tracks changes, GitHub is the **website/platform** where you store, share, and collaborate on those repositories online.

> 🔑 **Simple analogy:** Git is like the engine, GitHub is like the online garage where you park and share your car with others.

### Why Use GitHub?
- ☁️ **Backup:** Your code is safely stored in the cloud.
- 🤝 **Collaboration:** Teams can work on the same project without conflicts.
- 📜 **History:** Every change is logged — you can see exactly what was changed and by whom.
- 🌍 **Portfolio:** Showcase your projects publicly to employers or collaborators.
- 🐛 **Issue tracking:** Report bugs and manage tasks within a project.

### Key GitHub Features

| Feature | Description |
|---|---|
| **Repository (Repo)** | The online home of your project on GitHub |
| **README.md** | A markdown file that describes your project (like this one!) |
| **Fork** | Creates your own copy of someone else's repository |
| **Pull Request (PR)** | A request to merge your changes into someone else's repository |
| **Issues** | A place to report bugs or suggest features |
| **Star** | Bookmarking/favoriting a repository you like |

---

## 12. Essential Git Commands

Here are the fundamental commands you'll use when working with Git and GitHub:

| Command | What It Does |
|---|---|
| `git init` | Initializes a new Git repository in the current folder |
| `git clone <url>` | Copies (downloads) a remote repository to your computer |
| `git status` | Shows which files have been changed |
| `git add <file>` | Stages a file (marks it as ready to be committed) |
| `git add .` | Stages **all** changed files at once |
| `git commit -m "message"` | Saves a snapshot of staged changes with a description |
| `git push` | Uploads your commits to GitHub |
| `git pull` | Downloads the latest changes from GitHub |
| `git branch` | Lists all branches, or creates a new one |
| `git checkout <branch>` | Switches to a different branch |
| `git merge <branch>` | Merges another branch into your current branch |
| `git log` | Shows the commit history |

---

## 13. Typical Git Workflow

Here's the standard cycle you'll follow when working on a project:

1. **Clone the repository** (only once, to get a local copy):
   ```bash
   git clone https://github.com/username/repository.git
   ```
2. **Make changes** to your files (edit code, add new files, etc.)
3. **Check what changed:**
   ```bash
   git status
   ```
4. **Stage your changes:**
   ```bash
   git add .
   ```
5. **Commit your changes** with a clear message:
   ```bash
   git commit -m "Added login feature"
   ```
6. **Push your changes** to GitHub:
   ```bash
   git push
   ```
7. **Pull before you start working again** (to get teammates' latest updates):
   ```bash
   git pull
   ```

> ⚠️ **Best Practice:** Always write clear, descriptive commit messages (e.g., `"Fix navbar bug"` instead of `"update"`) so your project history stays understandable.

---

## 14. Week 2 Quick Recap

✅ **Overleaf** = an online editor for writing LaTeX documents with live PDF preview and collaboration
✅ **LaTeX** = a markup-based system for creating professional, technical documents
✅ Every LaTeX doc needs `\documentclass{}`, `\begin{document}`, and `\end{document}`
✅ **Git** = a version control system that tracks changes to your files over time
✅ **GitHub** = a cloud platform for hosting and collaborating on Git repositories
✅ Core workflow: **clone → edit → add → commit → push → pull**

---

### 📚 Recommended Next Step
Create a free account on **overleaf.com** and **github.com**, then try creating a simple LaTeX document and a basic GitHub repository to practice the commands above!

---
---

# 📝 Week 3: Word Processing Tools – Basics (MS Word / Google Docs)

This lecture covers **word processing software** — the tools you'll use most often to create everyday business and academic documents like letters, resumes, and reports.

---

## 15. Introduction to Word Processing Tools

### What is a Word Processor?
A **word processor** is software used to create, edit, format, and print text-based documents. Unlike a plain text editor, it lets you control fonts, spacing, layout, images, and much more.

### Popular Word Processing Tools

| Tool | Type | Key Advantage |
|---|---|---|
| **Microsoft Word** | Desktop/offline (with cloud sync via Microsoft 365) | Industry-standard, powerful formatting & templates |
| **Google Docs** | Cloud-based, browser-only | Free, real-time collaboration, auto-saves to Google Drive |

| Feature | MS Word | Google Docs |
|---|---|---|
| Works offline | ✅ Yes | ⚠️ Limited (needs setup) |
| Real-time collaboration | ⚠️ Requires OneDrive/365 | ✅ Built-in, seamless |
| Cost | Paid (or one-time license) | Free |
| Advanced formatting tools | ✅ More extensive | ✅ Good, but simpler |
| Auto-save | Manual/periodic | ✅ Automatic, continuous |

> 💡 **Why this matters:** Whether you're applying for a job, writing a report, or drafting a business letter, word processors are the primary tool used in almost every office and academic setting.

---

## 16. Creating Business Documents

Word processors are commonly used to create **standardized business documents**. Here's what each one is and how it's typically structured:

### 📩 Business Letters
A formal letter used for professional communication (e.g., job applications, complaints, official requests).

**Standard structure:**
```
[Your Name]
[Your Address]
[Date]

[Recipient's Name]
[Recipient's Address]

Dear [Recipient's Name],

[Opening paragraph – state the purpose of the letter]
[Body paragraph(s) – details/explanation]
[Closing paragraph – call to action or summary]

Sincerely,
[Your Signature]
[Your Printed Name]
```

### 📋 Memos (Memorandums)
A short, internal document used to communicate information within an organization (announcements, policy updates, reminders).

**Standard structure:**
```
MEMO

To:      [Recipient(s)]
From:    [Sender]
Date:    [Date]
Subject: [Brief topic of the memo]

[Body — direct and concise message]
```

> 📌 Unlike letters, memos skip the greeting/closing and get straight to the point.

### 📄 Resumes (CVs)
A summary of your education, skills, and work experience — used when applying for jobs.

**Standard sections:**
| Section | Purpose |
|---|---|
| **Contact Information** | Name, phone, email, LinkedIn/portfolio |
| **Summary/Objective** | A short pitch about who you are and what you're looking for |
| **Education** | Degrees, institutions, graduation dates |
| **Work Experience** | Job titles, companies, dates, key achievements |
| **Skills** | Technical and soft skills relevant to the job |
| **Certifications/Projects** | Extra credentials or notable work |

> ✅ **Tip:** Keep resumes to **1 page** (especially for students/entry-level roles), use consistent formatting, and tailor them to each job application.

---

## 17. Formatting Tools

Formatting makes documents easier to read and more professional. Here are the essential tools found in both MS Word and Google Docs:

### Headings
Used to organize a document into sections (like this README uses `#`, `##`, `###`).
- **Heading 1** → Main titles
- **Heading 2** → Section titles
- **Heading 3** → Sub-section titles

> 💡 Using proper heading styles (instead of just making text bold/bigger) allows Word/Docs to auto-generate a **Table of Contents**.

### Bullets & Numbering

| Type | Use Case | Example |
|---|---|---|
| **Bullet points** | Unordered lists (no specific sequence matters) | • Item A <br> • Item B |
| **Numbered lists** | Ordered/sequential steps or ranked items | 1. Step one <br> 2. Step two |

### Indentation
Indentation shifts text inward from the margin — used to:
- Show hierarchy in lists (sub-points).
- Highlight quotes or specific paragraphs.
- Follow formatting rules (e.g., first line of a paragraph in some styles).

### Other Common Formatting Tools

| Tool | Function |
|---|---|
| **Bold / Italic / Underline** | Emphasize specific text |
| **Font & Font Size** | Controls the style and size of text |
| **Text Alignment** | Left, Center, Right, Justify |
| **Line Spacing** | Controls space between lines (e.g., single, 1.5, double) |
| **Styles** | Pre-set formatting combinations (Heading 1, Normal, Quote, etc.) |

---

## 18. Page Setup, Header/Footer

### Page Setup
Controls the overall layout of your document:

| Setting | Description |
|---|---|
| **Margins** | The blank space around the edges of the page |
| **Orientation** | Portrait (tall) or Landscape (wide) |
| **Paper Size** | A4, Letter, Legal, etc. |
| **Columns** | Split text into 2 or more vertical columns (e.g., newsletters) |

### Header & Footer
- **Header:** The area at the **top** of every page — commonly used for document titles, chapter names, or logos.
- **Footer:** The area at the **bottom** of every page — commonly used for page numbers, dates, or company info.

> ✅ **Use case:** In a school report, you might put the **subject name** in the header and **page numbers** in the footer.

**How to add one (general steps):**
1. Go to the **Insert** menu.
2. Select **Header & Footer** (or "Header/Footer" in Google Docs).
3. Type your content — it will automatically repeat on every page.

---

## 19. Working with Tables

Tables organize information into **rows and columns** — useful for schedules, comparisons, data summaries, and structured lists.

**How to insert a table (general steps):**
1. Go to the **Insert** menu → **Table**.
2. Choose the number of rows and columns.
3. Click into any cell to start typing.

### Common Table Actions

| Action | Purpose |
|---|---|
| **Merge cells** | Combine multiple cells into one (e.g., for a title row) |
| **Split cells** | Divide one cell into multiple |
| **Add/delete rows or columns** | Adjust table size as needed |
| **Table borders & shading** | Improve visual clarity and style |
| **Sort table data** | Organize rows alphabetically or numerically |

> 💡 **Example use:** A resume might use a table (with hidden borders) to neatly align job titles on the left and dates on the right.

---

## 20. Working with Images

Adding visuals makes documents more engaging and easier to understand.

**How to insert an image (general steps):**
1. Go to the **Insert** menu → **Image/Picture**.
2. Choose to upload from your device, or insert from a URL/Drive.
3. Click and drag the corners to resize.

### Image Formatting Options

| Option | Function |
|---|---|
| **Text Wrapping** | Controls how text flows around the image (e.g., square, behind text, in line with text) |
| **Alt Text** | A description of the image for accessibility (screen readers) and SEO |
| **Cropping** | Trims unwanted parts of the image |
| **Alignment** | Positions the image left, center, or right on the page |
| **Captions** | Adds a labeled description below the image (e.g., "Figure 1: Sales Growth") |

> 📌 **Best practice:** Always compress large images before inserting them to keep file size manageable, and use **captions** in formal/academic documents.

---

## 21. Week 3 Quick Recap

✅ **Word processors** (MS Word, Google Docs) are used to create formatted text documents
✅ Common business documents: **letters, memos, resumes** — each with its own standard structure
✅ Formatting tools: **headings, bullets, numbering, indentation** help organize content clearly
✅ **Page setup** controls margins/orientation; **headers/footers** repeat content on every page
✅ **Tables** organize data into rows & columns; **images** make documents visual and engaging

---

### 📚 Recommended Next Step
Open MS Word or Google Docs and try creating a one-page resume using headings, bullet points, and a table for your work experience/education — this is one of the most practical skills from this lecture!
