---
layout: page
headline: Contextual Ligature Table
title: How to Create Contextual Ligature Lookup Tables in Fontforge  
description: This tutorial will show you how to create contextual ligature lookup tables in Fontforge.  
image: /assets/images/contextual/0-how-to-create-contextual-lookups-fontforge.png
nav_order: 7
---

<center><img src="/assets/images/contextual/1-how-to-create-contextual-lookups-fontforge.png" alt="how-to-create-contextual-lookup-table-in-fontforge" width="30%" height="30%"/></center>  

# {{ page.title }}  

**{{ page.description }}**  

## How this Tutorial Is Organized  
{: .no_toc}

1. We'll start with a brief outline of definitions.  
2. Followed by creating a set of glyphs to be used in the lookup subtables.  
3. Then we’ll create two (2) separate single substitution lookup tables.  
4. Next, we’ll create a contextual substitution lookup table.  
5. Then we’ll test whether our contextual substitution lookup works.  
6. I’ll provide alternate formulas so you can see how they work, and 
7. I’ll give you some tips on why your contextual substitution lookup may not be working.  

>  i. You can download Fontforge for Windows, Mac, or Linux from [here](https://fontforge.org/en-US/downloads/).  
>  ii. The font used in this tutorial is called [Belmist](https://www.dafont.com/belmist.font?l%5b%5d=10). It’s a free font for personal and commercial use with an open source license.   
>  iii. This tutorial is shown on a Windows 10 computer with Fontforge version 03142020.  
>  iv. Fontforge does crash, so save often.  
>  v. Detailed information on lookup tables can be found at [Fontforge](https://fontforge.org/docs/ui/dialogs/lookups.html).  

---

## Definitions  

**This is 'Font View'**  

<img src="/assets/images/contextual/2-how-to-create-contextual-lookups-fontforge.png" alt="font-view-how-to-create-contextual-lookup-table-in-fontforge" width="70%" height="70%"/>  

| Title | Meaning | Also Known As |
|---|---|---|
Single Substitution Lookup Table | It's a table you create when you want to replace a single glyph with another single glyph. | Lookup, lookup table, substitution lookup, single substitution lookup  
Subtable | Every lookup table has one or more subtables that defines what glyph will replace another glyph. | Lookup subtable, substitution subtable, single substitution lookup subtable  
Contextual Substitution Lookup Table | It's a table describing glyph substitutions in context. It can be a substitution of one or more glyphs within a certain pattern of glyphs. | Contextual substitution lookup, contextual substitution table, contextual lookup  
Contextual Substitution Lookup Subtable | This has the same meaning as 'Subtable'  

--- 

## Nominating Glyphs  

8. For this tutorial we’ll be adding two single substitution lookup tables, and one contextual substitution lookup table.  

9. First we'll create a set of glyphs to be used for the first subtable.  
a)  In this example I’ve created:  

	     g.slant, s.slant, y.slant

    <img src="/assets/images/contextual/3-how-to-create-contextual-lookups-fontforge.png" alt="adding-glyphs-to-font-using-fontforge" width="70%" height="70%"/>  

10. Now, create a second set of glyphs that will be used for the second subtable.  
a)  In this example I’ve created:  

	     g.sc, s.sc, y.sc  

    <img src="/assets/images/contextual/4-how-to-create-contextual-lookups-fontforge.png" alt="how-to-add-glyphs-to-font-using-fontforge" width="70%" height="70%"/>  
	
---

## Single Substitution Lookup Table 1  

11. Now we will create our first single substitution lookup table to describe our changes.  

12. To create a new lookup table, make sure you’re in ‘Font View’ then   
a)  Click on ‘Element>Font Info’  
    <img src="/assets/images/contextual/5-how-to-create-contextual-substitution-fontforge.png" alt="adding-a-single-substitution-lookup-table-in-fontforge" width="70%" height="70%"/>  

