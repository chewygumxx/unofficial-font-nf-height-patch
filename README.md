# Nerd Font Height Patch

> You may be searching for the esteemed Nerd Font Repository: 
> **[ryanoasis/nerd-fonts][Nerd Fonts]**

If you've found this repository and are seeking the utility for patching
regular font files to produce new amalgamated files composed of the original
input font plus the additional spectacular glyphs of Nerd Font compilation
fame, please consult the [font-patcher][] section of the official Nerd Font
README.

> [!NOTE]
> I am neither contributer nor sanctioned associate of the renowned
> [Nerd Fonts][] project.

## Abstract

This repository provides a python script for uniform height manipulation of
font glyph bounding boxes. The script is speciali sed for Nerd Font patched
files for fine-tuned height adjustment performed distortion-free upon most
glyphs. TUI rendering glyphs ***are*** vertically interpolated to address
hairline breaks of box drawing, specified per the Unicode ranges below:

```python3
# Lines 67 to 72
ranges = [(0x2500,0x257F),   # Box Drawing
          (0x2580,0x259F),   # Block Elements
          (0x2800,0x28FF),   # Braille Patterns
          (0xE0A0,0xE0D7),   # Powerline
          (0x1FB00,0x1FBFF), # Legacy Computing Block
         ]

```

[Nerd Fonts]: <https://github.com/ryanoasis/nerd-fonts/tree/master>
[font-patcher]: <https://github.com/ryanoasis/nerd-fonts#font-patcher>
['Anonymice Pro Nerd Font']: <https://github.com/ryanoasis/nerd-fonts/tree/master/patched-fonts/AnonymousPro>

## Dependencies

- python3
- python-fonttools

## Problem: Anonymous Pro + Nerd Fonts 

I've adored the Anonymous Pro font for 10 years. It's clean, it's familiar,
it's the typeface I best harmonise and consider aesthetically quintessential.

Nerd Fonts are not new. They've been communally embraced and adopted as
terminal necessity for many welcome years. Recently however, I accidentally
misconfigured my font precedence, elevated `Anonymice Pro Nerd Font` above
`Anonymous Pro`, and [compromised my reading experience][gh-squeeze-issue].
The effect was so subtle, I had not realised until my rate of reading
exhaustion was apparent.

[gh-squeeze-issue]: <https://github.com/ryanoasis/nerd-fonts/issues/850>

There are many ephemerally efficacious fixes for line height congestion. The
most efficient involving compulsion of the system to surrender to the symptom,
to increase line height style values for every application can bend, until the
temporary fix becomes permanent solution and any unfeasible to feign fealty for
the font so fickle, farewelled and forbidden from this Leaning Limping Letter
Leper Village.

## The Provided 'Solution'

The `font-patch-height-nf-unofficial` script does not manipulate the dedicated 
line height properties of tables `head`, `hhea`, `OS/2`, nor any other. The 
projected line height of any provided file is resolved exclusively from the 
difference between `hhea.ascent` and `hhea.descent`.


`------=====------ I'll finish this later, the script works. ------=====------`

`------=====----- Please exercise care, I may have been lucky ------=====------`
