CSS SECTIONING
=========

=============================================

CSS Sectioning is a term I (the author) use to describe the application of specific sections to a web page.  In practice, sectioning helps to organize content and make it more readable for the user.  Web traffic from mobile devices is increasing every day, and sectioning is a common practice among developers to support mobile integration.  In this overview, I will discuss:

  - Sectioning 'gotchas'
  - Things to look out for
  - Tips for implementing sectioning into your development project


GOTCHAS, TIPS, AND LINKS
-------------------
'In programming, a gotcha is a feature of a system, a program or a programming language that works in the way it is documented but is counter-intuitive and almost invites mistakes because it is both enticingly easy to invoke and completely unexpected and/or unreasonable in its outcome.' - WIKIPEDIA

When designing a web app in CSS, there are several 'gotchas' that fit this definition perfectly.  Here are five you should be aware of:

1. IMAGE RESOLUTION -   When considering the use of a background image, you may think that any image you pull off the web will work because CSS allows you to resize it.  This is a trap, however, because computers are increasingly being built with higher resolution screens that can easily highlight image blur.

    TIP: When searching Google Images, click "search tools", then "size", and select an image resolution of 2MP or higher. This will accomodate even retina screens on the new Macbooks.

    HELPFUL LINK: http://css-tricks.com/perfect-full-page-background-image/
    
2. LAYERING - Many of us grew up with drag and drop functionality using tools like Microsoft Word.  Being used to this kind of functionality can make CSS very frustrating, as layering can be one of the most counterintuititve processes to master.  The most important thing to remember when trying to layer one div on top of another is that positioning and z-index are your best friends.  If you neglect to take parent divs into consideration, that will also get you into trouble.
    
    TIP: Follow these steps when attempting to layer divs in CSS.  First, identify any parent divs related to those you wish to layer.  Once you find them, make sure they are given the attribute of 'position: relative' in CSS.  From there, the div you wish to layer on top will have the attribute 'position: absolute' and a z-index higher than the div you wish to place it on top of.

    HELPFUL LINK: http://css-tricks.com/almanac/properties/z/z-index/

3. SIZING - One 'gotcha' you want to be aware of is the trap of 100% height.  When attempting to make multiple sections on a single page, no single section can have 100% height because CSS will take that to mean you want the individual section to fill the entire page.  In other words, CSS does not know that you want to fill 100% of that specific section (unless the section is within a parent div that has already been pre-sized).
    
    TIP: Size your section height using 'em' measurements, rather than pixels or percentages.  If you wish to have 100% width, simply writing 'width: 100%' will size your section appropriately.  If you absolutely insist on using 100% height, perhaps because want your website to be responsive, here is a link that may help you avoid the problems mentioned above:

    HELPFUL LINK: http://www.mattboldt.com/css-100-percent-height/
    
4. UNORGANIZED WORKFLOW: Given the design-focus of CSS, it's easy to fall into the trap of designing the most important or design-heavy sections first.  Depending on your specific project, this may even mean designing the footer first.  This practice, however, can lead to many struggles down the road.  Layering in particular can be very difficult, as you may struggle to keep track of z-indexes and position attributes while bouncing around from one section to another.

    TIP: Use the 'top-down approach".  Top-down is a best practice used by many front-end developers to organize and prioritize their workflow.  Rather than bouncing around from section to section, following the top-down approach means literally starting at the top of your web page and working your way down.  You cannot move to the next section until a working model is in place.  This is a great practice, because failing to follow this model can lead to tremendous struggles down the line with layering, margins, and padding. 
    
5. DIVIDERS - Perhaps one of the most important aspects of CSS Sectioning is to make sure that your page sections are clearly defined.  Defined sections make it easy for users to organize information, and also have the added bonus of helping you to organize content as you move through a project. Whether you organize sections by divider lines, background colors, or images, it's an important practice that you should adopt right away.

    TIP: Flat design is trending right now, so try dividing your sections by color rather than divider lines.  If you do use a divider line, make sure that the hr element is on it's own line and not a part of your parent div.  This will make it easier to span the full width of the page.
    
    HELPFUL LINK: http://css-tricks.com/simple-styles-for-horizontal-rules/