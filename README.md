# 🇺🇸 Markdown to PDF Resume  

This repository contains my resume written in Markdown, available in both Portuguese and English

## Automatic PDF Generation

Every time a change is pushed to the `main` branch, a GitHub Action generates the PDF version of the resume from the `en_resume.md` file. For the Portuguese version, use the `pt_resume.md` file.

The process uses Pandoc and TinyTeX to convert the `.md` file into a `.pdf`. The final file is available for download in the repository's "Actions" tab as a build artifact.

## How to Generate the PDF Locally

To generate the PDF locally, you must have Pandoc and a LaTeX distribution (like TinyTeX, MiKTeX, or TeX Live) installed.

Then, run in your terminal:

**For the Portuguese version:**

```bash
pandoc pt_resume.md -o resume_pt.pdf --pdf-engine=xelatex -V geometry:"top=2cm, bottom=2cm, left=2cm, right=2cm" -V mainfont="Arial"
```  

**For the English version:**

```bash
pandoc en_resume.md -o resume_en.pdf --pdf-engine=xelatex -V geometry:"top=2cm, bottom=2cm, left=2cm, right=2cm" -V mainfont="Arial"
```
---

# 🇧🇷 Currículo Markdown para PDF

Este repositório contém meu currículo escrito em Markdown, disponível tanto em português quanto em inglês.

## Geração Automática do PDF

Toda vez que uma alteração é enviada para a branch `main`, uma Action do GitHub gera a versão em PDF do currículo a partir do arquivo `en_resume.md`. Para a versão em portugês, utilizar o arquivo `pt_resume.md`

O processo utiliza Pandoc e TinyTeX para converter o arquivo `.md` em `.pdf`. O arquivo final fica disponível para download na aba "Actions" do repositório como um artefato da build.

## Como Gerar o PDF Localmente

Para gerar o PDF localmente, é preciso ter o Pandoc e uma distribuição LaTeX (como TinyTeX, MiKTeX ou TeX Live) instalados. 

Depois, execute no seu terminal:

**Para a versão em português:**

```bash
pandoc pt_resume.md -o resume_pt.pdf --pdf-engine=xelatex -V geometry:"top=2cm, bottom=2cm, left=2cm, right=2cm" -V mainfont="Arial"
```  

**Para a versão em inglês:**

```bash
pandoc en_resume.md -o resume_en.pdf --pdf-engine=xelatex -V geometry:"top=2cm, bottom=2cm, left=2cm, right=2cm" -V mainfont="Arial"
```
---
