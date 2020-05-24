---
layout: page  
title: Scale Glyphs  
description: This tutorial will show you how to scale glyphs in Fontforge.  
image: /assets/images/scale/0-how-to-scale-glyphs-fontforge.png
nav_order: 2  
permalink: /scale-glyphs/  
---

<center><img src="/assets/images/scale/1-how-to-scale-glyphs-fontforge.png" alt="how-to-scale-glyphs-in-fontforge" width="35%" height="35%"/></center>  

# HOW TO SCALE GLYPHS USING FONTFORGE  

**This tutorial will show you how to scale glyphs in Fontforge.**  

## How this Tutorial is Organized  
{: .no_toc }

1. We’ll start with a brief definitions section.  
2. Next we'll select the glyphs we want to scale.  
2. Then we'll go through the settings within the Transform dialogue box.  
3. Then we'll test the scaled glyphs to make sure we’re happy with them.  

> i. You can download Fontforge for Windows, Mac, or Linux from [here](https://fontforge.org/en-US/downloads/).  
> ii. The font used in this tutorial is called [Lovers Quarrel](https://www.fontsquirrel.com/fonts/lovers-quarrel). It’s a free font for personal and commercial use with an open source license.  
> iii. This tutorial is shown on a Windows 10 computer with Fontforge version 03142020.  
> iv. Fontforge does crash, so save often.  

---

## Definitions  

**This is 'Font View'**  

<img src="/assets/images/scale/2-how-to-scale-glyphs-fontforge.png" alt="font-view-for-scaling-glyphs-in-fontforge" width="70%" height="70%"/>  

--- 

## Selecting Glyphs  

In this tutorial we'll be selecting all the glyphs in Lovers Quarrel.  

4. To do this, make sure you’re in ‘Font View’ then,  
a) Click on ‘Edit>Select>Select All’  
	<img src="/assets/images/scale/3-how-to-scale-glyphs-fontforge.png" alt="select-all-glyphs-for-scaling-with-fontforge" width="70%" height="70%"/>  

5. Now that all the glyphs are selected,  
a) Click on ‘Element>Transformations>Transform’.  
	<img src="/assets/images/scale/4-how-to-scale-glyphs-fontforge.png" alt="transform-tool-to-scale-glyphs-in-fontforge" width="70%" height="70%"/>  

6.  The transform dialogue box will pop up and the next step will be to change the settings.  
 
---

## Transform Dialogue Box  

6. The transform' dialogue box includes several settings for you to consider, including performing a sequence of events.  
a) This tutorial does not explore sequences.  

7. Start by clicking on the drop down box next to the word ‘Origin:’ then,  
a) select ‘Glyph Origin’ from the list.  

    i. Selecting the ‘Glyph Origin’ option will scale our glyphs without compromising the original font structure, meaning kerning and spacing is maintained.  
	<img src="/assets/images/scale/5-how-to-scale-glyphs-fontforge.png" alt="transform-settings-to-scale-glyphs-in-fontforge" width="70%" height="70%"/>  

8. Next chose one of the following:  
a) Click ‘Scale Uniformly’ if you intend on scaling the width and height equally, or  
b) Click ‘Scale’ if you intend to scale with different width and height percentages.  
    For this tutorial, we’ll be selecting ‘Scale Uniformly’.  
	<img src="/assets/images/scale/6-how-to-scale-glyphs-fontforge.png" alt="how-to-scale-glyphs-in-fontforge-using-the-transform-tool" width="70%" height="70%"/>  

9. Enter your scale dimensions out of 100.  
a) I use between 140% - 160% when glyphs are around 600 above the baseline.  

10. If you would like to do more transforming and perform a sequence,  
a) Select the ‘Do Nothing’ drop down boxes, and choose the events that will occur after scaling.  

11. In this guide, we just want to scale, therefore we’ll be selecting ‘Do Nothing’.  

12. If you’ve inserted additional ‘Layers’, or ‘Guide Layers,’ tick these two boxes, otherwise leave them unticked.  

13. Tick the next three (3) boxes, then  
a) Click on ‘OK’.  
	<img src="/assets/images/scale/7-how-to-scale-glyphs-fontforge.png" alt="transform-settings-to-scale-glyphs-in-fontforge" width="70%" height="70%"/>  

