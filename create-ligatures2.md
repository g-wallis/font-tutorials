---
layout: page
title: Ligature Tables 2
description: This tutorial will show you how to create ligature tables in Fontforge, via ‘Glyph Info’.
image: /assets/images/ligature2/0-how-to-create-ligature-tables-fontforge.png  
nav_order: 6
permalink: /create-ligatures2/  
---

<center><img src="/assets/images/ligature2/1-how-to-create-ligature-tables-fontforge.png" alt="how-to-create-ligature-tables-in-fontforge" width="35%" height="35%"/></center>  

# HOW TO CREATE LIGATURE TABLES USING FONTFORGE VIA GLYPH INFO  

**This tutorial will show you how to create ligature tables in Fontforge, via ‘Glyph Info’.**  

<center><img src="/assets/images/ligature2/2-how-to-create-ligature-tables-fontforge.png" alt="how-to-create-ligature-tables-in-fontforge" width="25%" height="25%"/></center>  

## How this Tutorial Is Organized  
{: .no_toc}

1. We’ll start with a brief definitions section.  
2. Next we'll add a new encoding slot so that we can create and build the ‘tt’ ligature.  
3. Then we’ll add a single substitution lookup table, using ‘Glyph Info’.  
4. Next we’ll type ‘tt’ in “Metrics View’ to check whether our ligature table works.  
5. To finish off, I'll provide tips in case your ligature lookup table may not be working.

>  i. You can download Fontforge for Windows, Mac, or Linux from [here](https://fontforge.org/en-US/downloads/).  
>  ii. The font used in this tutorial is called [Belmist](https://www.dafont.com/belmist.font?%5b%5d=10). It’s a free font for personal and commercial use with an open source license.  
>  iii. This tutorial is shown on a Windows 10 computer with Fontforge version 03142020.  
>  iv. Fontforge does crash, so save often.  

---

## Definitions  

**This is 'Font View**  

<img src="/assets/images/ligature2/3-how-to-create-ligature-tables-fontforge.png" alt="font-view-in-how-to-create-ligature-tables-fontforge" width="70%" height="70%"/>  

**This is 'Metrics View'**  

<img src="/assets/images/ligature2/3i-how-to-create-ligature-tables-fontforge.png" alt="metrics-view-in-how-to-create-ligature-tables-fontforge" width="70%" height="70%"/>  

--- 

## Adding A New Encoding Slot  

5. For this tutorial we’ll be adding a new encoding slot for the ‘tt’ ligature, however you can also,  
a) use one of the Private Use Area (PUA) Unicode slots which start at E000, or  
b) use one of the Unicode slots for ligatures at FB00, or  
c) use an existing Unicode slot.  

6. To add a new encoding slot,  
a) Click on ‘Encoding>Add Encoding Slots’  

    <img src="/assets/images/ligature2/4-how-to-create-ligature-tables-fontforge.png" alt="adding-a-new-encoding-slot-for-ligature-tables-in-fontforge" width="70%" height="70%"/>  

7. On the next screen that pops ups,  
b) Insert the number of encoding slots to add.  
c) Then click ‘OK'.  

    <img src="/assets/images/ligature2/5-how-to-create-ligature-substitution-lookup-tables.png" alt="nominating-number-of-encoding-slots-for-ligature-tables-in-fontforge" width="40%" height="40%"/>  

8.  The new encoding slot will be added to the end and right at the bottom of ‘Font View’.

---

## Naming Your New Encoding Slot  

Now we need to name our new encoding slot.  

9. Click on the new encoding slot glyph cell,  
a) then right click  
b) Select ‘Glyph Info’  

    <img src="/assets/images/ligature2/6-how-to-create-ligature-substitution-lookup-tables.png" alt="glyph-info-menu-for-single-substitution-lookup-table" width="80%" height="80%"/>  

10. On the next screen, make sure ‘Unicode’ is selected in the left hand column then,  
a) In the box next to ‘Glyph Name’, manually type in the name of your glyph.  
    In this example we’ll be typing: `t_t`  
    <img src="/assets/images/ligature2/7-how-to-create-ligature-substitution-lookup-tables.png" alt="naming-your-new-encoding-slot-for-ligature-tables-in-fontforge" width="70%" height="70%"/>  

