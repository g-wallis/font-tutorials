---
layout: page  
title: Ligature Tables 1  
description: This tutorial will show you how to create ligature substitution tables in Fontforge, via ‘Font Info’.  
image: /assets/images/ligature1/0-how-to-create-ligature-tables-fontforge.png
nav_order: 5  
permalink: /create-ligatures1/  
---

<center><img src="/assets/images/ligature1/1-how-to-create-ligature-tables-fontforge.png" alt="how-to-create-ligature-tables-in-fontforge" width="35%" height="35%"/></center>  

# HOW TO CREATE LIGATURE TABLES USING FONTFORGE VIA FONT INFO  

**This tutorial will show you how to create ligature substitution tables in Fontforge, via ‘Font Info’.**  

<center><img src="/assets/images/ligature1/2-how-to-create-ligature-tables-fontforge.png" alt="how-to-create-ligature-tables-in-fontforge" width="25%" height="25%"/></center>  

## How this Tutorial Is Organized  
{: .no_toc}

1. We'll start with a brief outline of definitions.  
2. Followed by adding a new encoding slot so that we can create and build the ‘fi’ ligature.  
3. Then we’ll add a single substitution lookup table, using ‘Font Info’.  
4. Next we’ll type ‘fi’ in 'Metrics View’ to check whether our ligature table works.  
5.  To finish off, I'll provide tips in case your ligature lookup table may not be working.  

>  i. You can download Fontforge for Windows, Mac, or Linux from [here](https://fontforge.org/en-US/downloads/).  
>  ii. The font used in this tutorial is called [Playball](https://fonts.google.com/specimen/Playball). It’s a free font for personal and commercial use with an open source license.  
>  iii. This tutorial is shown on a Windows 10 computer with Fontforge version 03142020.  
>  iv. Fontforge does crash, so save often.  
>  v. Detailed information on lookup tables can be found at [Fontforge](https://fontforge.org/docs/ui/dialogs/lookups.html).  

---

## Definitions  

**This is 'Font View'**  

<img src="/assets/images/ligature1/3-how-to-create-ligature-tables-fontforge-font-view.png" alt="font-view-for-ligature-tables-in-fontforge" width="70%" height="70%"/>  

| Title | Meaning | Also Known As |
|---|---|---|
Single Substitution Lookup Table | It's a table you create when you want to replace a single glyph with another single glyph. | Lookup, Lookup table, Substitution Lookup, Single Substitution Lookup  
Subtable | Every lookup table has one or more subtables that defines what glyph will replace another glyph. | Lookup subtable, Substitution subtable, Single substitution lookup subtable  

---

## Adding A New Encoding Slot  

5. For this tutorial we’ll be adding a new encoding slot for the ‘fi’ ligature, however you can also,  
a) use one of the Private Use Area (PUA) Unicode slots which start at E000,  
b) use one of the Unicode slots for ligatures at FB00, or  
c) use an existing Unicode slot.  

6. To add a new encoding slot, make sure you’re in ‘Font View’ then,  
a) Click on ‘Encoding>Add Encoding Slots’.  

    <img src="/assets/images/ligature1/4-how-to-create-ligature-tables-fontforge.png" alt="add-an-encoding-slot-for-ligature-substitution-lookup-table-fontforge" width="70%" height="70%"/>  

7. On the next screen that pops ups,  
a) Insert the number of encoding slots to add.  
b) Then click ‘OK’.  
    <img src="/assets/images/ligature1/5-how-to-create-ligature-substitution-tables-fontforge.png" alt="add-an-encoding-slot-for-ligature-substitution-lookup-table-fontforge" width="40%" height="40%"/>  

8.  The new encoding slot will be added to the end and right at the bottom of ‘Font View’.  

### Naming Your New Encoding Slot  

9.  Now we need to name our new encoding slot.  

10. Click on the new encoding slot glyph cell,  
a) then right click  
b) Select ‘Glyph Info’  
    <img src="/assets/images/ligature1/6-how-to-create-ligature-substitution-tables-fontforge.png" alt="menu-in-to-select-glyph-info-fontforge" width="70%" height="70%"/>  

