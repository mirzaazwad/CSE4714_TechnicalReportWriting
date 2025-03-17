# LaTeX Guide: Mathematical Notation and Formatting

## 1. **Document Structure**
### **Basic Setup**
```latex
\documentclass[12pt, a4paper]{article}  % Defines article class with 12pt font size and A4 paper size.
\usepackage[margin=1in]{geometry}      % Sets 1-inch margins.
\usepackage{stix2}                     % Uses STIX Two font for better typography.
\usepackage[colorlinks]{hyperref}       % Enables clickable links with color.
\usepackage{amsmath, amssymb}           % Provides enhanced math symbols and environments.
```

## 2. **Text Formatting**
### **Quotation Marks**
Use double backticks (``) and double apostrophes ('') to generate proper quotation marks:
```latex
``The teacher said, ``You must take permission.''
```

## 3. **Mathematical Expressions**
### **Math Modes**
- **Inline Math:** `$(a + b)^2 = a^2 + 2ab + b^2$`
- **Alternate Inline Math:** `\( (a + b)^2 = a^2 + 2ab + b^2 \)`
- **Display Math (centered):**
  ```latex
  \[ (a + b)^2 = a^2 + 2ab + b^2 \]
  ```
- **Using `equation` environment:**
  ```latex
  \begin{equation}
      (a + b)^2 = a^2 + 2ab + b^2
  \end{equation}
  ```

### **Super and Subscripts**
Use `^{}` for superscripts and `_ {}` for subscripts:
```latex
\begin{equation}
    a^{3.14} + b_{(i, j)}
\end{equation}
```

### **Fractions & Square Roots**
- **Basic fraction:** `\frac{a}{b}`
- **Square root:** `\sqrt{x}`
- **Complex expression:**
  ```latex
  \begin{equation}
      \sqrt{\frac{(a + b)}{(a - b)}}
  \end{equation}
  ```

### **Operators & Trigonometry**
Use `\sin`, `\cos`, `\tan`:
```latex
\begin{equation}
    \sin^2\theta + \cos^2\theta = 1
\end{equation}
```

### **Brackets & Parentheses**
Use `\left` and `\right` for automatic resizing:
```latex
\begin{equation}
    \left( \frac{a}{b} \right)
\end{equation}
```

## 4. **Greek Alphabets & Calculus**
### **Greek Letters**
```latex
\alpha \beta \gamma \delta \Gamma \Delta
```

### **Limits & Integrals**
```latex
\begin{equation}
    \lim_{x \to \infty} \frac{1}{x} = 0
\end{equation}
```
```latex
\begin{equation}
    \int_{0}^{100} x dx = 500
\end{equation}
```

## 5. **Calligraphy & Sets**
```latex
\begin{equation}
    \mathcal{ABCDE} \mathbb{ABCDE}
\end{equation}
```
```latex
\begin{equation}
    A \cup B = C \cap D, \text{ for all } x \in \mathbb{Z}
\end{equation}
```

## 6. **Vectors & Comparison Operators**
```latex
\begin{equation}
    \vec{A} \times \vec{B} = \vec{C}, \quad \hat{i} \times \hat{j} = \hat{k}
\end{equation}
```

```latex
\begin{equation}
    1 = 1 < 2 > 5 \neq 10 \geq 2 \leq 5
\end{equation}
```

## 7. **Advanced Math Environments**
### **Multiline Equations**
```latex
\begin{multline}
    a + b + c + d + e + f + g + h + i + j \\
    + k + l + m + n + o + p + q + r = 10
\end{multline}
```

### **Splitting Equations**
```latex
\begin{equation}
    \begin{split}
         x &= \frac{10}{20} \\
         &= \frac{1}{2} \\
         &= 0.5
    \end{split}
\end{equation}
```

### **Alignment of Equations**
```latex
\begin{align}
    a + 2b - 3c &= 10 \\
    2a + 5b + 6c &= -2 \\
    -a + b + 6c &= -4
\end{align}
```

### **Matrix Representation**
```latex
\begin{equation*}
    \mathbf{A} = \begin{bmatrix}
        1 & 2 & 3 \\
        4 & 5 & 6 \\
        7 & 8 & 9 \\
    \end{bmatrix}
\end{equation*}
```

## **Conclusion**
This document provides an **easy-to-remember** guide for writing LaTeX mathematical expressions with examples and best practices. 
