---
layout: page  
title: Abg Font Thumbnails  
description: This tutorial will show you how to change the Abg text on font thumbnails using Fontforge.  
image: /assets/images/thumbnail/0-how-to-change-abg-font-thumbnail.png
nav_order: 1  
permalink: /abg-thumbnails/  
---

<center><img src="/assets/images/thumbnail/1-how-to-change-abg-font-thumbnail.png" alt="fix-abg-letters-thumbnails-before-and-after" width="35%" height="35%"/></center>  

# HOW TO CHANGE THE Abg TEXT ON FONT THUMBNAILS USING FONTFORGE  

**This tutorial will show you how to change the Abg text on font thumbnails using Fontforge.**  

  <img src="/assets/images/thumbnail/2-how-to-fix-abg-font-thumbnails.png" alt="how-to-fix-abg-font-thumbnails-before-and-after" width="30%" height="30%"/>  

## How this Tutorial is Organized  
{: .no_toc }

1. We’ll start with opening the font.  
2. Then we’ll change the encoding settings.  
3. Next, we’ll specify the character page settings so an English Abg will display on your thumbnail.  
4. And lastly, I’ll show you how to generate your updated font and briefly outline the settings required to do this.  

>  i. You can download Fontforge for Windows, Mac, or Linux from [here](https://fontforge.org/en-US/downloads/).  
>  ii. The font used in this tutorial is called [Lovers Quarrel](https://www.fontsquirrel.com/fonts/lovers-quarrel). It’s a free font for personal and commercial use with an open source license.  
>  iii. This tutorial is shown on a Windows 10 computer with Fontforge version 03142020.  
>  iv. Fontforge does crash, so save often.  

---

## Opening A Font  

5. We’ll begin this tutorial by selecting a font and opening it in Fontforge.  

6. The first screen to pop up in Fontforge will be the ‘Open Font’ dialogue box where you can navigate and select your font file, using either,  
a) The ‘arrow’ button (1),  
b) the ‘dropdown’ bar (2), or  
c) typing into the address bar (3).  
    <img src="/assets/images/thumbnail/3-how-to-open-fontforge.png" alt="how-to-open-fontforge" width="40%" height="40%"/>  

7. Once located and selected, click ‘OK’.  
    <img src="/assets/images/thumbnail/4-how-to-use-fontforge.png" alt="how-to-use-fontforge" width="40%" height="40%"/>  

8. Ignore error or warning dialogue boxes that may pop up.  
    <img src="/assets/images/thumbnail/5-fontforge-warning.png" alt="opening-fontforge-warning-pop-up" width="50%" height="50%"/>  

9. After clicking ‘OK’, Fontforge will open your font where you’ll see each glyph has its own cell. This screen or interface is called ‘Font View’. In the next step I’ll show you how to change the encoding settings from ‘Font View’.  
    <img src="/assets/images/thumbnail/6-change-abg-font-thumbnail.png" alt="font-view-fontforge-abg-thumbnails" width="70%" height="70%"/>  

---

## Encoding Settings

10. Next we’ll change the font's encoding settings. To do this,  
a) click on ‘Encoding>Reencode’  
b) then click on your preferred Unicode format.  
c) In this tutorial we’ll be selecting ‘ISO 10646-1 (Unicode, Full)’ because it’s a large set of all the other Unicode formats, which guarantees no information or glyph is lost when re-encoding.  
    <img src="/assets/images/thumbnail/7-fix-abg-font-thumbnails.png" alt="fix-abg-thumbnail-reencode-font-settings" width="65%" height="65%"/>  

11. Further information on [encoding](https://fontforge.org/docs/ui/menus/encodingmenu.html) can be found in Fontforge documentation.  

---

## Character Settings

12. Now we need to change the character settings, because this defines the Abg thumbnail.  
a) What this means is, if character settings are set to display Mathematical Operators for Abg, then the thumbnail will show mathematical symbols that represent Abg, instead of an English Abg.  

    b) In other words, if you see Greek Abg instead of an English Abg, then the font’s character settings are set to ‘Greek and Coptic’.  

    c) Or Cyrillic Abg instead of an English Abg, then the character settings are set to ‘Cyrillic’.  
    <img src="/assets/images/thumbnail/8-how-to-change-abg-font-thumbnail.png" alt="example-wrong-abg-font-thumbnail" width="35%" height="35%"/>  

13. The below table provides a visual representation of what I've just described.  

	| Abg | Character Set |
	|:---:|---|
	| ∑√ ≠ | Mathematical Operators (Suppl. & Misc.) |
	| Aβγ | Greek and Coptic, 1253 Greek |
	| Абф | Cyrillic & Supplement, 1251 Cyrillic |  

14. Looking at the thumbnail for Lovers Quarrel, which displays one mathematical symbol and nothing else, we'll need to turn off the Mathematical Operator character settings, so that Abg will display on our thumbnail.  
    <img src="/assets/images/thumbnail/9-change-abg-font-thumbnail.png" alt="how-to-fix-abg-font-thumbnails-before-Lover's-Quarrel" width="20%" height="20%"/>  

15. To change the character settings, make sure you’re back in ‘Font View’ then,  
a) Click on ‘Element>Font Info’.  
    <img src="/assets/images/thumbnail/10-change-abg-font-thumbnail.png" alt="character-settings-for-changing-font-Abg-thumbnail" width="70%" height="70%"/>  

	### OS/2 Charsets  

