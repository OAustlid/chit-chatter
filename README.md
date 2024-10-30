# pecha-kucha

Simple tool for creating a Pecha Kucha presentation

## How-to

To use this tool:
- Clone the repo
- Create 20 slides, and export them as png, jpg or webp files (or any other img-type file).
- Put them in the main folder. (the slides will be .gitignored, apart from the "empty.png" placeholder).
- Edit the presentation (using f.ex VS Code or something similar) wrt. the <img> elements: set the src of each element to point to a slide.
  - If setting `randomize_slides_sequence = true`, the order is not important, as it will be scrambled at presentation time.
- Launch the start.html ahead of your presentation. To start it just click on the link and it will start.

You have 20 seconds (configurable) for each slide.

When there are a few seconds left for a slide, a timer will be displayed in the top left corner.

(Optional) You may set the <img> element with class "final" to a slide that will always be the ending of the presentation. That slide will not have a timeout, nor show a timer.
