# Arabic Trace Studio

This standalone tool will be hosted at `https://moenegm.github.io/arabic-trace-studio/` after its repository's GitHub Pages workflow is enabled and deployed. You can also open `index.html` directly in a modern browser. No installation or network connection is needed.

Paste one label per line, press **Set list**, then draw each item on the square canvas. Each pen-down and pen-up is kept as a separate stroke in the order you made it. Use **Place dot** for dots or other point marks; these are also stored in order. Apple Pencil, finger, and mouse input use browser pointer events.

The tool records normalized coordinates from 0 to 1 with the origin at the top left. It does not smooth, simplify, reorder, or otherwise reshape points. Grid and direction arrows are display aids only. Work autosaves in the current browser profile; download the project JSON regularly to keep a portable backup. Reopen that JSON with **Open saved project JSON** to continue later.

**Download Swift paths** exports every labeled item and its marks in order. That file is a coordinate data export; adapting its type names to the app's current trace model may be needed before dropping it into Xcode. This tool does not modify the app's existing trace paths.