12. **Note** it is standard practice for ligatures to have an underscore ( _ ) separating glyphs, although Fontforge seems to recognize either; an underscore (f_i) or, no underscore (fi) for the output fi.  
a) or this tutorial, we’ll be using an underscore ( _ ).  
    {: .blockquote}  

13. For a detailed explanation of the Glyph Info dialogue box visit Fontforge’s [userguide](https://fontforge.org/docs/ui/dialogs/charinfo.html).  

14. Once you’ve named your new encoding slot, we'll move on to creating a ligature substitution lookup table.  

---

## Creating the Lookup Table  

15. To create a ligature substitution lookup table, make sure you're still in the ‘Glyph Info’ dialogue box from the previous step.  
a) Now select ‘Ligatures’ in the left hand column, then  
b) Select ‘New L>New Lookup Subtable’.  

    <img src="/assets/images/ligature2/8-how-to-create-ligature-substitution-lookup-tables.png" alt="adding-a-table-for-single-substitution-lookup-table" width="70%" height="70%"/>  

16. When the ‘Lookup’ dialogue box pops up,  
    a) select ‘Ligature Substitution’ from the drop down list at the top, next to the word ‘Type:’.  

    <img src="/assets/images/ligature2/9-how-to-add-ligature-lookup-table-fontforge.png" alt="completing-the-lookup-dialogue-box" width="50%" height="50%"/>  

    b) Now click on the little button next to <New\> to add a new line, which should also trigger a drop down list.  
    <img src="/assets/images/ligature2/10-how-to-add-ligature-substitution-lookup-table.png" alt="adding-a-new-line-to-single-substitution-lookup-table" width="50%" height="50%"/>  

    c) Select ‘liga Standard Ligatures’.  
    <img src="/assets/images/ligature2/11-how-to-create-ligature-substitution-lookup-tables.png" alt="selecting-liga-from-the-menu-for-single-substitution-lookup-table" width="50%" height="50%"/>  

17. The ‘Lookup Name’ will now be auto populated and a ‘liga’ will be added to the feature column.  
a)  You can either keep the default 'Lookup Name' or change it.  
b) In this example I’m going  to keep it.  
    <img src="/assets/images/ligature2/12-how-to-add-ligature-substitution-lookup-subtable.png" alt="changing-the-font-lookup-name-in-fontforge" width="50%" height="50%"/>  

18. Next,  
a) Go ahead and untick ‘Store ligature data in AFM files’,  
b) then click ‘OK’.  

    <img src="/assets/images/ligature2/13-how-to-create-ligature-substitution-lookup-tables.png" alt="saving-your-lookup-table" width="50%" height="50%"/>  

19. A new dialogue box will pop up asking you to name this subtable. The next step in this tutorial will guide you through the process of naming and completing this subtable.  

### Adding a Ligature Substitution Subtable  

20. To add the corresponding ligature substitution subtable go ahead and,  
a) Click ‘OK’ to accept the default name, or change it.  

    <img src="/assets/images/ligature2/14-how-to-add-ligature-substitution-lookup-tables.png" alt="adding-a-subtable-to-your-single-substitution-lookup-table" width="70%" height="70%"/>  

21. The subtable name will be added to the subtable column on the left.  

    <img src="/assets/images/ligature2/15-how-to-add-ligature-substitution-lookup-subtables.png" alt="auto-populated-subtable-name" width="70%" height="70%"/>  

22. Next, we’ll need to associate our ligature glyphs with their default source glyphs.  

22. We'll do this by typing the letters into the right hand column called 'Source Glyph Names'.  
a)  In this example I’ll enter: `t t`  
b)  If your ligature is made up of more than 1 source glyph, separate them with a ‘space’.  

    For example: mpl = m p l  

    Our example is:  tt =  t t  

    We will type: t t  making sure to separate each glyph with a space.  
    
    c) To view your entries you can hover your mouse over the source glyphs and a pop up will appear.  

23. When you've finished,  
a) click ‘OK’ to commit and save your ligature substitution lookup table.  

    <img src="/assets/images/ligature2/16-how-to-add-ligature-substitution-lookup-tables.png" alt="click-ok-to-save-your-single-substitution-lookup-table" width="80%" height="80%"/>  

24. We have now completed adding a ligature substitution lookup table and you should be back in ‘Font View’, ready for the next step.  

