# Rust Book Index Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Add a legal, newest-first Rust learning-resource index with concise summaries and direction guidance, without adding book files.

**Architecture:** `README.md` remains the single reader-facing catalogue. Each resource table row records the year, direction, concise overview, and a first-party URL; a short reading-path section maps common goals to rows. The Git index is checked before committing to exclude PDF, EPUB, MOBI, and other book binaries.

**Tech Stack:** Markdown, Git sparse checkout, PowerShell HTTP requests.

---

### Task 1: Verify candidate resources and URLs

**Files:**

- Modify: `README.md`

- [ ] **Step 1: Assemble current, legal candidates from first-party sources**

Use resources published or materially updated in 2026 or 2025 where available, plus maintained official Rust documentation for coverage. Record only a source URL controlled by the publisher, author, Rust project, or resource repository.

- [ ] **Step 2: Check each source is reachable**

Run a PowerShell `Invoke-WebRequest -Method Head` request for every candidate URL, allowing up to five redirects.

Expected: Each URL returns a successful HTTP response after redirects.

- [ ] **Step 3: Exclude unsuitable candidates**

Do not include a candidate if its URL is a third-party file-sharing or piracy site, if the publisher cannot be identified, or if its access type cannot be described accurately as online reading or official download.

### Task 2: Write the reader-facing book index

**Files:**

- Modify: `README.md`

- [ ] **Step 1: Replace the two-line README with catalogue structure**

Add a title, a legal-source policy, a newest-first table, and a reading-path section. Keep the existing Chinese audience and state clearly that no files need to be downloaded from the repository.

- [ ] **Step 2: Add one complete row per resource**

Use this exact Markdown table shape for every row:

```markdown
| 年份/状态 | 书籍或资源 | 方向 | 概要 | 访问 |
| --- | --- | --- | --- | --- |
| 2026 | Example | CLI | 从参数解析到发布流程的实战指南。 | [在线阅读](https://example.com/) |
```

Expected: Every row contains a title, a year/status, a direction, a one-sentence overview, and a legal first-party link.

- [ ] **Step 3: Order resources newest-first**

Place verified 2026 resources before 2025 resources. Put maintained official documents after dated releases, explicitly labeled as continuously maintained so readers do not infer a publication year.

- [ ] **Step 4: Add goal-based reading paths**

Add six concise bullets for: beginner language learning, asynchronous/concurrent services, CLI tools, Web services, embedded/no-std, and compiler/build tooling. Each bullet must name one or more catalogue resources.

### Task 3: Validate and commit without book files

**Files:**

- Modify: `README.md`

- [ ] **Step 1: Validate Markdown coverage**

Check that the README contains the five table headings and the reading-path heading.

Expected: The validation exits successfully without reporting a missing heading.

- [ ] **Step 2: Check staged content and whitespace**

Stage `README.md` with `git add --sparse README.md`, then run `git diff --cached --check` and `git diff --cached --name-only`.

Expected: No whitespace errors; the only staged content file is `README.md` (the already committed design and plan files are not restaged).

- [ ] **Step 3: Commit the index update**

Run `git commit -m "docs: add latest Rust learning resource index"`.

Expected: One commit containing the README index only; no PDF, EPUB, MOBI, or other book file is committed.

- [ ] **Step 4: Remove the abandoned normal-clone directory**

Remove the task-created incomplete clone at `D:\Downloads\Rust_Books`, then confirm its path no longer exists. Keep the sparse working clone until the user no longer needs local repository access.

## Self-review

- Spec coverage: Task 1 enforces legal, current sources; Task 2 implements newest-first summaries and study directions; Task 3 verifies links, Markdown, and the no-book-files requirement.
- Scope: The plan changes only documentation and the task-created incomplete clone; it does not mirror or modify books.
- Ambiguity resolved: official online reading links are preferred over direct file downloads, and link labels state the access type.