13.  On the next screen that pops up, make sure you’ve selected ‘Lookups’ in the left hand column, then  
a)  select ‘Add Lookup’.  
    <img src="/assets/images/contextual/6-how-to-create-contextual-substitution-fontforge.png" alt="adding-a-lookup-table-in-fontforge" width="70%" height="70%"/>  

14. When the ‘Lookup’ dialogue box pops up,  
a)  Select ‘Single Substitution’ from the drop down list.  
b)  There’s no need to add a feature line item.  
c)  Type the name of your lookup in the box next to ‘Lookup Name:’  
    In this example I’ve named it ‘slant’.  
d)  Click ‘OK.’  

    <img src="/assets/images/contextual/7-how-to-create-contextual-substitution-table.png" alt="naming-a-single-substitution-lookup-table-in-fontforge" width="50%" height="50%"/>  

### Adding a Subtable  

15. Now we'll add a subtable to our lookup by,  
a)  selecting ‘slant’,  
b)  then click on ‘Add Subtable’.  

    <img src="/assets/images/contextual/8-how-to-create-contextual-substitution-fontforge.png" alt="adding-a-subtable-to-a-single-substitution-lookup-table" width="70%" height="70%"/>  

    c)  Then click ‘OK’ to accept the default name, or you can rename it.  

    <img src="/assets/images/contextual/9-how-to-create-contextual-substitution-table.png" alt="naming-lookup-table-in-fontforge" width="25%" height="25%"/>  

16. On the next dialogue box that pops up, we’ll associate our substitution glyphs with their default source glyphs by,  
a)  typing ‘slant’ in the box next to ‘Default Using Suffix’.  

    i. The suffix is linked to the name you gave your glyphs. For example, I called my new glyphs ‘`g.slant, s.slant, y.slant`’ and their suffix is ‘`slant`’.  
    ii. If I created ‘`g.name, s.name, y.name`’ their suffix would be ‘`name`’ and I would type ‘name’ in the box next to ‘Default Using Suffix’.   
    {: .blockquote}

    <img src="/assets/images/contextual/10-how-to-create-contextual-substitution-table.png" alt="default-using-suffix-to-add-a-subtable-in-fontforge" width="50%" height="50%"/>  

    b)  Now click the button called ‘Default Using Suffix’ to automatically fill the list.   

    <img src="/assets/images/contextual/11-how-to-create-contextual-substitution-lookup-table.png" alt="default-using-suffix-to-add-a-subtable-in-fontforge" width="50%" height="50%"/>  

    c)  If the list doesn’t auto fill,  

    - check the glyph names,  
    - check spelling,   
    - make sure you’re referring to the right names (g.sc and G.sc are not the same), are you thinking about the uppercase glyph and have named it with a lowercase letter.  
    - Try to manually type in the list, and as a last resort save, quit and restart Fontforge and start again.  
    - **Be aware** if you get a warning pop up asking ‘whether the glyphs you typed were intentional’, you need to save, quit, restart Fontforge and start again for the ‘Default Using Suffix’ button to work.  
    - 'Default Using Suffix' will never work if you've used Fontforge's 'Mass Glyph Rename' function. I've outlined the reasons why and what to do, to be able to use 'Default Using Suffix', [here].  
    {: .blockquote}

    d)  Click ‘OK’.  

    <img src="/assets/images/contextual/12-how-to-create-contextual-substitution-lookup-table.png" alt="saving-single-substitution-lookup-table-in-fontforge" width="50%" height="50%"/>  

---

## Single Substitution Lookup Table 2  

17. Now we'll create our second single substitution lookup table just as we did in the previous step, only now using the second set of glyphs.  

         g.sc, s.sc, y.sc  

18. We’re going to repeat the previous steps to create a new lookup table. Make sure you’re in ‘Font View’ then  
a)  Click on ‘Element>Font Info>Lookups>Add Lookup’.  
    <img src="/assets/images/contextual/13-how-to-create-contextual-substitution-lookup-table.png" alt="add-glyphs-to-font-using-fontforge" width="70%" height="70%"/>  

