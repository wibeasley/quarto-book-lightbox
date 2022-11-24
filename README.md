# quarto-book-lightbox

This minimal example is to help me troubleshoot a problem encountered with the [*Guide to N3C*](https://github.com/National-COVID-Cohort-Collaborative/guide-to-n3c-v1)

The current error is
```
GET: /lightbox.html
Error running filter _extensions/quarto-ext/lightbox/lightbox.lua:
_extensions/quarto-ext/lightbox/lightbox.lua:113: attempt to call a nil value (field 'is_format')
stack traceback:
```

(There is nothing listed after "stack traceback".)

I've tried to replicate the "Simple Lightbox Example" at <https://github.com/quarto-ext/lightbox>.

I get this error when I try to render:

* the book's [lightbox.qmd](lightbox.qmd) through VS Code (using `quarto preview`, and several variations)
* the stand-alone [not-in-the-book.qmd](not-in-the-book.qmd) through VS Code (using `quarto preview`, and several variations)
* the book's [lightbox.qmd](lightbox.qmd) through RStudio (using the "Render button)
* the stand-alone [not-in-the-book.qmd](not-in-the-book.qmd) through RStudio (using the "Render button)


# Resolution:

Upgrade to the newest version of Quarto.  The version from a week or two ago apparently didn't correspond with the Lightbox extension

https://stackoverflow.com/a/74565982/1082435
