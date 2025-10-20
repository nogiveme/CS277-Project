## Project Structure Documentation

This project follows a modular organization for collaborative LaTeX document writing:

### Directory Organization

- **`sections/`**: Contains individual `.tex` files, with each file representing a separate section of the document. Contributors should write content by creating or editing section files in this directory.

- **`main.tex`**: The main LaTeX file that uses `\input{}` commands to include all section files from the `sections/` folder. This file orchestrates the document structure.

- **`build/`**: Stores all compilation outputs and intermediate files generated during the LaTeX build process. This directory should not be edited manually.

- **`assets/`**: Houses all resources such as figures, images, tables, and other media files referenced in the document.

- **`reference.bib`**: Contains all BibTeX entries for bibliographic references used throughout the document.

### Workflow for Contributors

1. Create or edit `.tex` files in the `sections/` directory for your assigned section
2. Add the section to `main.tex` using `\input{sections/your-section}`
3. Place any images or tables in the `assets/` directory
4. Add citations to `reference.bib` in BibTeX format
5. Compile from `main.tex` - outputs will appear in `build/`