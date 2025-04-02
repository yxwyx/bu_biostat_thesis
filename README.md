# Boston University Biostatistics Thesis Template

This repository contains a LaTeX template formatted according to the thesis requirements of the Department of Biostatistics at Boston University. It includes built-in support for BU’s formatting rules, commonly-used LaTeX packages, and helper files to streamline the writing of a doctoral dissertation.

The BU-specific LaTeX style is adapted from an MIT style file by **Stephen Gildea**, modified for BU by **Paolo Gaudiano**, **Jonathan Polimeni**, **Janusz Konrad**, **Cameron Morland**, **Karen Yeats**, and most recently updated by **Hanna Gerlovin** in 2018.

---

## 🏗️ Project Structure

```bash
.
├── bu_math_thesis.sty          # BU-specific formatting style file
├── Thesis.tex                  # Main LaTeX file
├── chapters/
│   ├── Acknowledgements.tex
│   ├── Abstract.tex
│   ├── chapter1.tex
│   ├── chapter2.tex
│   ├── chapter3.tex
│   ├── Symbols.tex
│   ├── Glossary.tex
│   ├── AppendixA.tex
│   ├── Journals.tex
├── figures/                    # All figure files should go here
├── tables/                     # All table files should go here
├── Thesis.bib                  # Bibliography file in BibTeX format
└── README.md                   # This file
```

---

## ✅ Key Features

- **Single-sided printing** setup
- **Proper page margins** (toggle `showframe` to check layout)
- **Captions** formatted with bold labels
- **Automatic title, abstract, approval pages** using BU conventions
- **Appendix and symbols support**
- **Curriculum Vitae** section at the end
- **APA-style bibliography** with URLs and access dates

---

## 📄 How to Compile

This template is designed to be compiled with **PDFLaTeX** or **XeLaTeX** in Overleaf or locally.

```bash
pdflatex Thesis.tex
bibtex Thesis.aux
pdflatex Thesis.tex
pdflatex Thesis.tex
```

---

## ✏️ Customization

### Title, Author, and Degree Info
Update these commands in `Thesis.tex`:

```latex
\title{Your Dissertation Title}
\author{Your Name}
\degree=2  % 2 = PhD, 4 = Prospectus
\prevdegrees{BA ..., MA ...}
\department{Department of Biostatistics}
\faculty{Graduate School of Arts and Sciences}
```

### Readers and Major Professor
Specify each reader’s name, degree(s), and title:

```latex
\reader{First}{Name, Degree(s)}{Title}
```

### Chapters and Sections
Add or remove chapters by modifying the following:

```latex
\include{chapters/chapter1}
```

Place your LaTeX content in the corresponding `chapters/*.tex` files.

---

## 📚 References

- Place all `.bib` references in `Thesis.bib`
- Use APA format: `\bibliographystyle{apa-good}`

---

## 📘 List of Symbols

Fill out `chapters/Symbols.tex` with symbols or abbreviations used.

---

## 📝 Curriculum Vitae

Fill in the final section of `Thesis.tex` with your academic training, publications, and dissertation details.

---

## 🧠 Tips

- Use `\graphicspath{{figures/}{tables/}}` to manage media
- Use `\allowdisplaybreaks` for math-heavy chapters
- Use `\nocite{}` for including references not directly cited

---

## 🛠 Dependencies

- `bu_math_thesis.sty` — included in repo
- APA bibliography style: `apa-good.bst`
- Standard LaTeX packages (`caption`, `graphicx`, etc.)

---

## 👤 Acknowledgments

The BU-specific LaTeX style (bu_math_thesis.sty) is adapted from an MIT style file by Stephen Gildea, modified for BU by Paolo Gaudiano, Jonathan Polimeni, Janusz Konrad, Cameron Morland, Karen Yeats, and most recently updated by Hanna Gerlovin in 2018.

---

## 📜 License

This template is provided under the MIT License. Please modify it as needed for your institution.
