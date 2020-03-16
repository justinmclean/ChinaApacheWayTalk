
# ASF and the Apache Way

An overview of the ASF foundation and how it operates under the Apache Way.

## Technology Used

The slides are generated from [asciidoctor](https://asciidoctor.org) markup and displayed with [reveal.js](https://asciidoctor.org/docs/asciidoctor-revealjs/). This means the content can be kept under version control and exported to a number of formats other than HTML.

Please check out the examples of [asciidoctor-revealjs](https://asciidoctor.org/docs/asciidoctor-revealjs/#syntax-examples) for more information about using markdown with reveal.js.

## How to Build

To install the needed dependencies on OSX run:

`install-deps.sh`

Then run:

`mvn clean compile`

## How to Update the ASF Statistics

To update the ASF statistics (no of podlings, no of committers etc. etc.) run:

`cd src/main`
`python3 stats.py > asciidoc/projectstats.adoc`

## How to View the Slides

Once built, the generated slides can be found at:

`target/generated-slides/index_en.html`
`target/generated-slides/index_cn.html`

Just open the `index_en.html` or `index_cn.html` in a browser to view the slides.

Some features require the slides to be viewed via a http/https url you can do this by running:

`mvn jetty:run-exploded`

And goto `http://127.0.0.1:8080/index_en.html` or `http://127.0.0.1:8080/index_cn.html`in a browser to view.

How to print pdf:
please access "http://127.0.0.1:8080/index_en.html?print-pdf” in a browser and print the page with landscape layout.

Some key shortcuts that may help you give a presentation:

- Cursor keys and space can navigate the slides.
- Press S will show speaker notes and a timer in a separate window.
- Press F for full screen.
- Press N for next slide or P for previous slide.
- Press O (for overview) will show a slide map / overview.
- Press B will black the screen.
