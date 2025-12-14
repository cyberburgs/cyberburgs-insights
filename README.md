# Cyberburgs Insights - Contribution Guide

Welcome to the **Cyberburgs Insights** repository. This repository hosts main blog content for the Cyberburgs website. The website's "Smart Sync" engine automatically fetches posts from here.

## 📝 How to Upload a Blog Post

To publish a new blog post on the website, simply create a new Markdown file (`.md`) in this repository.

### 1. File Naming
Name your file using lowercase letters and hyphens. This filename will become the URL of the post.
*   **Good:** `ransomware-analysis-2025.md` -> `cyberburgs.com/blog/ransomware-analysis-2025`
*   **Bad:** `Ransomware Analysis.md` (Avoid spaces and uppercase)

### 2. Frontmatter (Metadata)
Every file **MUST** start with a metadata block (Frontmatter) enclosed in `---`. This tells the website the title, author, and category.

**Copy and paste this template at the very top of your file:**

```markdown
---
title: Your Blog Post Title Here
date: 2025-12-14
author: Your Name
category: Threat Analysis
description: A short summary of the article (1-2 sentences) that will appear on the card.
---

# Your Main Heading

Write your article content here using standard Markdown.

## Subheading
- Bullet point 1
- Bullet point 2
```

### 3. Supported Categories
Use one of these categories for consistent tagging:
*   `Threat Analysis`
*   `Innovation`
*   `Architecture`
*   `Forensics`
*   `General`

### 4. Images
Currently, the system serves a default image for all blogs. (Advanced image support coming soon).

## 🤖 Using AI to Write Blogs (GPT Prompt)

You can use ChatGPT or any AI to automatically format your content for this blog. Copy and paste this prompt:

> **"I have some raw content about [TOPIC]. Please convert it into a Markdown blog post file for my cybersecurity blog. You MUST follow these strict formatting rules:**
>
> 1.  **Frontmatter**: Start the file with this metadata block:
>     ```yaml
>     ---
>     title: [Create a catchy, hacker-style title]
>     date: [Today's Date YYYY-MM-DD]
>     author: [My Name]
>     category: [Choose one: Threat Analysis, Innovation, Architecture, Forensics]
>     description: [A 2-sentence summary]
>     ---
>     ```
> 2.  **Formatting**:
>     *   Use `# Main Heading` for the title.
>     *   Use `## Subheadings` for sections.
>     *   Use **bold** for key terms.
>     *   Use `inline code` for technical terms (paths, commands, tools).
>     *   Use code blocks (```bash or ```python) for scripts/commands.
> 3.  **Tone**: Professional, technical, enterprise cybersecurity.
>
> **Here is my raw content:**
> [PASTE YOUR CONTENT HERE]"

## 🚀 Publishing
1.  **Commit** your `.md` file to the `main` branch.
2.  **Wait ~5 minutes** or ask an admin to restart the website server.
3.  Your post will automatically appear in the **Insights** section!
