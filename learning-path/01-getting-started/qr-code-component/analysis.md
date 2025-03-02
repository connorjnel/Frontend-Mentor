# Project Name

QR Code Component

## Requirements

- Create QR code component, desktop and mobile version
- Design is static, not reponsive
- Has design doc with custom colors and font size as well as font family
- Test for all screen sizes
- Confirm final design against screenshot provided
- Confirm colours, font sizes, fonts, spacing against provided figma file
- Take screenshot of final design

## Extra challenges

- Use semantic HTML
- Pixel perfect design

## Libraries, Components

- HTML
- CSS

## Analysis

Basic QR Code component with fixed size, no responsive needed so just center it vertically and horizontally.  Viewports used are 1440px for desktop and 375px for mobile. Component size is 320px by 499px regardless of viewport size.  Has a fixed background color.  Component itself is basically a card with border-radius, static qr image with text below.  QR image also has border radius, might have a drop shadow but not sure to be honest. Check style guide for colors, body font size, font as well figma for the padding values

## Notes

- Style setup copying color values from style-guide.md to style.css, also copying the padding and font etc from figma to css variables
- Changed colours to hex, personal preference, kept same var names as style guide.
- Super important, built in VSCODE translate to hex had different result that style in guide in pixel, used those hex values instead
- Updated font from google fonts, also edited link in index.html
- Did most of the css already since its mainly globals from style docs, now writing the html
- Had minor issue with qr image having a 16px spacing at bottom stacking above the text block, changing font size of figure class resolved, could be because its expecting a figcaption?
- May be smart to move figure into article and add the text as a figcaption instead of current which is section, figure, article
