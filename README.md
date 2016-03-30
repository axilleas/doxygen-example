# doxygen-example
A silly C  program example to demonstrate doxygen

## Requirements
- Doxygen
- GraphViz (dot) [optionally]
- make [on *nix]

If generating PDFs:
- PDF-LaTeX (I use MikTex). This may ask for permission, and install sub packages 
during a make operation
- Ghostscript

## Generate documentation
- To generate doxygen documentation run:

```
doxygen ./doxygen/Doxyfile
```
Generate HTML will be located in the location specified by the Doxyfile, in this 
case `./doxygen/documentation/html`.

- If also generating a PDF, an extra step is required:
    - On Windows:

    ```
    > ./doxygen/documentation/latex/make.bat
    ```

    - On *nix:
    ```
    $ make all -C ./doxygen/documentation/latex/
    ```
The resulting PDF is named refman.pdf and is placed in the latex directory.
