---
layout: page  
headline: User Interface Settings  
title: How to Change the User Interface and Display Settings in Fontforge
description: This tutorial will show you how to change the appearance of some of the user interface settings in Fontforge.  
image: /assets/images/interface/0-how-to-change-user-interface-fontforge.png
nav_order: 3  
---

<center><img src="/assets/images/interface/1-change-display-settings-fontforge.png" alt="how-to-change-display-settings-using-fontforge" width="30%" height="30%"/></center>  

# {{ page.title }}  

**{{ page.description }}**  

## How this Tutorial is Organized  
{: .no_toc}

1. We’ll start with the appearance of cells in ‘Font View’.  
2. Then we’ll look at changing the size of ‘Font View’s’ interface.  
3. Next, we’ll specify the settings for an active cell.  
4. And lastly, I’ll show you how to change the display font for some dialogue boxes, so it’s easier to read.  

>  i. You can download Fontforge for Windows, Mac, or Linux from [here](https://fontforge.org/en-US/downloads/).  
>  ii. The two fonts used in this tutorial are called [Goodlight] and [Linux Libertine]. They're both free fonts for personal and commercial, use with an open source license.  
>  iii. This tutorial is shown on a Windows 10 computer with Fontforge version 03142020.  
>  iv. Fontforge does crash, so save often.  
>  v. Further information that describes each ‘X Resource Editor’ item can be found at [Fontforge’s] Github repository or Fontforge’s online [documentation].  

---

## Definitions  

**This is 'Font View'**  

<img src="/assets/images/interface/2-change-display-settings-fontforge.png" alt="font-view-how-to-change-display-settings-using-fontforge" width="70%" height="70%"/>  

---

## Glyph Cell Appearance  

5. This section will focus on the appearance of the cells within ‘Font View’ and whether or not you want to see metrics in each glyph cell.  
a) This is what ‘Font View’ looks like when all the glyph cell metrics are hidden from display.  
	<img src="/assets/images/interface/3-change-display-settings-fontforge.png" alt="font-view-cell-metrics-hidden-user-interface" width="70%" height="70%"/>  

	b) This is what ‘Font View’ looks like when all the glyph cell metrics are displayed.  
	<img src="/assets/images/interface/2-change-display-settings-fontforge.png" alt="font-view-cell-metrics-visible-in-fontforge-user-interface" width="70%" height="70%"/>  

6. To access the settings and change what you see in each glyph cell, you need to,  
a) Click on ‘View>Show H. Metrics…’,  
	<img src="/assets/images/interface/4-change-cell-metrics-settings-fontforge.png" alt="access-cell-metrics-settings-dialogue-box" width="70%" height="70%"/>  

	b) ‘Tick’ the boxes to show metrics or  
	c) ‘Untick’ the boxes to hide metrics from Font View.  
	d) Click ‘OK’ to save your settings.  
	<img src="/assets/images/interface/5-change-cell-metrics-settings-fontforge.png" alt="show-cell-metrics-dialogue-box" width="25%" height="25%"/>  

---

## Font View's Interface  

Next we’re going to change the size of ‘Font View’s’ interface.  

7. To change the interface settings,  
a) click on ‘View’  
b) then select your desired size from the list.  

8. Consider also selecting ‘anti-alias’ to sharpen the display. Be aware that ‘anti-alias’ is slower to generate.  
	<img src="/assets/images/interface/6-change-display-settings-fontforge.png" alt="change-font-view's-user-interface-size" width="70%" height="70%"/>  

9. You can also change the number of cells displayed by,  
a) clicking on ‘View’  
b) then select your desired cell window.  
	<img src="/assets/images/interface/7-change-display-settings-fontforge.png" alt="cell-window-display-size-menu" width="70%" height="70%"/>  

    **Included below are examples to consider:**  

