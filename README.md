##FEATURES:##
1. table-based, modular HTML email optimized for Gmail App and iOS Apple Mail App
2. no media queries; width of 600px
3. use of rems and ems so that each module can be resized independently
4. thoroughly-documented, validated code
5. CSS fix for superscript HTML entities (&reg;) -- line-height distortion is anticipated, eliminated
6. Absolute paths to hosted images (social icons, etc)
7. Thoroughly-tested on desktop (Gmail and Thunderbird in Chrome, Edge, FireFox, Internet Explorer 11) and mobile (Gmail app, iOS Mail app)
8. Includes an HTML snippet that fixes Gmail's attempt to automatically resize fonts. A discussion of this can be found [here](http://freshinbox.com/blog/gmail-on-ios-increases-font-size-on-some-emails/). The code is included just before the closing body tag.


##DIFFERENCES BETWEEN BUILD AND PSD:##
1. exact design ratios not possible:
  * Gmail does not support media queries, so compromises to layout had to be made
  * The original PSDs do not adhere to the convention of not exceeding a width of [approx.] 600px
2. button size increased in order to increase usability in small viewports
3. added underlined phone numbers that trigger the phone application, for increased usability
4. when the content of the "quad section" (the area with the gray background) exceeds a certain word-count, the 4 black squares no longer adhere to the desired design ratio.
5. A different font has been used for the HTML build since only a limited number of fonts are suggested for HTML email


##POSSIBLE FUTURE ISSUES:##
1. The email template will break in Gmail if the HTML dash entity is used in the markup.
2. I initially sized the social icons in the footer with a height and width property (in ems), but ultimately eliminated the height property and switched to pixels...this resolved an inconsistency in how the iOS Mail app was displaying these images.
3. The Gmail auto resize feature (a.k.a. "nightmare") was initially resolved by implementing the HTML snippet mentioned above. However, further testing shows that the results are inconsistent. The initial test with Sendmetric will sometimes show the snippet to be ineffective...but a second test (sent immediately after the first) will display properly, even when no code has been updated. I'm still not sure what's causing this issue.


##REQUIRED ACTIONS:##
1. put all CSS inline
2. update placeholders with content, e.g. [AP Time] and [Customer Name]
3. test again after updating any content, images, or links