16. On the next screen that pops up,  
a) you’ll need to select ‘OS/2’ in the left hand column,  
b) then click on the tab called ‘Charsets’ on the right.  
    <img src="/assets/images/thumbnail/11-how-to-fix-abg-font-thumbnails.png" alt="OS/2-character-settings-to-change-abg-font-thumbnail" width="70%" height="70%"/>  

	#### Unicode Ranges  

17. Next we’ll focus on the top box called ‘Unicode Ranges’, where you can see a number of lines are selected in blue.  
a) scroll down the 'Unicode Ranges' box and locate ‘Math Operators & Sup Math Operators’,  
b) then de-select this line by holding down Ctrl on the keyboard and left mouse click.  
or  
c) you can de-select everything by clicking on an unselected line or white area.  
d) then select ‘Basic Latin’ which is the first (1st) line, when you scroll back to the top.  
    <img src="/assets/images/thumbnail/12-how-to-change-abg-font-thumbnail.png" alt="unicode-ranges-maths-to-fix-Abg-font-thumbnail" width="70%" height="70%"/>  

	#### MS Code Pages  

18. Now we’ll scroll through the bottom box called ‘MS Code Pages’, to see if there are any unusual lines selected.  
a) You can de-select by holding down Ctrl on the keyboard and left mouse click.  
b) As Lovers Quarrel is a Latin font, anything unusual would be anything other than Latin.  

19. When scrolling through this box for Lovers Quarrel, it looks normal with only 2 lines and therefore we will not de-select anything.  
a) 1252, Latin-1 and  
b) Mac Roman.  

20. When you’ve finished,  
a) Click ‘OK’ to save your changes and we'll be taken back to ‘Font View’.  
    <img src="/assets/images/thumbnail/13-change-abg-font-thumbnail.png" alt="code-pages-settings-to-change-abg-font-thumbnail" width="70%" height="70%"/>  

---

## Generating Your Font  

21. We are now ready to generate our updated font.  
a) Click on ‘File>Generate Fonts’.  
    <img src="/assets/images/thumbnail/14-fontforge-generate.png" alt="generating-your-font-settings-for-changing-font-Abg-thumbnail" width="60%" height="60%"/>  

22. The next dialogue box that pops up is called ‘Generate Fonts’ where we’ll make changes by,  
a) re-naming our font or changing the folder we're saving to, making sure we don’t save over the top of our original font, then  
b) Untick ‘Validate Before Saving’, then  
c) Make sure ‘No Bitmap Fonts’ and ‘No Rename’ are displayed in the dropdown boxes.  
    <img src="/assets/images/thumbnail/15-fix-abg-font-thumbnail.png" alt="generate-font-settings-to-fix-Abg-font-thumbnail" width="45%" height="45%"/>  

	### TrueType or OpenType  

23. Now we will be determining whether our font will be True Type TTF or Open Type OTF by,  
a) clicking the drop down menu button, (mine displays ‘OpenType(CFF)’, the last setting I used).  
b) Then select your preferred format.  

    i. The common formats are TrueType or OpenType.  
    ii. In this example, we’ll be selecting OpenType-CFF.  
    <img src="/assets/images/thumbnail/16-change-abg-font-thumbnail.png" alt="opentype-truetype-settings-when-generating-your-font" width="45%" height="45%"/>  

	### Options Box  

24. Next, we’ll be clicking on the button called ‘Options’ which will bring up another small dialogue box called ‘Options’.  
    <img src="/assets/images/thumbnail/17-fix-abg-font-thumbnail.png" alt="generate-font-options-settings-for-changing-font-Abg-thumbnail" width="45%" height="45%"/>  

25. In the ‘Options’ dialogue box there are a number of settings to consider.  

26. The ‘Options’ box should be auto populated with the original font’s settings.  

27. If Fontforge doesn’t auto populate the ‘Options’ box, the following settings can be used. This applies to other fonts you want to generate as well.  
a) Tick ‘Hints’ and ‘Flex Hints’  
b) Tick the next four (4) boxes (TrueType Hints, PS Glyph Names, Apple, and OpenType)  
c) Tick ‘Lookup Names’.  

28. By selecting Apple, as well as the others mentioned, your font can be installed on both Mac and Windows operating systems.  
    
29. When you have finished,  
a)  click ‘OK’ to save your settings.  
    <img src="/assets/images/thumbnail/18-how-to-fontforge-options.png" alt="generate-font-options-settings-for-changing-font-Abg-thumbnail" width="45%" height="45%"/>  

30. Now you'll be back in the ‘Generate Fonts’ dialogue box, where you can,  
a) click ‘Generate’ to generate and save your updated font, to your nominated file path ready for reviewing.  
    <img src="/assets/images/thumbnail/19-fix-abg-font-thumbnail.png" alt="generating-your-font-dialogue-box" width="45%" height="45%"/>  

If you're on this page from another tutorial you can now head back there.  
<span class="fs-3">[Back to Font Names](/font-names/#generating-your-font){: .btn .mr-2}  [Back to Scale Glyphs](/scale-glyphs/#review--test){: .btn }</span>
{: .blockquote}

**Congratulations on making it to the end.**  

Tada! You have successfully updated your first Abg font thumbnail. If you'd like to see your font directory organized so that font styles are grouped in the same family, click on the tutorial for [font names].  

I hope this tutorial has been of assistance and you can put some of the information to good use when using Fontforge.  
<img src="/assets/images/thumbnail/20-change-abg-font-thumbnail.png" alt="finished-picture-of-abg-font-thumbnail" width="15%" height="15%"/>  

[font names]: /font-names  