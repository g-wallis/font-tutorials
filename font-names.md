---
layout: page
title: Font Names
description: This tutorial will show you how to name a font families so that they all group together in your operating system’s font location, as well as in Adobe Illustrator and Adobe Photoshop font previews, using Fontforge.    
image: /assets/images/name/0-how-to-name-font-families-fontforge.png
nav_order: 4
permalink: /font-names/
---

<center><img src="/assets/images/name/1-how-to-name-font-families-fontforge.png" alt="how-to-name-font-families-in-fontforge" width="35%" height="35%"/></center>  

# HOW TO NAME A FONT FAMILY IN FONTFORGE  

**This tutorial will show you how to name font families so they group together in your operating system’s font location, as well as in Adobe Illustrator and Adobe Photoshop font previews, using Fontforge.**  

## How this Tutorial is Organized  
{: .no_toc}

1. We’ll start by defining terms and discussing the reasons why you may want to change a font’s name.  
2. From here, we’ll open Fontforge and select a font file.  
3. Then we’ll change the font name and review error messages.  
4. Next, we’ll generate our re-named font.  
5. Then, we’ll review and test our font.  
6. Finally, I'll provide tips on why it may not be working for you.  

>  i. You can download Fontforge for Windows, Mac, or Linux from [here](https://fontforge.org/en-US/downloads/).  
>  ii. The font used in this tutorial is called [Linux Libertine](https://www.dafont.com/linux-libertine.font?l%5b%5d=10).  It’s a free font for personal and commercial use with an open source license.  
>  iii. This tutorial is shown on a Windows 10 computer with Fontforge version 03142020.  
>  iv. Fontforge does crash, so save often.  
>  v. Detailed information on naming conventions can be found at [Fontforge](https://fontforge.org/docs/ui/dialogs/fontinfo.html), [Microsoft](https://docs.microsoft.com/en-us/typography/opentype/spec/name), [Adobe].  

---

## Definitions  

**This is 'Font View'**  

<img src="/assets/images/name/2-how-to-name-font-families-fontforge.png" alt="font-view-of-naming-convention" width="70%" height="70%"/>  

6. Given font naming can be a little confusing, the following definitions will be used for this tutorial;  

| Title | Meaning | Example |
|---|---|---|
Font family name or family name | The name of a font | Linux Libertine, or Goodlight, or Lovers Quarrel.  
Font family or family | Font family name + the group of font styles associated with this Font family name |  Linux Libertine has 16 font styles and as a group (family name + font styles) this is a font family called Linux Libertine. <br>Lovers Quarrel has one (1) font style and as a group this is a font family called Lovers Quarrel.
Font styles or style | The style of font | bold, italic, small caps, regular, display capitals etc. These are all font styles. Linux Libertine has 16 font styles.  
Font name | Windows name for Font family + font style | Linux Libertine Bold, Linux Libertine Italic, Lovers Quarrel Regular

---

## Why Would You Change the Name of a Font  

7. There may be several reasons why you may want to change the name of a font or a group of fonts.  This tutorial will review some of the more common reasons and solutions, which are present using Linux Libertine as an example. The approach taken in this tutorial applies to all fonts not just the example font Linux Libertine.

8. To get started, I've gone ahead and installed all 16 font styles of Linux Libertine.  

    <img src="/assets/images/name/3-how-to-name-font-families-fontstyles.png" alt="example-linux-libertine-font-thumbnails" width="60%" height="60%"/>  

    **Problems**  

9. The first problem I see when reviewing Linux Libertine in my Windows font directory, is  
a) only nine (9) font styles out of 16 showed up, and  
b) it has installed in a manner where some font styles are grouped and others are not.  
    <img src="/assets/images/name/4-how-to-name-font-families-fontforge.png" alt="font-directory-with-font-thumbnails-scattered" width="60%" height="60%"/>  

10. This is a problem for me because I want them all grouped as one, not scattered in a random way that expands my font library, and I want to be able to use all 16 font styles not just nine (9).  

11. The next problem I see is, in Adobe Illustrator, when opening the font preview list.  
a) Again, some font styles are grouped, others are not, and some don’t appear at all.  
    <img src="/assets/images/name/5-how-to-name-font-families-fontforge.png" alt="adobe-illustrator-font-preview-menu-of-fonts" width="50%" height="50%"/>  

12. The problem with this is, it makes it hard to find fonts and it's time consuming having to scroll through hundreds of fonts in Adobe Illustrator or Photoshop. I also want to be able to use all 16 font styles not just nine (9).  

    **Why Don't They All Show Up?**  

