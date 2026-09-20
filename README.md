# L-Size Photo Sizer

Crops photos to the exact printed frame for a **Canon SELPHY CP1500** on L-size
paper (119 × 89 mm), and renders a print-resolution JPEG at 400 dpi
(1874 × 1402 px per sheet).

**Live: https://joymanubag21.github.io/photo-sizer/**

Three formats, built to real paper geometry in millimetres:

| Format | Layout | Printer setting |
| --- | --- | --- |
| Memory Lane story card | two 54 × 56 mm frames, 0.1 in gap, caption band below | L Borderless · Landscape · **Fill Entire Paper** · 100% |
| Instax mini guest card | two 54 × 86 mm cards per sheet, 46 × 62 mm window, cut hairlines | L Borderless · **Print Entire Image** · 100%, then cut |
| Full L-size photo | edge to edge, no card, no text | L Borderless · Landscape · **Fill Entire Paper** · 100% |

Everything runs in the browser. No upload, no backend, no build step — the whole
app is one self-contained `index.html`. Photos never leave the device.

The resolution warning is computed live from the source pixels actually fed into
a frame at the current zoom, not from the file's dimensions, so zooming past what
a photo can carry flags it and names the pixel count you need.