19. When the ‘Lookup’ dialogue box pops up,  
a)  Select ‘Single Substitution’ from the drop down list.  
b)  There’s no feature needed for this one.  
c)  Type the name of your lookup in the box next to ‘Lookup Name:’  
    In this example I’ve named it ‘sc’.  
d) Click ‘OK.’  

    <img src="/assets/images/contextual/14-how-to-create-contextual-substitution-lookup-table-fontforge.png" alt="creating-a-single-substitution-lookup-table-in-fontforge" width="50%" height="50%"/>  

### Adding a Subtable

20. Now, we need to create and name a subtable.  
a)  select ‘sc’,  
b)  then click ‘Add Subtable’.  

    <img src="/assets/images/contextual/15-how-to-create-contextual-substitution-lookup-table-fontforge.png" alt="completing-a-single-substitution-lookup-subtable-in-fontforge" width="70%" height="70%"/>  

    c) Click ‘OK’ to accept the default name.  

    <img src="/assets/images/contextual/16-how-to-create-contextual-substitution-lookup-table-fontforge.png" alt="accepting-default-name-in-fontforge" width="20%" height="20%"/>  

21. Next, we’ll associate our substitution glyphs with their default source glyphs.  
a)  Type ‘sc’ in the box next to ‘Default Using Suffix’.  

22. Then click the button called ‘Default Using Suffix’ to automatically fill the list.  
a)  Click ‘OK’ to take you back to the 'Font Info' dialogue box.  

    <img src="/assets/images/contextual/17-how-to-create-contextual-substitution-lookup-table-fontforge.png" alt="default-using-suffix-to-add-a-subtable-in-fontforge" width="50%" height="50%"/>  

---

## Contextual Substitution Lookup Table  

23. Next, we'll create another lookup table just as you did above, only now using ‘contextual substitution’.  

24. On the 'Font Info' dialogue box,  
a) click on ‘Add Lookup’.  

    <img src="/assets/images/contextual/18-how-to-create-contextual-substitution-lookup-table-calt.png" alt="adding-a-calt-contextual-lookup-table" width="70%" height="70%"/>  

25. When the ‘Lookup’ dialogue box pops up,  
a) select ‘Contextual Substitution’ from the drop down list at the top, next to the word ‘Type:’.  

    <img src="/assets/images/contextual/19-how-to-create-contextual-substitution-lookup-table-calt.png" alt="selecting-contextual-substitution" width="50%" height="50%"/>  

    b)  Now click on the little button next to ‘<New\>’ to add a new line, which should also trigger a drop down list.  

    <img src="/assets/images/contextual/20-how-to-create-contextual-substitution-lookup-table-calt.png" alt="completing-lookup-dialogue-box" width="50%" height="50%"/>  

    c)  select ‘calt Contextual Alternatives’ from the drop down list.  

    <img src="/assets/images/contextual/21-how-to-create-contextual-substitution-lookup-table-calt.png" alt="selecting-calt-contextual-alternatives-from-the-list" width="50%" height="50%"/>  

26. The ‘Lookup Name’ will now be auto populated and a ‘calt’ will be added to the feature column.  

    <img src="/assets/images/contextual/22-how-to-create-contextual-substitution-lookup-table-calt.png" alt="populating-the-lookup-name" width="50%" height="50%"/>  

27. In the box next to ‘Lookup Name’, you can either keep the default name or change it.  
a)  In this example I’m going to keep the name.  

28. Now go ahead and,  
a)  Click ‘OK’.  
    <img src="/assets/images/contextual/23-how-to-create-contextual-substitution-font.png" alt="saving-contextual-lookup-table" width="50%" height="50%"/>  

29. Now that we’ve added a contextual lookup table, the next step will be to add a corresponding subtable to it, just like we did in the previous steps.  