14. Now wait for the transformation action to occur.  
	<img src="/assets/images/scale/8-how-to-scale-glyphs-fontforge.png" alt="scaled-results-in-font-view" width="70%" height="70%"/>  

---

## Review & Test  

15. Next, we'll look at two (2) options to review and test our scaled glyphs,  
a) using Fontforge's ‘Metrics View’, and  
b) generate and install the font, and test it in Adobe Photoshop and Adobe Illustrator.  

    ### Metrics View Testing  

16. First we'll review and test our scaled glyphs in ‘Metrics View’. Start from ‘Font View’ then,  
a) click on ‘Metrics>New Metrics Window’  
	<img src="/assets/images/scale/9-how-to-scale-glyphs-fontforge.png" alt="testing-scaled-glyphs-in-metrics-view" width="70%" height="70%"/>  

17. With the ‘Metrics View’ open,  
a) type into the text box and review each glyph for inconsistencies or things you want to change.  

18. For example, I've typed in 'own fox jumps' and noticed a couple of letters don't join up. This can be fixed using the kerning feature in Fontforge.  
a) I've circled these in red for illustration purposes.  
	<img src="/assets/images/scale/10-how-to-scale-glyphs-fontforge.png" alt="identifying-errors-in-metrics-view" width="70%" height="70%"/>  

20. This is what it looks like after adjusting the kerning.  
a)  It turns out the ‘o’ and ‘x’ are vertically apart and need to be manually extended in ‘Char View’.  
	<img src="/assets/images/scale/11-how-to-scale-glyphs-fontforge.png" alt="review-after-fixing-kerning" width="70%" height="70%"/>  

21. How to kern will not be discussed in this tutorial because it’s such a big topic and this tutorial is focused on how to scale glyphs.  

    ### Generating and Installing the Font  

22. Now we’ll look at reviewing and testing the scaled glyphs by generating and installing the font.  

23. If you're unsure on what to do with the 'generate font' settings, head on over to my [Abg Font Thumbnail] tutorial for detailed instructions on generating fonts.  

23. After you've generated your updated font,  
a) compare your scaled font with the original by double clicking on the font thumbnails to open.  
	<img src="/assets/images/scale/12-how-to-scale-glyphs-fontforge.png" alt="thumbnail-of-original-font-size" width="20%" height="20%"/>  <img src="/assets/images/scale/13-how-to-scale-glyphs-fontforge.png" alt="thumbnail-of-scaled-size" width="20%" height="20%"/>  
	<img src="/assets/images/scale/14-how-to-scale-glyphs-fontforge.png" alt="font-window-comparison-of-original-and-scaled-glyphs" width="60%" height="60%"/>  

24. Identify areas you may want to change.  

25. For example, I've circled these in red for illustration purposes.  
	<img src="/assets/images/scale/15-how-to-scale-glyphs-fontforge.png" alt="red-circled-errors-to-fix" width="90%" height="90%"/>  

26. I then installed the scaled font and opened Adobe Photoshop and Adobe Illustrator and tested the font, to see if it needed changes or it’s simply part of the font style.  
	<img src="/assets/images/scale/16-how-to-scale-glyphs-fontforge.png" alt="adobe-photoshop-font-preview-of-scaled-glyphs" width="33%" height="33%"/>  <img src="/assets/images/scale/17-how-to-scale-glyphs-fontforge.png" alt="adobe-illustrator-font-preview-of-scaled-glyphs" width="35%" height="35%"/>  
	<img src="/assets/images/scale/18-how-to-scale-glyphs-fontforge.png" alt="adobe-photoshop-font-preview-of-scaled-glyphs" width="43%" height="43%"/>  <img src="/assets/images/scale/19-how-to-scale-glyphs-fontforge.png" alt="adobe-illustrator-font-preview-of-scaled-glyphs" width="35%" height="35%"/>  

**That brings us to the end of this tutorial**  

I hope this tutorial has been of assistance and you can put some of the information to good use when scaling glyphs.  

[Abg Font Thumbnail]:  /abg-thumbnails/#generating-your-font  