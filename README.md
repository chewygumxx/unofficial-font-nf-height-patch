# Nerd Font Height Patch \[Unofficial]

> [!NOTE]
> I am neither a contributer nor sanctioned associate of the renowned
> [Nerd Font][] project.
> 
> Apparently some repository names are reserved :)

## Directions to [Nerd Fonts][]

The esteemed Nerd Font Repository awarded :star: *>63k Stars* :star:: 
**[ryanoasis/nerd-fonts][Nerd Fonts]**

If you've found this repository and are seeking the utility for patching
regular font files to produce new amalgamated files composed of the original
input font plus the additional spectacular glyphs of Nerd Font compilation
fame, please consult the [font-patcher][] section of the official Nerd Font
README.

[Nerd Fonts]: <https://github.com/ryanoasis/nerd-fonts/tree/master>
[font-patcher]: <https://github.com/ryanoasis/nerd-fonts#font-patcher>.
['Anonymice Pro Nerd Font']: <https://github.com/ryanoasis/nerd-fonts/tree/master/patched-fonts/AnonymousPro>

## Problem: Anonymous Pro + Nerd Fonts 

I've adored the Anonymous Pro font for the last 10 years. It's clean, it's 
familiar, it's the typeface of I best harmonise and consider aesthetically
quintessential.

Nerd Fonts are not new. They've been communally embraced and adopted as
terminal necessity for many welcome years. Recently however, I accidentally
misconfigured my font precedence, elevated `Anonymice Pro Nerd Font` above
`Anonymous Pro` standard, and [compromised my reading
experience][gh-squeeze-issue]. The effect was so subtle, I could not tell it
had happened until my rate of reading exhaustion followed a pattern.

[gh-squeeze-issue]: <https://github.com/ryanoasis/nerd-fonts/issues/850>

There are many proposed, ephemerally efficacious fixes for glyph line_height
congestion. The easiest involve compromising the system to address the symptom,
to increase line_height within every application that allows, until the new
normal is status quo and whatever cannot compensate for a broken font is
forbidden from Limping Letter Land.

## The Tenuous Solution

The font-patch-heigh-nf-unofficial script does not manipulate the line height
of 'head', 'hhea','OS/2',

The 
script involved more glyph study than my working memory permit.

The aforementioned lassitude trap is one I sympathise given this python
involves more line-reading than script-play performance. It's executed without
issue, produces  the few orms without needlessly difficult compared to increasing line_height. The final straw was
needlessly difficult compared to increasing line_height. The final straw was