---

## Adding a Contextual Subtable  

30. Now we’ll be adding a subtable to our contextual lookup.  
a)  Click ‘Add Subtable’  

    <img src="/assets/images/contextual/24-how-to-create-contextual-substitution-font.png" alt="adding-calt-contextual-lookup-subtable" width="70%" height="70%"/>  

    b)  Click ‘OK’ to accept the default name, or rename it.  

    <img src="/assets/images/contextual/25-how-to-create-contextual-substitution-font.png" alt="default-name-in-fontforge-for-subtable" width="35%" height="35%"/>  

31. On the next dialogue box that pops up,  
a)  Select ‘By classes’, and ‘Single’,  
b)  Click ‘Next>’  

    <img src="/assets/images/contextual/26-how-to-create-contextual-substitution-font.png" alt="completing-the subtable-in-fontforge" width="40%" height="40%"/>  

    ### Bottom Section

32. For the next section, **be aware** the bottom container needs to be completed before the top container.  
    {: .tip}


33. First, we’re going to define the glyphs that will form the context class.  
a)  Type the word ‘`letters`’, or a name of your choosing, in the column on the left.  
b)  Then, in the right hand column, type in each glyph ‘`g s y`’, separated by a space, or use the drop down arrow to select the glyphs that represent the class you want substituted.  

    i.  The bottom section should look like this:  
    {: .blockquote}

		letters  |  g s y  

    <img src="/assets/images/contextual/27-how-to-create-contextual-substitution-font.png" alt="example-formula-bottom-section-of-calt-contextual-lookup-subtable" width="50%" height="50%"/>  

    ### Top Section

34. Now to create the rule in the top section,  
a)  click on '<New\>'  
b)  Type the word ‘`letters`’, which should auto populate as you type.  

    <img src="/assets/images/contextual/28-how-to-create-contextual-substitution-font.png" alt="example-formula-top-section-of-calt-contextual-lookup-subtable" width="50%" height="50%"/>  

    c)  Click on ‘Add Lookup’,  
    d)  then select ‘slant’,  

    <img src="/assets/images/contextual/29-how-to-create-contextual-substitution-rule-font.png" alt="adding-lookup-to-formula-top-section-of-calt-contextual-lookup-subtable" width="50%" height="50%"/>  

    e)  now type '`letters`' again, and  
    f)  click on ‘Add Lookup’ again, but this time select 'sc'.  
    <img src="/assets/images/contextual/30-how-to-create-contextual-substitution-rule-font.png" alt="completed-formula-top-section-of-calt-contextual-lookup-subtable" width="50%" height="50%"/>  

35. The contextual formula for the top container should look like this:  

		 letters @<slant> letters @<sc>  

    a)  Note that ‘spaces’ in the formula are inconsequential.  

36. The contextual formula means:  
	if any of the glyphs present in ‘letters’ is followed by any of the glyphs present in ‘letters’, apply the lookup ‘slant’ to the first glyph and apply the lookup ‘sc’ to the second glyph.  

37. Now click ‘OK’.  

    <img src="/assets/images/contextual/31-how-to-create-contextual-substitution-rule-font.png" alt="saving-contextual-lookup-table" width="50%" height="50%"/>  

38. Click ‘OK’ again to commit and save all of your lookup tables.  

    <img src="/assets/images/contextual/32-how-to-create-contextual-substitution-rule-font.png" alt="click-ok-save-all-tables-and-font-subtables" width="70%" height="70%"/>  

39. We have now finished completing our lookup tables and will move on to testing them.  

---

## Testing the Contextual Lookups  