13. The reason why some font styles appear and others don't is because many or all of the font styles, have the same ‘Font name’.  
a) For example when I click on the original thumbnails to open Linux Libertine, I can see some have the same 'Font name', which means only one file will appear when installed.
    <img src="/assets/images/name/6-how-to-rename-font-families-fontforge.png" alt="example-font-files-with-the-same-font-name" width="70%" height="70%"/>  

14. The remainder font styles (or files), you installed, will be buried and saved in your system. You will never see them and they will not be displayed or recognized unless you delete the font you can see, or of course change each file’s ‘Font name’.  

    **Why Are Some Grouped & Others Not?**  

15. The reason why some font styles are grouped and others are not is because,   
a) some font styles do not have identification that associates them to their font family, or  
b) they have identification, but it's in the wrong place and therefore not recognized, or  
c) they have identification, and therefore they are grouped.  

16. There's also the following, which display different groupings,  
a) a [Microsoft] naming convention which only allows four (4) font styles to be grouped. These are regular, bold, italic, bold italic.  
b) a Mac naming convention, and  
c) an [Adobe](https://www.adobe.com/content/dam/acom/en/devnet/font/pdfs/5088.FontNames.pdf) naming convention.  

    **Hidden Fonts Solution**  

17. The solution, to be able to see and use all 16 font styles of Linux Libertine, is to make sure each font style has a different ‘Font name’.  
a) For example: Linux Libertine Regular, Linux Libertine Bold, Linux Libertine Bold Italic.  
b) These changes need to be made using software that’s designed for fonts, like Fontforge.  

    **Ungrouped Fonts Solution**  

18. If I want all 16 font styles to be grouped or nested within the same font family in Windows and Adobe software, then each file needs to include identification that associates them to their font family.  
a) These changes can be made using Fontforge.

The next section of this tutorial will go through the steps, to change the 'Font name' and identification, so that all font styles are visable and grouped into font families.  

---

## Selecting a Font File  

19. To change a font name we need to open Fontforge, locate the font, select it and click 'OK'.  
    <img src="/assets/images/name/7-how-to-change-font-families-names-fontforge.png" alt="opening-a-font-in-fontforge" width="50%" height="50%"/>  

20. Ignore and close any warning dialogue boxes that open up.  
    <img src="/assets/images/name/8-how-to-see-installed-font-families-fontforge.png" alt="warning-popup-when-opening-a-font-in-fontforge" width="70%" height="70%"/>  

{: .tip}
- Make sure you're not selecting, changing or saving any fonts within your Windows font directory, or system directory.  
  - If you want to change these ones, copy them onto your desktop, make changes to the copy, then move the original to a safe place.  
  - Delete the one you’re replacing, do not save over the top of it because Windows will not ‘replace’ the file with this new one, it will bury the original beneath the replacement. This will slow down your computer.  

---

## Changing A Font Name  

Next we’ll be changing the details of the font name.  

21. Starting in ‘Font View’,  
a) click on ‘Element>Font Info’,  
    <img src="/assets/images/name/9-how-to-fix-font-names-fontforge.png" alt="font-info-menu-in-fontforge" width="70%" height="70%"/>  

22. The ‘Font Info’ dialogue box will pop up,  
a) select ‘PS Names’ in the left hand column.  

23. We’ll be changing what’s written in the boxes next to ‘Fontname’ and ‘Family Name’.  
a) Change ‘Fontname’ so there are no spaces and include a hyphen between the font family name and font style.  

        LinuxLibertine-DisplayCapitals  

    b)	On the second line called ‘Family Name’, you need to include a hyphen between the font family name and font style. There are no spaces between the hyphen.  

         Linux Libertine-Display Capitals  

    <img src="/assets/images/name/10-how-to-rename-font-families-fontforge.png" alt="how-to-rename-a-font-font-info-dialogue-box" width="100%" height="100%"/>  

    **OS/2 Settings**  

24. Now in the left hand column,  
a) Select ‘OS/2’  
b) Then, type either a ‘4’ or ‘5’ into the ‘OS/2 Version’ field.  

    i. This applies to all fonts. Currently there are [6 versions] with 0 being the oldest. [Apple] provides an easier to read document on OS/2 tables, and at the bottom of their page describes how Mac OS handles the OS/2 table.  
    {: .blockquote}

    <img src="/assets/images/name/11-how-to-change-font-names-fontforge.png" alt="OS/2-settings-for-changing-font-name-and-font-families" width="70%" height="70%"/>  

    After changing the settings in ‘OS/2’, we’ll move on to changing the information within ‘TTF Names’.  

    **TTF Names**  

25. Make sure you’ve selected ‘TTF Names’ in the left hand column, then  
a) Check that the cell next to ‘Family’ is populated with the same name you entered in the previous step from ‘PS Names>Family Name:’.  

         Linux Libertine-Display Capitals

    <img src="/assets/images/name/12-how-to-name-font-naming-convention-fontforge.png" alt="change-post-script-font-family-name-field-in-TTF names" width="90%" height="90%"/>  

