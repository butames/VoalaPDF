# VoalaPDF

I am creating this Quarto extension to serve as a template to generate a PDF with (pretty) styling using LaTeX. Use `PrettyPDF-pdf` as the format if using LaTeX.

## Installation and use

To install the Quarto extension, create a directory, and use the template file:

``` bash
quarto use template sbutame/VoalaPDF
```

To use the extension in an existing project without installing the template file:

``` bash
quarto install extension sbutame/VoalaPDF
```
Note that you will need to update the output format to `format: PrettyPDF-pdf` to enable use of the extension. For book projects, add:

```
project:
  type: PrettyPDF
```
to the `_quarto.yml` file.

## Adjusting LaTeX Styling

If you want to update the LaTeX version of this template to use a different colour or logo, open up the `_extensions/nrennie/PrettyPDF/PrettyPDF.tex` file after you have installed the extension.

### Logo

Either replace the `logo.png` file with a new file of your choosing, or change the file path on line 28 to point to a different logo file. Note that the file path is relative to your .qmd file.

### Colours

Lines 14-16 define three colours used in the template: `light`, `dark`, and `highlight`. Change the hex colours in these lines to update the colours. The `light` colour changes the sidebar and code block background colours. The `dark` colour changes the text. The `highlight` colour changes the link colours.

## Reference/Source

Read more about this extension, how it was built, and how to make your own in my blog post at [nrennie.rbind.io/blog/making-pretty-pdf-quarto](https://nrennie.rbind.io/blog/making-pretty-pdf-quarto/).