40. To test your contextual lookups, start from ‘Font View’  
a)  Click on ‘Metrics>New Metrics Windows’  
b)  Type into the box and test whether your formula works or not.  
c)  De-select ‘calt’ by holding down ‘Ctrl’ on your keyboard, and left mouse click on the word ‘calt’.  

    <img src="/assets/images/contextual/33-how-to-test-contextual-substitution-rule.png" alt="review-and-testing-in-metrics-view-with-calt-contextual-lookup" width="70%" height="70%"/>  
    <img src="/assets/images/contextual/34-how-to-test-contextual-substitution-rule.png" alt="review-and-testing-in-metrics-view-without-calt-contextual-lookup" width="70%" height="70%"/>  

---

## Alternate Formula Examples  

41. Here are some alternate formulas to consider.  

	*Alternate Example 1*  

42. In this example, the two single substitution lookups stay the same.  

        slant
        sc

43. However the contextual lookup formula changes.  
a)  For example, the formula for the top part of the container is:  

	    letters letters @<sc>  

	b)  Note that ‘spaces’ in the formula don’t matter.  
    <img src="/assets/images/contextual/35-how-to-test-contextual-substitution-rule.png" alt="alternate-formula-examples-of-calt-contextual-lookups" width="50%" height="50%"/>  

44. The contextual formula means,  

	If two glyphs, from ‘letters’ appear consecutively, then replace the second glyph with ‘lookup @<sc\>’  

45. This is what it looks like when testing in ‘Metrics View’.  
    <img src="/assets/images/contextual/36-how-to-test-contextual-substitution-rule.png" alt="alternate-formula-examples-of-calt-contextual-lookups" width="70%" height="70%"/>  

	*Alternate Example 2*  

46. The next example changes both the top section of the contextual lookup formula and adds a line to the bottom section of the formula.  

47. The two single substitution lookups stay the same:  

        slant
        sc  

48. This is what the formula for the top section looks like:  

         g @<sc> letters @<slant>  

49. This is what will be added to the bottom section:  

        letters  |  s y  
        g  |  g    

	a)  Remember the bottom part needs to be completed before you can add the top formula.  

    <img src="/assets/images/contextual/37-how-to-test-formula-contextual-substitution-rule.png" alt="alternate-formula-examples-of-calt-contextual-lookups" width="50%" height="50%"/>  

50. The contextual formula means:  

	Replace g with ‘lookup @<sc\>’ if it’s followed by a glyph from ‘letters’, and if it is, then replace the glyph from letters with ‘lookup @<slant\>’.  


51. This is what it looks like when testing in ‘Metrics View’.  
a)  Remember to hold down Control (Ctrl) on your keyboard, then left mouse click on the word ‘calt’ to change between normal text and calt text.  

    <img src="/assets/images/contextual/38-how-to-test-formula-contextual-substitution.png" alt="testing-and-reviewing-alternate-formula-examples-of-calt-contextual-lookups" width="70%" height="70%"/>  
    <img src="/assets/images/contextual/39-how-to-test-formula-contextual-substitution-lookup.png" alt="testing-and-reviewing-alternate-formula-examples-of-calt-contextual-lookups" width="70%" height="70%"/>  

---

## It's Not Working  

52. Here are some solutions to the problems that I’ve encountered when completing contextual lookups.  

53. If it’s not working out correctly,  
a) Review your two ‘single substitution’ look up tables.  
b) Make sure lookup tables match what you’ve typed or match what you’ve included in your contextual formula top and bottom containers.  
c) Check spelling throughout.  
d) Start with small formulas so that you can identify what is and is not working.  
e) If you get a warning pop up asking ‘whether the glyphs you typed were intentional’, you need to save, quit, restart Fontforge and start again for the ‘Default Using Suffix’ button to work.  
f) 'Default Using Suffix' will never work if you've used Fontforge's 'Mass Glyph Rename' function. I've outlined the reasons why and what to do, to be able to use 'Default Using Suffix', [here].  

**Congratulations on making it to the end of this tutorial.**

If all went well, you now have a working contextual lookup and you can build a fully functional font using Fontforge.  

[here]: /how-to-chained-contextual-ligatures/#problems-completing-the-subtable