26. Next we’ll be changing the cell next to ‘Styles (SubFamily)’.  
a) select and right mouse click on the cell next to ‘Styles (SubFamily)’, then  
b) select ‘Same as PostScript Names’ from the drop down.  
    <img src="/assets/images/name/13-how-to-name-font-naming-convention-fontforge.png" alt="change-post-script-font-style-subfamily-field-in-TTF" width="90%" height="90%"/>  

    i. The field will ‘go blank’, which is normal.  
    <img src="/assets/images/name/14-how-to-name-font-naming-convention-fontforge.png" alt="changing-subfamily-field-in-TTF-automatically-creates-blank-field-which-is-okay" width="90%" height="90%"/>  
    {: .tip}


    ii. If this drop down box doesn’t pop up, left mouse click into the dell and delete whatever is in there. In this example it's ‘Small Caps’.  
	iii. Then type the words that appear after the hyphen in your ‘Fontname’ field from the previous steps. In this example it’s ‘` DisplayCapitals `’.  
    <img src="/assets/images/name/15-how-to-name-font-naming-convention-fontforge.png" alt="manually-entering-subfamily-fontstyle-into-this-field" width="90%" height="90%"/>  

27. The next line we’ll change is the ‘UniquieID’ line.  
a) Select and right mouse click on ‘UniqueID’, then  
b) select ‘Delete’ from the drop down box.  
    <img src="/assets/images/name/16-how-to-name-font-naming-convention-fontforge.png" alt="delet-uniqueid-line-in-TTF" width="90%" height="90%"/>  


    i. If you forget to delete the ‘UniqueID’ line, a helpful message pops up when you click ‘OK’.  
    ii. If you do receive this pop up, click ‘Change’ which will delete the entry and take you back to ‘Font View’.  
    <img src="/assets/images/name/17-how-to-rename-font-naming-convention-fontforge.png" alt="change-uniqueid-line-in-TTF-warning-box" width="50%" height="50%"/>  
    {: .tip}


    iii. When you generate the font, and ‘UniqueID’ has been deleted, Fontforge will generate a new ‘UniqueID’ line. Fontforge takes the information from the ‘Name For Humans’. The ‘Name For Humans’ is found under the ‘PS Names’ tab.  

    <img src="/assets/images/name/18-how-to-rename-font-naming-convention-fontforge.png" alt="after-deleting-uniqueid-line-in-TTF-fontforge-generates-a-new-uniqueid-when-generating-font" width="90%" height="90%"/>  

    **Identification**

28. Now we’ll create 4 new entries so that our font styles associate and identify with their font family and group together.  

29. This section is a little tricky and annoying.  
a) If nothing pops up when you left mouse click on the cells, just click in the cell and start manually typing.  
b) Sometimes, clicking on the cell, deletes the line entirely and you’ll have to re-add the line and start again.  
c) You can also follow Fontforge’s inbuilt prompts which display when you hover over text.  

30. To create a new line,  
a) click on ‘New’,  
b) celect your language from the pop up list – English (US).  

    <img src="/assets/images/name/19-how-to-rename-font-naming-convention-fontforge.png" alt="creating-a-new-line-to-include-font-preferred-family-name" width="90%" height="90%"/>  

31. In the next column,  
a) click on ‘UniqueID’ and select ‘Preferred Family’.  

    <img src="/assets/images/name/20-how-to-change-fix-font-naming-convention.png" alt="preferred-family-name-in-font-naming-convention" width="90%" height="90%"/>  

32. In the last column we need to manually type our preferred family name.  
a) The ‘Preferred Family’ is the first half of the name you entered in the previous step from ‘PS Names>Family Name:’.  
b) In other words, it’s the words that appear *before* the hyphen in your ‘Family Name’ field from the previous steps.  
c) In this example it’s ‘Linux Libertine’.  

    <img src="/assets/images/name/22-how-to-change-fix-font-naming-convention.png" alt="preferred-family-name-is-taken-from-font-family-name" width="90%" height="90%"/>  

33. Next, we’ll add a second line just like we did in the previous step, but this time we’ll select ‘Preferred Style’.  
a) Click on ‘<New\>’  
b) Select ‘English (US)’ from the list.  

    <img src="/assets/images/name/23-how-to-change-fix-font-naming-convention.png" alt="preferred-style-name-in-font-naming-convention" width="90%" height="90%"/>  

34. In the next column,  
a) click on ‘UniqueID’ and select ‘Preferred Style’.  

    <img src="/assets/images/name/24-how-to-change-fix-font-naming-convention.png" alt="preferred-style-name-is-taken-from-font-family-name-font-style" width="90%" height="90%"/>  