10. This is an example of the display option  
a) ‘8x2 cell window’,  
b) with a ’96 pixel outline’,  
c) anti-aliased enabled.  
	<img src="/assets/images/interface/8-change-user-interface-fontforge.png" alt="example-8x2-cell-window-in-fontforge-user-interface" width="70%" height="70%"/>  

11. This is an example of the display option  
a) ‘16x4 cell window’,  
b) with a ’24 pixel outline’,  
c) anti-aliased disabled.  
	<img src="/assets/images/interface/9-change-display-settings-fontforge.png" alt="example-16x4-cell-window-in-fontforge-user-interface" width="50%" height="50%"/>  

12. This is an example of the display option  
a) ‘16x4 cell window’,  
b) with a ’48 pixel outline’,  
c) anti-aliased enabled.  
	<img src="/assets/images/interface/10-change-appearance-fontforge.png" alt="example-16x4-cell-window-in-fontforge-user-interface" width="70%" height="70%"/>  

---

## Active Cell Settings  

13. The next section looks at defining the ‘active cell’ settings. More specifically, when you click on a cell it becomes an active cell and we’ll be selecting a color that displays when you click on a cell.  
	<img src="/assets/images/interface/11-change-active-cell-settings-fontforge.png" alt="active-cell-settings-fontforge-user-interface" width="70%" height="70%"/>  

14. To change the background color an active cell,  
a) Click on ‘File>X Resource Editor’  
	<img src="/assets/images/interface/12-change-active-cell-settings-fontforge.png" alt="xresource-editor-in-fontforge-user-interface" width="70%" height="70%"/>  

15. Ensure you have ‘Font View’ selected in the left hand column, then  
a) change the ‘Selected BG Color’ (Background Color) to a color of your choosing.  
	<img src="/assets/images/interface/13-change-active-cell-settings-fontforge.png" alt="active-cell-background-color-settings-in-fontforge-user-interface" width="70%" height="70%"/>  
	<img src="/assets/images/interface/14-change-active-cell-settings-fontforge.png" alt="active-cell-background-color-settings-in-fontforge-user-interface" width="20%" height="20%"/>  

16. To change the color of the glyph when it's an active cell,  
a) change the ‘Selected FG Color’ (Foreground Color) to a color of your choosing.  
	<img src="/assets/images/interface/15-resource-editor-settings-fontforge.png" alt="active-cell-foreground-color-settings-in-fontforge-user-interface" width="70%" height="70%"/>  
	<img src="/assets/images/interface/16-change-active-cell-settings-fontforge.png" alt="active-cell-foreground-color-settings-in-fontforge-user-interface" width="20%" height="20%"/>  

17. When you have finished,  
a) Click ‘Save As’ and save your settings. For this example, I’ve called my personal preferences file, ‘setting1.txt’.  
b) If you click ‘OK’, the default setting will return the next time you open Fontforge.  
	<img src="/assets/images/interface/17-resource-editor-settings-fontforge.png" alt="save-and-name-personal-preferences-file-for-fontforge-user-interface" width="70%" height="70%"/>  

18. Test out your changes by selecting a few cells. If you don’t like the colors you’ve chosen, just repeat the process until you find colors you do.  
	<img src="/assets/images/interface/18-change-active-cell-settings-fontforge.png" alt="testing-active-cell-foreground-and-background-color-settings-in-fontforge-user-interface" width="70%" height="70%"/>  

---

## Display Font - Lookups  

Next we’ll be changing the display font for the ‘Element>Font Info>Lookups’ dialogue box.  

18. Here's a picture of the default font display for 'Lookups'. To change it, you’ll need to add a line of code to your personal preferences file.  
a) **Note** that adding the code to Fonforge’s ‘resources’ file or ‘preferences’ file, had no effect for me on Windows 10.  
	<img src="/assets/images/interface/19-change-display-font-fontforge.png" alt="font-display-settings-size-style-for-fontforge-user-interface" width="70%" height="70%"/>  

