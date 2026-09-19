# LaTeX Resume Template

This folder contains a clean, professional, ATS-friendly LaTeX resume template specifically designed for technical roles.

## What is LaTeX?
LaTeX is a document preparation system often used in academia and technical fields. Instead of formatting text visually (like in Microsoft Word), you write plain text with special commands to define the structure, and LaTeX compiles it into a perfectly formatted PDF.

## Why use this template?
- **ATS-Friendly:** It's single-column and text-based, making it easy for Applicant Tracking Systems to read.
- **Clean Formatting:** Consistent margins, fonts, and spacing are handled automatically.
- **Professional:** It avoids distracting graphics, photos, or multiple colors, focusing purely on your content.

## How to Use in Overleaf

You don't need to install anything on your computer to use this template! We recommend using Overleaf, a free online LaTeX editor.

1. Create a free account at [Overleaf.com](https://www.overleaf.com/).
2. Click **New Project** -> **Blank Project** and give it a name (e.g., "My Resume").
3. Overleaf will generate a default `main.tex` file. Clear all the code inside it.
4. Copy the entire contents of `resume-template.tex` from this repository and paste it into your Overleaf `main.tex` file.
5. Click the green **Recompile** button (or press `Ctrl + S` / `Cmd + S`) to see the PDF preview on the right.

## How to Edit Your Resume

### 1. What to Edit
Look for the comments in the code (lines starting with `%`). They will guide you!

- **Header:** Replace "Firstname Lastname", email, phone, and links.
- **Content:** Replace the sample university, jobs, and projects with your own.

**Example: Adding an Experience**
```latex
\resumeEntry
    {Your Job Title --- Company Name}
    {Start Date -- End Date}
    {Location}

\begin{itemize}
    \item Your first bullet point describing what you did.
    \item Your second bullet point describing impact.
\end{itemize}
```

**Example: Adding a Project**
```latex
\projectEntry
    {Project Name --- Subtitle/Context}
    {Date}

\begin{itemize}
    \item Description of what you built and how you built it.
    \item \href{https://link-to-project.com}{Live Demo}
\end{itemize}
```

### 2. Adding/Removing Sections
To remove an entire section (e.g., "Open Source Contributions"), simply delete or comment out (using `%` at the start of each line) the code block from `\section{...}` down to the end of that section's content.

### 3. Hyperlinks
To add a clickable link, use the `\href` command:
`\href{URL}{\underline{Text to display}}`

### 4. What NOT to Modify (Unless you know LaTeX)
- The header packages (`\usepackage{...}`)
- Formatting commands at the top (`\newcommand{...}`)
- Page geometry (`margin=0.75in`)
- These dictate the structural layout of the resume. Changing them might break the alignment.

## Downloading the PDF
Once you are happy with the preview:
1. Click the **Download PDF** icon on the top right of the PDF viewer in Overleaf.
2. Rename the file to something professional (e.g., `Firstname_Lastname_Resume.pdf`).
3. **Always open and read your downloaded PDF** to ensure everything looks correct before sending it to recruiters!