35. In the last column we need to manually type our preferred style name.  
a) The ‘Preferred Style’ is the second half of the name you entered in the previous step from ‘PS Names>Family Name:’.  
b) It’s the words that appear *after* the hyphen in your ‘Family Name’ field from the previous steps.  
c) In this example it’s 'Display Capitals'.   

    <img src="/assets/images/name/25-how-to-change-fix-font-naming-convention.png" alt="preferred-style-name-is-taken-from-font-family-name-font-style" width="90%" height="90%"/>  

36. Now go ahead and create two (2) more rows, just as we did in the previous two rows, only this time changing the second column to ‘WWS Family’ and ‘WWS Subfamily’.  

37. When completed the additional 4 rows should look like this:  

    <img src="/assets/images/name/26-how-to-see-all-installed-missing-font.png" alt="add-wws-family-and-subfamily-lines" width="90%" height="90%"/>  

    a) Click ‘OK’ to save the changes and return to ‘Font View’.  

After clicking ‘OK’, you may receive an error message about long font names. The next section will help you overcome this.  

---

## Error Messages  

41. If your ‘Fontname’ and or ‘Family Name’ are too long, a dialogue box will pop up.  

42. If you receive one or both of these dialogue boxes,  
a) Click ‘Cancel’ and reduce the number of characters.  
b) ‘Family Name’ is related to the Windows error.  
c) ‘Fontname’ is related to the Adobe error.  

43. When you’ve finished reducing the name,  
a) click ‘OK’ to save the changes and return to ‘Font View’.  
b) There is no need to change the information within OS/2 or TTF Names.  
    <img src="/assets/images/name/27-how-to-see-all-installed-missing-font.png" alt="error-messages-because-of-long-fontnames-and-long-family-name" width="90%" height="90%"/>  

---

## Generating Your Font  

44. Now we’re ready to generate our font. Make sure you’re in ‘Font View’ then,  
a) click on ‘File>Generate Fonts’.  

    <img src="/assets/images/name/28-how-to-see-all-installed-missing-font.png" alt="file-menu-to-generating-your-font-in-fontforge" width="70%" height="70%"/>  

45. Head on over to my [Abg Font Thumbnail] tutorial for detailed instructions on generating fonts.  

46. When you've completed all the settings in the 'Generate Fonts' dialogue box,  
a) click 'Generate'.  

47. After clicking on 'Generate' you may receive an error pop up,  
a) click ‘Yes’.  

    <img src="/assets/images/name/29-how-to-see-all-installed-missing-font.png" alt="error-message-because-em-size-not-1000" width="50%" height="50%"/>  

48. Your updated font will save to your nominated file path ready for reviewing.   

---

## Review And Test 

49. Open your generated font and check the font name for correctness.  

50. Delete any legacy Linux Libertine fonts in your system.  
a) I’ve found it’s best to delete or uninstall the font you want to replace, then install the replacement font, rather than letting Windows ‘replace’ the new font, because Windows often saves over the top and buries the unwanted font deeper into the operating system.  

    <img src="/assets/images/name/30-how-to-see-all-installed-missing-font.png" alt="open-font-file-to-review-font-family-name" width="60%" height="60%"/>  

51. Then install your re-named Linux Libertine font styles and test them out to see if they’ve grouped within your font directory, and software font preview drop down lists.  

    <img src="/assets/images/name/31-how-to-see-all-installed-missing-font.png" alt="open-font-directory-and review-thumbnails-of-renamed-font" width="60%" height="60%"/>  
    <img src="/assets/images/name/32-how-to-see-all-installed-missing-font.png" alt="view-updated-font-in-adobe-illustrator-font-preview-menu-of-fonts" width="60%" height="60%"/>  

---

## It's Not Working

52. If it's not working out correctly, after you've followed this tutorial, then  
a) review what you've entered in the 'PS Names' section and the 'TTF Names' section,  
b) make sure the 'PS Names' section matches the 'TTF Names' section,  
c) check spelling throughout,  
d) check spaces, no spaces and hyphens are in the right place,  
e) go back and make sure you've followed the instructions, step by step.   


**That brings us to the end of this tutorial.** 

I hope this tutorial has been of assistance and you can put some of the information to good use when you want to change the font attributes using Fontforge.  

[Microsoft]:  https://docs.microsoft.com/en-us/typography/opentype/spec/name#name-ids  
[Adobe]:  https://www.adobe.com/devnet/font.html  
[Apple]: https://developer.apple.com/fonts/TrueType-Reference-Manual/RM06/Chap6OS2.html  
[6 versions]:  (https://docs.microsoft.com/en-us/typography/opentype/spec/os2)  
[Abg Font Thumbnail]:  /abg-thumbnails/#generating-your-font