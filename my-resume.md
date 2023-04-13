# My Resume

This repository contains the source code for my resume, which is written in Markdown format and converted to PDF using GitHub Actions.

[![Convert resume to PDF](https://github.com/onurravli/my-resume/actions/workflows/convert-to-pdf.yaml/badge.svg)](https://github.com/onurravli/my-resume/actions/workflows/convert-to-pdf.yaml)

## Usage

To generate a PDF version of the resume, simply push any changes to the `my-resume.md` file to the `main` branch of this repository. The GitHub Actions workflow will automatically convert the Markdown file to PDF and store it as an artifact, which you can download from the Actions tab.

Additionally, the workflow will move the generated PDF file to the `output` folder in the root directory of the repository. You can use this folder to store multiple versions of the resume, or to make it available for download via your website or other channels.

## Dependencies

This GitHub Actions workflow relies on the following dependencies:

-   `pandoc`: A document converter that can convert files from one format to another. Used to convert Markdown to PDF.
-   `texlive-xetex`: A TeX distribution that includes the XeTeX engine, which is used by `pandoc` to generate PDFs with custom fonts and styles.

These dependencies are installed automatically by the GitHub Actions runner, but are also cached to improve workflow performance.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.