19. First you need to, create a personal preferences file via ‘File>X Resource Editor’.  
a) It’s the file you created when you changed the active cell color in the previous step, and clicked ‘save as’.  

20. If you haven’t already created a personal preferences file, go ahead and change any of the settings within the X Resource Editor and save your preferences to your hard drive by clicking ‘Save As’ and a box called ‘Save Resources File as’ will pop up asking you to name your file.   

    For this example, I’ve called my personal preferences file, ‘setting1.txt’.  

    a) Click ‘Save’  
	<img src="/assets/images/interface/17-resource-editor-settings-fontforge.png" alt="save-and-name-personal-preferences-file-for-fontforge-user-interface" width="70%" height="70%"/>  

21. Second, you need to close Fontforge so that any changes you make to your personal preferences file will take affect the next time you start Fontforge.  

22. Third, open your personal preferences file with Notepad or a text editor.  
a) To do this, right click on your personal preferences file and select either ‘open’ - to open with Notepad, or ‘open with’ and locate Notepad or ‘Edit with Notepad++’.  
	<img src="/assets/images/interface/21-change-display-font-fontforge.png" alt="locate-and-open-your-personal-preferences-file-for-fontforge-user-interface" width="50%" height="50%"/>  <img src="/assets/images/interface/22-change-display-font-fontforge.png" alt="choose-a-program-to-open-your-personal-preferences-file-for-fontforge-user-interface" width="20%" height="20%"/>  

23. Fourth, paste the example line of code into your personal preferences file, anywhere on a separate line or choose your own desired font, weight and size.  
	<img src="/assets/images/interface/23-change-display-font-fontforge.png" alt="paste-example-code-into-your-personal-preferences-file-for-fontforge-user-interface" width="50%" height="50%"/>  

24. Fifth, save and close your personal preferences file, then open up Fontforge, and navigate to 'Element>Font Info>Lookups' to view your changes.  

**Included below are some examples to consider:**  

<img src="/assets/images/interface/24-change-display-font-fontforge-trebuchet.png" alt="example-font-12pt-trebuchet" width="80%" height="80%"/>  

     fontforge.FontInfo.Font: 400 12pt Trebuchet MS  

---

<img src="/assets/images/interface/25-change-display-font-fontforge-segoe.png" alt="example-font-11pt-segoe" width="80%" height="80%"/>  

     fontforge.FontInfo.Font: 400 11pt Segoe UI  

---

<img src="/assets/images/interface/26-change-display-font-fontforge-Nirmala.png" alt="example-font-9pt-nirmala" width="80%" height="80%"/>  

     fontforge.FontInfo.Font: 400 9pt Nirmala UI  

---

<img src="/assets/images/interface/27-change-display-font-fontforge-Tahoma.png" alt="example-font-10pt-tahoma" width="80%" height="80%"/>  

     fontforge.FontInfo.Font: 600 10pt Tahoma  

---

<img src="/assets/images/interface/28-change-display-font-fontforge-verdana.png" alt="example-font-9pt-verdana" width="80%" height="80%"/>  

	 fontforge.FontInfo.Font: 400 9pt Verdana  

---

<img src="/assets/images/interface/29-change-display-font-fontforge-myriad-pro.png" alt="example-font-12pt-myriad-pro" width="80%" height="80%"/>  

	 fontforge.FontInfo.Font: 600 12pt Myriad Pro  

---

## Display Font - Show ATT

25. Next we’ll be changing the display font for the ‘View>ShowATT’ dialogue box, just like we did in the previous step for Lookups.  

	<img src="/assets/images/interface/30-change-display-font-fontforge.png" alt="showatt-display-font" width="70%" height="70%"/>  

26. This is what the default font looks like. To change it, you’ll need to add a line of code to your personal preferences file.  
	<img src="/assets/images/interface/31-change-display-font-fontforge.png" alt="adding-a-line-of-code-to-your-personal-preferences-file-for-fontforge-user-interface" width="35%" height="35%"/>  

