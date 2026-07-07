# Osc-brand Extension For Quarto

This\ extension is intended to be applied to our Quarto projects where we want to apply consistent LMU Open Science Center styling, images, and branding. This extension thus makes use of Quarto's developing `_brand.yml` feature with LMU colors, OSC logos, and some custom typography. The presets in this `_brand.yml` file are then principally applied to any type of Quarto output where the fields are applicable or usable.

Moreover, at the time of initial creation, there is also a custom HTML format available via this extension. This should be applied to essentially all of our websites, and can be done like so:

```{.markdown filename="_quarto.yml"}
project:
  type: website

format: osc-brand-html

# or, if specifying more fields
# format:
#   osc-brand-html:
#      ...further specs here
```


## Installing

```bash
quarto add lmu-osc/osc-brand
quarto add lmu-osc/osc-tutorial
```

This will install the extensions under the `_extensions` subdirectory.
If you're using version control, you will want to check in this directory.

**Yes, these are two separate extensions in one repo! The osc-tutorial extension, however, depends on the osc-brand extension and they must be installed together if you want to use the `osc-tutorial-html` format. The osc-brand extension, however, is independent of the other extension.**

## Using

This extension installs a [brand.yml](https://posit-dev.github.io/brand-yml/) configuration.

## Example

Here is the source code for a minimal example: [example.qmd](example.qmd). To see it in action, clone this repo and preview:

```bash
git clone git@github.com:lmu-osc/osc-brand.git
cd osc-brand
quarto preview
```


*The LMU OSC logos are trademarks and are not granted under this license — they may only be used in accordance with LMU brand guidelines.*