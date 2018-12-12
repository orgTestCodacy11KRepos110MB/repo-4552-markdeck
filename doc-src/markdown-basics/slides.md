---
title: markdeck - markdown basics
highlight_style: github-gist
# pdf: markdeck-scaffold.pdf
# slideNumber: true
controls: true
controlsTutorial: true
controlsLayout: edges
---


# markdeck - the markdown basics {bgcss=sea-gradient .light-on-dark}

| &nbsp;

<small>
to proceed to the next slide,</br>
press 'space' or 'cursor right'
</small>


# self-documenting slides {bg=#123456 .light-on-dark}

That means,
you can see
the rendered result on the left

and
the markdown source on the right side.


```render_a2s
#------------------#------------#
|                  :            |
|     rendered     |   slide    |
|      slide       |   source   |
|                  |            |
|                  |            |
|                  |            |
#------------------#------------#
```


# source files

all files matching `slide*.md` are considered source files

and get rendered on change, ordered by name


# meta data

every slide deck needs a set of meta data to begin with

so start your slides with something like this:

    ---
    title: my slide deck title
    ---

You can find all valid parameters in the console output of the markdeck container,
in the ```config``` section.


# meta data

As per v0.33, these parameters are:

    -------- config --------
    {
      "controls": true,
      "autoSlideMethod": "Reveal.navigateNext",
      "variant": "reveal",
      "autoPlayMedia": "null",
      "shuffle": false,
      "transition": "slide",
      "hideAddressBar": true,
      "rtl": false,
      "history": true,
      "progress": true,
      "highlight_style": "github-gist",
      "transitionSpeed": "default",
      "pdf_size": "1189x841",
      "pdf_delay": "100",
      "center": true,
      "overview": true,
      "asciinema": false,
      "embedded": false,
      "help": true,
      "previewLinks": false,
      "backgroundTransition": "fade",
      "slideNumber": false,
      "loop": false,
      "mouseWheel": false,
      "autoSlideStoppable": true,
      "pdf": "",
      "keyboard": true,
      "touch": true,
      "standalone": "",
      "html": "index.html",
      "controlsBackArrows": "faded",
      "controlsTutorial": false,
      "showNotes": false,
      "autoSlide": "0",
      "title": "markdeck basics",
      "fragments": true,
      "defaultTiming": "120",
      "controlsLayout": "bottom-right",
      "theme": "simple"
    }
    ASCIIART_CONFIG=/markdeck/lib/render-asciiart-filter.config
    -------- /config --------


# a new slide

To begin a slide, add a section by starting
a new line with `#`

The content gets centered and scaled appropriately.


# 

In case you don't need a headline:
empty headlines are allowed, too


# markdown

Normal text renders as normal text.<small>tadahh</small>

Single
newlines
get
removed, so you can wrap
your text
whereever
you want.

To start a new paragraph,
insert an empty line.


TODO link to markdown, pandoc


# basic markup

TODO link to markdown doc

* list item a
* list item b

_emphasized text_

1. ordered list
1. ordered list


# code

TODO


# links

internal, external, images


# eye candy

unicode: ♥

emojis: 😎

font-awesome: ![](fab fa-github)

images: ![](assets/buddy-egyptian.svg)

TODO: add links to docs/lists/8081 pages


# raw html

if in dire need, add raw html
<small>like this</small>


# next steps

TODO