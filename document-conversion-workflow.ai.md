## 📄 Chapter Conversion Workflow

### 1. **Automated PDF-to-Markdown Translation**
- Use your Python PDF-OCR notebook to extract text and images from the source PDF (`1-1-Output.pdf`).
- Output is saved as raw markdown (`output.md`) and supporting files (e.g., `ocr_response.json`, images).

### 2. **Initial Data Cleaning**
- Open the raw markdown output.
- Remove OCR artifacts, fix broken formatting, and ensure all content is present.

### 3. **Apply Repository Standards**
- Add the required frontmatter template at the top of the file:
```yaml
---
title: "1.0 First Program"
description: "A chapter on first program in C++."
course: "CS 124"
unit: "Unit 1"
chapter: "1.0"
tags:
    - cpp
    - procedural-programming
source:
    type: "AI-Generated Draft"
    method: "Mistral OCR"
    model: mistral-ocr-2505-completion
    original: "1-1-Output.pdf"
    generated: "2025-08-08T16:01:00-07:00"
    pages_processed: 12
    doc_size_bytes: 551389
    document_annotation: null
author:
    name: "Procedural Programming in C++"
    author: "James Helfrich"
    description: "CS 124 Textbook"
    ASIN: "B0DTWH6ZWQ"
---

# Title
<!-- ... -->
```

### 4. **Format Callouts and Code Blocks**
- Convert important notes, tips, warnings, and examples to the standardized callout syntax:
  > [!WARNING] Critical information

  > [!TIP] Helpful advice

  > [!EXAMPLE] Sample code or usage
- Use the correct code block shading and style for readability, matching the CSS themes.

### 5. **Image and Asset Handling**
- Ensure all image paths are relative (not absolute), generally prefixed with `(../../../)`.
- Place images in the appropriate `images/` folder and update links in markdown.

### 6. **Educational Enhancements**
- Add character callouts (Sue’s Tips, Sam’s Corner) where relevant:
  > [!DANGER] 💡 **Sue's Tip:**
  > ![Sue](.vscode/assets/sue.png){width=50 align=right}
  > Practical advice...

  > [!TLDR] 🤓 **Sam's Corner:**
  > ![Sam](.vscode/assets/sam.png){width=50 align=right}
  > Technical details...

### 7. **Final Review and Consistency**
- Align headers, check code block formatting, and ensure all sections follow the repository’s style.
- Compare with a completed chapter (e.g., `1-0-First-Program.ai.md`) for consistency.

### 8. **Save as Final Chapter File**
- Save the cleaned and formatted markdown as `1-1-Output.ai.md` in the chapter folder.

### 9. **PDF Export (Optional)**
- Use VS Code’s Markdown Extended extension to export the final markdown to PDF for review.

---

> [!summary] 📋 Example: Converting `1.1-Output` to match `1.0-First-Program` Finalized Format (this was written before this change)
> 
> To convert the `1.1-Output` folder to match the processed state of `1.0-First-Program`, follow these steps:
> 
> 1. **Locate Raw Outputs**  
>     - Find `output.md` and `ocr_response.json` in `1-1-Output/`.
> 
> 2. **Clean Raw Markdown**  
>     - Open `output.md` and remove OCR errors, fix formatting, and ensure all content is present.
> 
> 3. **Apply Repository Standards**  
>     - Add the frontmatter template at the top of the markdown file.
>     - Ensure the chapter title and metadata are accurate.
> 
> 4. **Format Content**  
>     - Convert notes, tips, warnings, and examples to standardized callout syntax.
>     - Format code blocks for readability.
> 
> 5. **Handle Images and Assets**  
>     - Move all images to `1-1-Output/images/`.
>     - Update image links in markdown to use relative paths (e.g., `(../../../images/filename.png)`).
> 
> 6. **Add Educational Enhancements**  
>     - Insert character callouts (Sue’s Tips, Sam’s Corner) where appropriate.
> 
> 7. **Review for Consistency**  
>     - Compare with `1-0-First-Program.ai.md` to ensure formatting and style match.
> 
> 8. **Save Final Markdown**  
>     - Save the cleaned and formatted file as `1-1-Output.ai.md` in the `1-1-Output` folder.
> 
> 9. **Optional PDF Export**  
>     - Use VS Code’s Markdown Extended extension to export the final markdown to PDF.
> 
> **Result:**  
> `1-1-Output` will now contain a finalized markdown file (`1-1-Output.ai.md`), matching the structure and standards of `1-0-First-Program`.