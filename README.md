# hotwirebutton_red
HOTWIRE FULLY-CLICKABLE CTA

Goals
Tasked with creating a CTA that had fully clickable area, with the possible drawback that it might not render exactly everywhere. Fortunately, it renders very consistently across all clients on our support list. We even achieved some progressive enhancements capabilities using hover states as, though they are simply demonstrative and not implemented into campaigns yet.

How it works
The base for this code is combing two techniques: inline styling directly on the <a> tag plus a table based approach with conditional code for Outlook. The structure of the code began from a  border-based “Ghost CTA” hence why there are multiple tables which are necessary to force Outlook dimensions. The height of CTA images in the left and right cells are what forces the dimensions, these are crucial.

Implementation
Repurposing this code is just about as simple as changing the styling! There are some caveats however:
1.	What you change inline needs to be done to the Outlook conditional class as well
2.	If there are multiple copies of the (visually) same CTA you obviously do not need to have duplicates of the conditional
3.	Make sure if the CTA is visually different, make a new class name
4.	If you only want a padding based CTA, you’ll still need the images on either side of the copy to force the height or else Outlooks (desktop and web) are going to blow out – you can use any image as long as dimensions are hard coded, these simply add rounding
5.	Use padding to set dimensions of clickable area, I recommend leaving a fix pixels of vertical space for Outlook