---

## Building a Composite Glyph  

25. Next, we need to build a composite glyph that will go into the new encoding slot.  

26. Make sure the new encoding slot you created, is selected, then  
a) click ‘Element>Build>Build Composite Glyph’.  

    <img src="/assets/images/ligature2/17-how-to-build-composite-glyphs.png" alt="building-a-composite-glyph-for-your-ligature-lookup-table" width="70%" height="70%"/>  

27. **Note** if you find that your ‘Element>Build’ is grayed out, it means that Fontforge is not yet able to recognize what glyphs it should use to build your composite glyph.  
a) In other words, you need to add a ligature substitution lookup table first, then come back and you’ll be able to access ‘Element>Build’ to complete this step.<br>
    <img src="/assets/images/ligature2/18-how-to-build-composite-glyphs.png" alt="grayed-out-build-a-composite-glyph-for-your-ligature-lookup-tablecomposite" width="80%" height="80%"/>  
    {: .blockquote}

28. After clicking ‘Element>Build>Build Composite Glyph’ your glyph cell should now be filled with two (2) glyphs.  
    <img src="/assets/images/ligature2/19-how-to-build-composite-glyphs.png" alt="you-ligature-will-now-be-visible-in-fontview" width="70%" height="70%"/>  

    ### Unlink Reference  

29. Before we edit the glyphs in this cell, we need to ‘unlink’ them from their source, otherwise any changes we make to the glyphs within the new encoding slot, will change the source glyphs.  

30. Linked glyphs or references will display a character above the glyph in ‘character view’.  
a)  You can get to ‘character view’ by double clicking a glyph cell from ‘Font View’.  
    <img src="/assets/images/ligature2/20-how-to-unlink-references-fontforge.png" alt="unlink-references-in-fontforge" width="50%" height="50%"/>  

31. To unlink them, make sure your new encoding slot is still selected, then;  
a) click ‘Edit>Unlink Reference’.  
    <img src="/assets/images/ligature2/21-how-to-unlink-references-fontforge.png" alt="how-to-unlink-references-in-fontforge" width="80%" height="80%"/>  

32. Your new encoding slot glyphs are now independent to your base glyphs and ready for editing, removing overlaps and adjusting the caret.  

33. Once you’ve finished editing, removing overlaps and adjusting the caret, you can move on to testing the lookup table.  

    <img src="/assets/images/ligature2/22-how-to-unlink-references-fontforge.png" alt="before-and-after-unlinking-references-caret-remove-overlaps-glyph-pictures" width="70%" height="70%"/>  

---

## Testing the Lookup Table  

34. To test your lookup table,  
a) go to ‘Font View’,  
b) click ‘Metrics>New Metrics Window',  
    <img src="/assets/images/ligature2/23-how-to-test-ligatures-fontforge.png" alt="testing-your-single-substitution-lookup-table-in-metrics-view" width="70%" height="70%"/>  
c) type ‘ttle’ in the text box, and  
d) deselect ‘liga’ by holding down ‘Ctrl’ on your keyboard and ‘Left Mouse Click’ with your mouse pointer on the word ‘liga’  

    <img src="/assets/images/ligature2/24-how-to-test-ligatures-fontforge.png" alt="reviwing-liga-ligature-by-typing-letters-into-metrics-view" width="70%" height="70%"/>  

35. Congratulations on making it to the end and creating your lookup table.

---

## It's Not Working  

36. If you see your ligature changing within the ‘Metrics View’, congratulations, if you don’t, go back and make sure:  
a)  you’ve followed the instructions step by step and haven't skipped a step like 'build composite glyphs'.  
b)  Check spaces and your spelling,  
c)  adjust the kerning of your new glyphs,  
d)  check that you've entered the correct letters in the subtable,  
e)  consider saving, closing Fontforge and restarting Fontforge.  
f)  'Default Using Suffix' will never work if you've used Fontforge's 'Mass Glyph Rename' function. I’ve outlined the reasons why and what to do, to be able to use ‘Default Using Suffix’, [here].  

**That brings us to the end of this tutorial.**  

I hope this tutorial has been of assistance and you can put some of the information to good use when using Fontforge.  

[here]: /contextual-chain/#problems-completing-the-subtable