27. Paste the example line of code into your personal preferences file, on a separate line or choose your own desired font, weight and size.  
	<img src="/assets/images/interface/32-change-display-font-fontforge.png" alt="insert-code-to-change-the-font-display-for-showatt" width="50%" height="50%"/>  

28. Save and close your personal preferences file, then open up Fontforge, and navigate to View>ShowATT to view your changes.  

**Included below are some examples to consider:**  

<img src="/assets/images/interface/33-change-display-font-fontforge-Tahoma.png" alt="example-font-8pt-tahoma" width="60%" height="60%"/>  

     fontforge.ShowATT.Font: 400 8pt Tahoma  

---

<img src="/assets/images/interface/34-change-display-font-fontforge-segoe.png" alt="example-font-10pt-segoe" width="60%" height="60%"/>  

     fontforge.ShowATT.Font: 400 10pt Segoe UI  

---

<img src="/assets/images/interface/35-change-display-font-fontforge-nirmala.png" alt="example-display-font-9pt-nirmala" width="60%" height="60%"/>  

     fontforge.ShowATT.Font: 400 9pt Nirmala UI 

---

<img src="/assets/images/interface/36-change-display-font-fontforge-trebuchet.png" alt="example-display-font-8pt-trebuchet" width="70%" height="70%"/>  

     fontforge.ShowATT.Font: 600 8pt Trebuchet MS  

---

## Display Font - Groups  

30. Next we’ll be changing the display font for the ‘Encoding>DisplayByGroups’ and ‘Encoding>DefineGroups’ dialogue boxes, just like we did in the previous steps for Lookups and ShowATT.  
    <img src="/assets/images/interface/37-change-display-font-fontforge.png" alt="change-display-font-for-groups-in-fontforge" width="70%" height="70%"/>  

    **Be aware** that within a couple of seconds after opening the ‘DisplayByGroups’ or ‘DefineGroups’ dialogue box, Fontforge crashes on Windows 10. This occurs with the default font and substituted font.  
    {: .note}

31. This is what the default font looks like;  
	<img src="/assets/images/interface/38-change-display-font-fontforge.png" alt="show-current-display-font-settings" width="30%" height="30%"/>  

32. To change it, you’ll need to add a line of code to your personal preferences file. Your changes will appear the next time you open Fontforge.  
	<img src="/assets/images/interface/39-change-display-font-fontforge.png" alt="you'll-need-to-adding-a-line-of-code-to-your-personal-preferences-file-for-fontforge-user-interface" width="50%" height="50%"/>  

    **Here are some examples:**  

<img src="/assets/images/interface/40-change-display-font-fontforge-tahoma.png" alt="example-display-font-8pt-tahoma" width="50%" height="50%"/>  

     Gdraw.Groups.Font: 400 8pt Tahoma  

---

<img src="/assets/images/interface/41-change-display-font-fontforge-nirmala.png" alt="example-display-font-10pt-nirmala" width="50%" height="50%"/>  

     Gdraw.Groups.Font: 400 10pt Nirmala UI

---

<img src="/assets/images/interface/42-change-display-font-fontforge-segoe.png" alt="example-display-font-9pt-segoe" width="50%" height="50%"/>  

     Gdraw.Groups.Font: 400 9pt Segoe UI  

**That brings us to the end of this tutorial.**  

I hope this tutorial has been of assistance and you can put some of the information to good use when using Fontforge.  

[Fontforge’s]: (https://github.com/fontforge/fontforge/blob/61ea6a817de0c0576c0b04b4faec956a7440666d/doc/sphinx/ui/misc/xres.rst)  
[documentation]: (https://fontforge.org/docs/ui/misc/xres.html).  
[Goodlight]: (https://www.dafont.com/goodlight.font?l%5b%5d=10)  
[Linux Libertine]: (https://www.dafont.com/linux-libertine.font?l%5b%5d=10)  