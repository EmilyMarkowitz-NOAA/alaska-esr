# NOAA Fisheries Alaska Ecosystem Status Reporrt

**This is a template repo to create report with a NOAA tech memo format in pdf, html, or docx format.**

> This code is always in development. Find code used for various report in the code [releases](https://github.com/afsc-gap-products/gap_products/releases).

*This code is primarily maintained by:*

**Emily Markowitz** (Emily.Markowitz AT noaa.gov;
[@EmilyMarkowitz-NOAA](https://github.com/EmilyMarkowitz-NOAA))

**Bridget Ferriss** (Bridget.Ferriss AT noaa.gov;
[@BridgetFerriss](https://github.com/BridgetFerriss))

Alaska Fisheries Science Center,

National Marine Fisheries Service,

National Oceanic and Atmospheric Administration,

Seattle, WA 98195

## Run notes

### R package dependencies

The package dependencies are defined in the DESCRIPTION file. You can check if you have all the required dependencies and install if necessary, via 
```
devtools::install_deps()
```
You run this from the base level, i.e. your working directory is where the DESCRIPTION file is. Install the {devtools} package first if you don't have it installed.

As you work on your project, add any packages your documents require to the DESCRIPTION file. That way users can quickly install dependencies. A easy way to analyze your project code and find any dependencies is using the {renv} package. You don't need to use {renv}; you can just use it's utility for analyzing all your code. It starts at the base directory and works downward.
```
renv::dependencies()
```

### Removing the coverpage

Go into `_frontmatter.yml` and change `coverpage: true` to `coverpage: false`.

### Changing the PDF

All the PDF specs are in `_frontmatter.yml`. See [Quarto Titlepages documentation](https://nmfs-opensci.github.io/quarto_titlepages/) for instructions on how to customize the coverpage and the titlepage.

<hr>

## NOAA README

This repository is a scientific product and is not official
communication of the National Oceanic and Atmospheric Administration, or
the United States Department of Commerce. All NOAA GitHub project code
is provided on an ‘as is’ basis and the user assumes responsibility for
its use. Any claims against the Department of Commerce or Department of
Commerce bureaus stemming from the use of this GitHub project will be
governed by all applicable Federal law. Any reference to specific
commercial products, processes, or services by service mark, trademark,
manufacturer, or otherwise, does not constitute or imply their
endorsement, recommendation or favoring by the Department of Commerce.
The Department of Commerce seal and logo, or the seal and logo of a DOC
bureau, shall not be used in any manner to imply endorsement of any
commercial product or activity by DOC or the United States Government.

## NOAA License

Software code created by U.S. Government employees is not subject to
copyright in the United States (17 U.S.C. §105). The United
States/Department of Commerce reserve all rights to seek and obtain
copyright protection in countries other than the United States for
Software authored in its entirety by the Department of Commerce. To this
end, the Department of Commerce hereby grants to Recipient a
royalty-free, nonexclusive license to use, copy, and create derivative
works of the Software outside of the United States.

<img src="https://raw.githubusercontent.com/nmfs-general-modeling-tools/nmfspalette/main/man/figures/noaa-fisheries-rgb-2line-horizontal-small.png" alt="NOAA Fisheries" height="75"/>
