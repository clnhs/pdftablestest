# Test-implementing PDF table recognition and extraction of data

Based on https://nanonets.com/blog/table-extraction-deep-learning/

Also see https://nanonets.com/blog/ocr-with-tesseract/

## How to use
Note: you can simply preview the notebook in GitHub by clicking on the "pdftablestest.ipynb" file.

### Create a new conda environment
Create a new environment using the "environment.yaml" file.

Open a terminal inside the project folder, then use the following command:
`conda env create -f environment.yml`.
   - This will create a new environment in which to run this project so it doesn't touch other environments/projects you already have on your computer. 
   - The required packages will be automatically installed in this environment.

### Run the notebook with jupyter lab
Note: Use the aforementioned conda environment — create it first if needed.

1. Activate the new environment, use the following command: `conda activate pdftablestest` (it's a very original name, I know).
2. Run `jupyter lab`.
3. Navigate to project folder, then open the "pdftablestest.ipynb" file.
4. Run all cells.

### Using with VS Code
Note: Use the aforementioned conda environment — create it first if needed.

1. Open the project folder in VS Code.
2. Make sure to select the proper python interpreter
    - Open the command palette (<kbd>CTRL</kbd>+<kbd>SHIFT</kbd>+<kbd>P</kbd>) then type "python select interpreter".
    - Select the one that says something like `'pdftablestest': conda`.
3. Open the "pdftablestest.ipynb" file.
4. You might need to tell it to trust the file before it opens it.
5. Click the "Run all cells" button (looks like the "forward" button on a remote control).

## Stuff this project uses
- pdf2image for converting PDF pages to images (once I implement it; should be trivial)
- OpenCV for finding blocks on the page (and possibly more, I don't know yet)
- Numpy because numbers, and probably pandas along the way.
- Tesseract for OCR (once I implement it)

## To-do
- [x] Find borders
- [ ] Use actual PDF file as input
- [ ] Convert input PDF file to pictures
- [ ] Grouping
- [ ] Find a way to identify tables without relying on their drawn borders
- [ ] Find irregular tables (like the invoice example's main table)

## Obligatory cat
![Yay](https://media1.tenor.com/images/b1568040b7983be6c7f8bce94caf8f21/tenor.gif?itemid=11797622)
