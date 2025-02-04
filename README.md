# FootNotes

## Overview

This repository is designed to automate the process of formatting citations for academic or legal publications. The automation extracts footnotes from a source document, parses multiple citations within each footnote, and generates a formatted Master Code document where each citation receives its own numbered page corresponding to the footnote number and order within the footnote.

## File Structure

**source_article.docx:** The document containing footnotes with citations.

**DPF_Master_Code.docx:** The template where formatted citations are inserted.

**script.py:** A script to automate the extraction and formatting process.

**README.md:** This document.

## Formatting Rules

Each footnote number corresponds to the footnote in the source document.

If a footnote contains multiple citations, they are separated into distinct entries labeled as X.1, X.2, X.3, etc., where X is the footnote number.

Each citation gets its own dedicated page in DPF_Master_Code.docx.

## Example

Footnote from **source_article.docx:**

```Bonnie Langston, Food fight: Some local farms prefer “Naturally Grown” over “Organic,” INSTITUTE FOR AGRICULTURE & TRADE POLICY (2007); Lisa Hill, The Rise of ‘Certified Naturally Grown’…and how it’s shaping the way we eat, CERTIFIED NATURALLY ORGANIC (May 16, 2022), https://www.naturallygrown.org/the-rise-of-certified-naturally-grown-and-how-its-shaping-the-way-we-eat/.```

Transformed in **DPF_Master_Code.docx:**

Page 1 (7.1):

```Bonnie Langston, Food fight: Some local farms prefer “Naturally Grown” over “Organic,” INSTITUTE FOR AGRICULTURE & TRADE POLICY (2007).```

Page 2 (7.2):

```Lisa Hill, The Rise of ‘Certified Naturally Grown’…and how it’s shaping the way we eat, CERTIFIED NATURALLY ORGANIC (May 16, 2022), https://www.naturallygrown.org/the-rise-of-certified-naturally-grown-and-how-its-shaping-the-way-we-eat/.```

## Usage

Place the source document (source_article.docx) in the repository folder.

Run **script.py** to extract and format citations.

The **DPF_Master_Code.docx** will be updated with properly formatted citations.

## Dependencies

N/A

## Future Improvements

Implement error handling for malformed citations.

Add support for additional citation styles.

Develop a GUI for easier interaction.

<hr>

For any questions or contributions, please open an issue or submit a pull request.
