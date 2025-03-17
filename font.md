In **LaTeX**, you can change font size in multiple ways depending on whether you want to adjust it **locally (for specific text)** or **globally (for the whole document)**. 

---

### **1. Changing Font Size Locally**
Use LaTeX font size commands inside braces `{}` to apply them to specific text.

```latex
{\tiny Tiny Text}
{\scriptsize Script Size Text}
{\footnotesize Footnote Size Text}
{\small Small Text}
{\normalsize Normal Size (Default)}
{\large Large Text}
{\Large Larger Text}
{\LARGE Even Larger Text}
{\huge Huge Text}
{\Huge Hugest Text}
```
 **Example**:
```latex
This is {\Large a large text} inside normal text.
```

---

### **2. Changing Font Size Globally**
Modify the font size for the whole document using **document class options**.

```latex
\documentclass[12pt]{article}  % Other options: 10pt (default), 11pt
```

Alternatively, for section titles and other elements, use `\renewcommand{\...}`:
```latex
\renewcommand{\normalsize}{\large}  % Changes normal text to \large
```

---

### **3. Changing Font Size for a Whole Section**
To change font size for a larger block of text:
```latex
\begingroup
\Large
This entire block is in large font.
\endgroup
```

Or use the `\fontsize{size}{baselineskip}\selectfont` command:
```latex
\fontsize{14pt}{16pt}\selectfont This text is 14pt.
```

