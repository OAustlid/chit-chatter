# pecha-kucha

Simple tool for creating a Pecha Kucha presentation

## How-to

To use this tool:

1) Clone the repo
1) Create 20 slides, and export or save them as png, jpg or webp files (or any other image-type file that is supported by your choice of browser).
1) Put the slides in the main folder. The `.gitignore` makes sure you don't accidentally share them.
1) Edit the `presentation.html` (using f.ex VS Code or something similar) wrt. the `<img>` elements. Set the `src` of each element to point to a slide.
1) Launch the start.html ahead of your presentation. To start it just click on the link and it will start.
1) *For extra effect, most browsers can be put in fullscreen mode. Consider doing this before clicking "start".*
1) In the `script` part there are a couple of settings:
 - `randomize_slides_sequence` set to `true` will randomize the sequence of the slides every time you run it, while `false` will preserve the order of the `<img>` elements.
 - `millis_per_slide` should stay at `20000` for a Pecha Kucha, but if you want you can change it.
 - `tick_is_active` is the small red visual indicator in the top left corner when slides are soon to change. Set to `false` to disable it.
 - `countdowntick` can be set to a number of seconds if you like a couple of seconds before the first slide appears.
 - `millis_per_tick` is just how long between checking for updates like a new slide or altering the ticks indicator. Any value between 10 and 100 should work just fine.


You have 20 seconds (configurable) for each slide.

When there are a few seconds left for a slide, a timer will be displayed in the top left corner.

(Optional) You may set the <img> element with class "final" to a slide that will always be the ending of the presentation. That slide will not have a timeout, nor show a timer.