11. On the next screen, make sure ‘Unicode’ is selected in the left hand column then,  
a) In the box next to ‘Glyph Name’, manually type in the name of your glyph.  
    In this example we’ll be typing: `f_i`  
    <img src="/assets/images/ligature1/7-how-to-create-ligature-substitution-tables-fontforge.png" alt="glyph-info-dialogue-box-in-fontforge" width="70%" height="70%"/>  

12. **Note** it is standard practice for ligatures to have an underscore ( _ ) separating glyphs, although Fontforge seems to recognize either; an underscore (f_i) or, no underscore (fi) for the output fi.  
a) For this tutorial, we’ll be using an underscore ( _ ).  
    {: .blockquote}  

13. Once you’ve named your new encoding slot,  
a) Click ‘OK’, to take you back to ‘Font View’.  
    <img src="/assets/images/ligature1/8-how-to-create-ligature-substitution-lookup-tables.png" alt="glyph-info-dialogue-box-in-fontforge" width="70%" height="70%"/>  

For a detailed explanation on completing all the fields in the Glyph Info dialogue box, visit Fontforge’s [userguide](https://fontforge.org/docs/ui/dialogs/charinfo.html).  

### Building Your Composite Glyph  

Now that we've named our new encoding slot, we need to build a composite glyph that will go into the new encoding slot.  

14. Make sure the new encoding slot you created, is selected, then  
a) Click ‘Element>Build>Build Composite Glyph’.  
    <img src="/assets/images/ligature1/9-how-to-create-ligature-substitution-lookup-tables.png" alt="build-composite-glyph-for-ligature-substitution-lookup-table-fontforge" width="70%" height="70%"/>  

15. **Note** if you find that your ‘Element>Build’ is grayed out, it means that Fontforge is not yet able to recognize what glyphs it should use to build your composite glyph.  
a) In other words, you need to add a ligature substitution lookup table first, then come back and you’ll be able to access ‘Element>Build’ to complete this step.<br>
    <img src="/assets/images/ligature1/10-how-to-create-ligature-substitution-lookup-tables.png" alt="grayed-out-build-composite-glyph-for-ligature-substitution-lookup-table-fontforge" width="80%" height="80%"/>  
    {: .blockquote}

16. After clicking ‘Element>Build>Build Composite Glyph’ your glyph cell should now be filled with two (2) glyphs, ready for editing.  
    <img src="/assets/images/ligature1/11-how-to-create-ligature-substitution-lookup-tables.png" alt="populated-cell-for-ligature-substitution-lookup-table-fontforge" width="70%" height="70%"/>  

17. Before we edit the glyphs in this cell, we need to ‘unlink’ them from their source, otherwise any changes we make to the glyphs within the new encoding slot, will change the source glyphs.  

    a) **Note:** Linked glyphs or references will display a character above the glyph in ‘character view’. You can get to ‘character view’ by double clicking a glyph cell from ‘Font View’.  
    <img src="/assets/images/ligature1/12-how-to-unlink-references-fontforge.png" alt="unlink-references-fontforge" width="40%" height="40%"/>  
    {: .blockquote}

18. To unlink them, make sure your new encoding slot is still selected, then;  
a) Click ‘Edit>Unlink Reference’.  
    <img src="/assets/images/ligature1/13-how-to-unlink-references-fontforge.png" alt="menu-to-unlink-references-fontforge" width="70%" height="70%"/>  

19. Your new encoding slot glyphs are now independent to your base glyphs and ready for editing, removing overlaps and adjusting the caret.  
    <img src="/assets/images/ligature1/14-how-to-unlink-references-fontforge.png" alt="before-and-after-fi-ligature-substitution-lookup-table-fontforge" width="70%" height="70%"/>  

20. Once you’ve finished editing, removing overlaps and adjusting the caret, we can move on to adding the ligature substitution lookup table.  

---

## Adding A Ligature Substitution Lookup Table  

Next we need to create a Ligature Substitution Lookup Table to describe our changes.  

