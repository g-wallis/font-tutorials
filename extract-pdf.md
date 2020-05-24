---
layout: page  
title: Fonts From PDFs  
description: This tutorial will show you how to extract fonts from a PDF file using Fontforge.  
image: /assets/images/pdf/0-how-to-extract-fonts-pdf-fontforge.png
nav_order: 9  
permalink: /extract-pdf/  
---

<center><img src="/assets/images/pdf/1-how-to-extract-fonts-pdf-fontforge.png" alt="how-to-extract-fonts-from-pdf-in-fontforge" width="35%" height="35%"/></center>  

# HOW TO EXTRACT FONTS FROM A PDF FILE USING FONTFORGE  

**This tutorial will show you how to extract fonts from a PDF file using Fontforge.**  

## How this Tutorial Is Organized  
{: .no_toc }

1. A brief outline on the limitations regarding font extraction.  
2. Then we’ll go through an example where a partial font can be extracted.  
3. Followed by a second example where no font can be extracted.  

>  i. You can download Fontforge for Windows, Mac, or Linux from [here](https://fontforge.org/en-US/downloads/).  
>  ii. The documents used in this tutorial are [Elements of Typographic Style v3 – Extract](http://s3.amazonaws.com/arena-attachments/2584673/e36028a1643a616ec4be1e8d0e859fbb.pdf?1534885560) and [FontNaming-kltf](https://kltf.de/downloads/FontNaming-kltf.pdf).  
>  iii. This tutorial is shown on a Windows 10 computer with Fontforge version 03142020.  
>  iv. Fontforge does crash, so save often.  

---

## Extracting Limitations  

The following factors need to be considered when using Fontforge to extracts glyphs from a PDF;  

4. Not all PDF documents can be read by Fontforge, because PDF documents can have restrictions, formatting peculiarities, embedded font, glyphs as pictures or some other configuration.  

5. Sometimes when a font is embedded into a PDF it will only contain the glyphs used.  
a) For example, if the PDF document you are trying to extract from does not contain the letter ‘Z’, then that letter will not be present.  

6. Where all the glyphs are present in the PDF document, Fontforge may not extract them all.  
a) This could be down to Fontforge’s code capabilities, the PDF format, it’s subsetting and optimization, locked or embedded PDF settings, or perhaps a little of both.  

7. Most PDFs which are online, only embed subets of the font and not the full font.  
a) Extracting a subset of a font is only useful in a very limited scope, if at all.  

8. When processing your extraction, Fontforge may display error dialogue boxes.  
a) If there are errors in the file, you can choose to ignore them or save the file and edit them.  
b) Most of the errors can be fixed automatically if you click "Fix" enough times.  

---

## Partial Extraction  

9. With this knowledge, we’ll begin with an example that produces a partial font extraction.  

10. Start by opening Fontforge, and on the first dialogue box,  
a) click on the button next to ‘Filter’,  
b) Select ‘Extract from PDF’ from the list,  

	<img src="/assets/images/pdf/2-how-to-extract-fonts-pdf-fontforge.png" alt="open-fontforge-select-extract-pdf-font" width="40%" height="40%"/>  

    c) Then, locate and select your PDF file,  
    d) Click ‘OK’.  

	<img src="/assets/images/pdf/3-how-to-extract-fonts-pdf-fontforge.png" alt="open-fontforge-select-file-extract-font-from-pdf" width="40%" height="40%"/>  

11. **Be aware** that completing step c) before b) will not show any PDF file to select. You must complete step b) before c) for PDF files to be recognized.  
    {: .tip}

12. If Fontforge is able to detect glyphs from the PDF, a dialogue box called 'Pick a font' will pop up listing the fonts detected within the PDF.  
a) Select your preferred font and click ‘OK’.  

	<img src="/assets/images/pdf/4-how-to-extract-fonts-pdf-fontforge.png" alt="select-font-to-extract-from-list" width="30%" height="30%"/>  

13. You'll be taken to 'Font View' where you can see the extracted glyphs.  

	<img src="/assets/images/pdf/5-how-to-extract-fonts-pdf-fontforge.png" alt="displays-result-of-font-from-pdf-extraction" width="70%" height="70%"/>  

14. From here you can either,  
a) abandon the whole idea,  
b) go ahead with the glyphs that have been extracted, or  
c) try another PDF document.  

15. To view, only the cells which have glyphs,  
a) click on ‘Encoding>Compact’  

	<img src="/assets/images/pdf/6-how-to-extract-fonts-pdf-fontforge.png" alt="compact-view-of-extracted-glyphs" width="70%" height="70%"/>  

16. With only the extracted glyphs visible, you’re now in a position to decide what to do next.  

	<img src="/assets/images/pdf/7-how-to-extract-fonts-pdf-fontforge.png" alt="compact-view-of-extracted-glyphs" width="70%" height="70%"/>  

17. To be able to view all the extracted glyphs, neatly on screen, I'll go ahead, and delete all the cells where the glyph is represented as a ‘square’.  

	<img src="/assets/images/pdf/8-how-to-extract-fonts-pdf-fontforge.png" alt="delete-empty-glyphs-from-extracted-fonts-from-pdf-in-fontforge" width="70%" height="70%"/>  

18. And to hide these empty glyphs I'll need to go back and,  
a) click on ‘Encoding>Compact’ which will expand the table, then  
b) repeat this action by clicking on ‘Encoding>Compact’.  

	<img src="/assets/images/pdf/9-how-to-extract-fonts-pdf-fontforge.png" alt="repeat-compact-process-two-times-to-view-extracted-glyphs" width="70%" height="70%"/>  

---

## No Extraction  

19. For the next example, I repeated the same steps above only selecting a different PDF file, ‘FontNaming-ktlf.pdf’.  

20. On this occasion, Fontforge is not able to read the PDF. In this situation Fontforge displays two (2) pop up dialogue boxes outlining the reason why.  
a) The dialogue box advises that the font is encrypted and cannot be read.  

	<img src="/assets/images/pdf/10-how-to-extract-fonts-pdf-fontforge.png" alt="warning-box-advising-font-cannot-be-read" width="45%" height="45%"/>  

	<img src="/assets/images/pdf/11-how-to-extract-fonts-pdf-fontforge.png" alt="warning-box-advising-font-cannot-be-read-it's-encrypted" width="70%" height="70%"/>  

21. As a result, there's nothing more that can be done on this PDF to extract it's font using Fontforge.  

**That brings us to the end of this tutorial.**  

I hope this tutorial has been of assistance and you can put some of the information to good use when extracting fonts from a PDF.  