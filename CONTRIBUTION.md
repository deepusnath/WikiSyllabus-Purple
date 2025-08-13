
# 📚 Contribution Guide

Thank you for your interest in contributing to this WikiSyllabus Repository! 🙌  
Together, we can make a fully open, searchable, and markdown-based syllabus index for students, teachers, and developers.

---

## 📌 What You Can Contribute

- ✅ **New Syllabus Files**  
  - Add missing course markdowns (`.md`) for different branches, semesters, or years.
- 🛠️ **Fix Errors**  
  - Typos, outdated content, or formatting issues.
- 📘 **Add References**  
  - Useful books, links, or official sources for specific courses.
- 💡 **Improve Structure**  
  - Suggestions for folder naming, file structure, or tagging.

---

## 🗂 Folder & File Naming Convention

- Follow this structure:

```

universities/university/branch/year/semester/xx.md

```

✅ Example:

```

universities/ktu/computer-science/2019/s8/01.md

````

### 🔹 Rules

- ✅ **Every file and directory name must be written in lowercase.**  
- 🔁 If you come across any uppercase in structure, **rename them to lowercase.**
- ✅ Filenames should always be **numbers** (e.g., `01.md`, `02.md`, ...)
- ❌ Do **not** use course codes in filenames.
- ✅ Course details like code/title should be inside the **YAML frontmatter**
- ✅ For multiple words in folder names, use **hyphens**, not underscores or spaces.

---

## 📝 Markdown File Format

Each `.md` file must start with YAML frontmatter:
```yaml
---
country: "india"
university: "ktu"
branch: "computer-science"
version: "2019"
semester: 8
course_code: "cst402"
course_title: "distributed-computing"
language: "english"
contributor: "@your-github-username"
---


````

### 📄 Common Papers

Some papers are **shared between multiple courses**.
To keep things clean and avoid duplication:

* **Folder Structure:**

```
universities/common-paper/<year>/<semester>/<xx>.md
```

Example:

```
universities/common-paper/2019/s1/01.md
```

* **YAML Frontmatter:**

```yaml
---
country: "india"
university: "ktu"
branch: "common-paper"
version: "2019"
semester: 1
course_code: "mat101"
course_title: "engineering-mathematics-1"
language: "english"
common_for: ["computer-science", "mechanical-engineering", "electrical-engineering"]
contributor: "@your-github-username"
---
```

> `common_for` lists the branches/courses this paper is applicable to.

---
Follow this with the syllabus content (objectives, content, references, etc.)

---

## 📝 How to Contribute

### 1. **Fork the Repository**

Create your own copy of the repository to work on.

### 2. **Create a New Branch**

```bash
git checkout -b feat/add-cst402
```

### 3. **Add Your Markdown File**

Use the correct folder structure and file naming convention.

### 4. **Commit Your Changes**

```bash
git add .
git commit -m "feat: add cst402 - distributed computing"
```

### 5. **Push and Make a Pull Request**

```bash
git push origin feat/add-cst402
```

Then go to GitHub and open a **Pull Request (PR)** to the **main** branch using the format given below.

---

### 🏷️ PR Title Format

Please follow this format for your Pull Request title:

```md
<university-name> <course-name> <year> <semester>
```

#### ✅ Example:

```md
KTU Chemical Engineering 2019 S1
```

#### 🔁 For multiple semesters in one PR:

```md
KTU Chemical Engineering 2019 S1-S6
```

---

### 📝 Add a Meaningful Description in Your PR

When creating your Pull Request, **please include a short description** that explains:

* What syllabus/courses you added or edited
* Any file restructuring you performed
* Any other relevant changes or notes

✅ This helps reviewers quickly understand your contribution and speeds up the approval process!

---

## 🔍 Before You Submit

- ✅ Check if the course already exists.
- ✅ Double-check formatting and spelling.
- ✅ Add your GitHub username as `contributor`.
- ✅ Ensure **all folders and files are lowercase**.
- ✅ Confirm naming and structure matches the guidelines.

---

## 🤝 Code of Conduct

Please follow the [CODE\_OF\_CONDUCT.md](./CODE_OF_CONDUCT.md).
Be respectful, inclusive, and collaborative — this is a shared space for learning and helping others.

---

## 🙋 Need Help?

Open an [issue](https://github.com/The-Purple-Movement/WikiSyllabus/issues) or tag a maintainer (e.g., `@admin`) in your PR for assistance.

---

Together, let’s build the best open academic resource!