21. Make sure you’re in ‘Font View’ then,  
a) Click on ‘Element>Font Info’.  
    <img src="/assets/images/ligature1/15-how-to-add-ligature-lookup-table-fontforge.png" alt="font-info-menu-for-ligature-table-in-fontforge" width="70%" height="70%"/>  

22. On the next screen that pops up, make sure you’ve selected ‘Lookups’ in the left hand column, then  
a) click on ‘Add Lookup’.  
    <img src="/assets/images/ligature1/16-how-to-add-ligature-lookup-table-fontforge.png" alt="add-lookup-dialogue-box-for-font-lookup-table" width="70%" height="70%"/>  

23. When the ‘Lookup’ dialogue box pops up,  
a)  Select ‘Ligature Substitution’ from the drop down list at the top, next to the word ‘Type:’.  
    <img src="/assets/images/ligature1/17-how-to-add-ligature-lookup-table-fontforge.png" alt="drop-down-menu-in-lookup-dialogue-box-for-adding-a-single-substitution-lookup-table" width="50%" height="50%"/>  
b)  Now click on the little button next to <New\> to add a new line, which should also trigger a drop down list.  
    <img src="/assets/images/ligature1/18-how-to-add-ligature-substitution-lookup-table.png" alt="creating-a-new-line-in-lookup-dialogue-box-for-adding-a-single-substitution-lookup-table" width="50%" height="50%"/>  

24. If you clicked on ‘<New\>’ instead of the little button, you can either;  
a)  Delete the line and start again, or  
b)  you need to first click into the right hand column (1) blue area, then click into the left hand blue area (2), then  
    <img src="/assets/images/ligature1/19-how-to-add-ligature-substitution-lookup-table-fontforge.png" alt="when-no-pop-up-appears-complete--the-following-steps-in-fontforge-lookup-dialogue-box" width="50%" height="50%"/>  
c)  click on the little down button (3) in the left hand blue area to access the drop down list.   
    <img src="/assets/images/ligature1/20-how-to-add-ligature-substitution-lookup-table-fontforge.png" alt="when-no-pop-up-appears-complete--the-following-steps-in-fontforge-lookup-dialogue-box" width="50%" height="50%"/>  

25. When you do see the long drop down list,  
a)  Select ‘liga Standard Ligatures’.  
    <img src="/assets/images/ligature1/21-how-to-add-ligature-substitution-lookup-subtable-fontforge.png" alt="select-standard-ligatures-in-fontforge-lookup-dialogue-box" width="50%" height="50%"/>  

26. The ‘Lookup Name’ will now be auto populated and a ‘liga’ will be added to the feature column.  
    <img src="/assets/images/ligature1/22-how-to-add-ligature-substitution-lookup-subtable.png" alt="lookup-name-in-fontforge-lookup-dialogue-box" width="50%" height="50%"/>  

27. In the box next to ‘Lookup Name’, you can either keep the default name or change it.  
a)  In this example I’m going to change it to ‘liga’.  
    <img src="/assets/images/ligature1/23-how-to-add-ligature-substitution-lookup-subtable.png" alt="changing-the-lookup-name-in-fontforge-lookup-dialogue-box" width="50%" height="50%"/>  

28. Now go ahead and,  
a)  untick ‘Store ligature data in AFM files, and  
b)  click ‘OK.’  
    <img src="/assets/images/ligature1/24-how-to-add-ligature-substitution-lookup-subtable.png" alt="click-ok-to-save-adding-a-single-substitution-lookup-table" width="50%" height="50%"/>  

Now that we’ve added a Ligature Substitution lookup table the next step will be to add a corresponding subtable to it.  

### Adding a Ligature Substitution Subtable  

29. To add a subtable to our Ligature table,  
a)  click on ‘Add Subtable’.  
    <img src="/assets/images/ligature1/25-how-to-add-ligature-substitution-lookup-subtable.png" alt="adding-a-subtable-in-fontforge" width="70%" height="70%"/>  
b)  Click ‘OK’ to accept the default name, or you can rename it.  
    <img src="/assets/images/ligature1/26-how-to-add-ligature-substitution-lookup-subtable.png" alt="accepting-the-default-subtable-name-in-fontforge-lookup-dialogue-box" width="20%" height="20%"/>  
30. On the next dialogue box that pops up, we’ll associate our substitution glyphs with their default source glyphs by,  
a) clicking on ‘<New\>’ to create a new line.  
    <img src="/assets/images/ligature1/27-how-to-add-ligature-substitution-lookup-subtable.png" alt="populating-subtable-in-fontforge" width="50%" height="50%"/>  

31. Now we'll need to type the name of our ligature, into the left hand column.  
a)  In this example I’ll enter: `f_i`  
b)  Remember to separate each glyph with an underscore (_).  

    <img src="/assets/images/ligature1/28-how-to-add-ligature-substitution-lookup-subtable.png" alt="left-column-f_i-in-ligature-substitution-subtable-fontforge" width="50%" height="50%"/>  

32. Then in the right hand column, type the name of the source glyphs.  
a)  In this example I'll enter: `f i`  
b)  If your ligature is made up of more than 1 source glyph, separate them with a ‘space’.  

    For example: mpl = m p l  

    Our example is:  fi =  f i  

    We will type: f i  making sure to separate each glyph with a space.  The line should auto populate as you type and with the below example, Fontforge has added '(fi)' to the end.  
 
    c)  To view your entries you can hover your mouse over the source glyphs and a pop up will appear.  
    d)  Click ‘OK’.  
    <img src="/assets/images/ligature1/29-how-to-add-ligature-substitution-lookup-subtable.png" alt="right-column-f i-in-ligature-substitution-subtable-fontforge" width="50%" height="50%"/>  
    e)  Click ‘OK’ again to commit and save our ligature substitution lookup table.  
    <img src="/assets/images/ligature1/30-how-to-add-ligature-substitution-lookup-subtable.png" alt="click-ok-to-save-adding-a-subtable" width="70%" height="70%"/>  

31. We have now completed the ligature substitution lookup table and you should be back in ‘Font View’ ready for testing our ligature table.  

---

## Testing Your Ligature Lookup Table  

32. To test your lookup table, make sure you’re in ‘Font View’ then,  
a)  Click ‘Metrics>New Metrics Window’  
    <img src="/assets/images/ligature1/31-how-to-test-ligature-substitution-lookup-table.png" alt="testing-ligature-substitution-lookup-table-fontforge" width="70%" height="70%"/>  
b)  Type ‘ofid’, or letters of your own choosing, in the text box, and  
c)  deselect ‘liga’ by holding down ‘Ctrl’ on your keyboard and left mouse click with your mouse pointer on the word ‘liga’.  
    <img src="/assets/images/ligature1/32-how-to-test-ligature-substitution-lookup-table.png" alt="metrics-view-with-example-ligature" width="70%" height="70%"/>  
    <img src="/assets/images/ligature1/33-how-to-test-ligature-substitution-lookup-table.png" alt="metrics-view-without-example-ligature" width="70%" height="70%"/>  

33. Congratulations on making it to the end and creating your ligature lookup table.  

---

## It's Not Working  

34. If you see your ligature changing within the ‘Metrics View’, congratulations, if you don’t, go back and make sure:  
a)  you’ve followed the instructions step by step and haven't skipped a step like 'build composite glyphs'.  
b)  Check spaces and your spelling,  
c)  adjust the kerning of your new glyphs,  
d)  check that you've entered the correct letters in the subtable,  
e)  consider saving, closing Fontforge and restarting Fontforge.  
f)  'Default Using Suffix' will never work if you've used Fontforge's 'Mass Glyph Rename' function. I’ve outlined the reasons why and what to do, to be able to use ‘Default Using Suffix’, [here].  

**That brings us to the end of this tutorial.**  

I hope this tutorial has been of assistance and you can put some of the information to good use when using Fontforge.  

[here]:  /contextual-chain/#problems-completing-the-subtable  