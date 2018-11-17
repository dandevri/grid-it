## 1. Incredibly Easy Layouts with CSS Grid
Explicit vs implicit grid. The browser will decide implicit.
Grid container, all direct children becomes item. Everything that's outside that container cannot be placed on that grid.
Image are inline, they have a bit of line-height so that why display block.
Fraction of the space.

## 2. Flexibility & The Fold – new possibilities with CSS Grid
We don't have control of the width of the viewvport.
We care about left and right, but what about bottom and top? That's where the 'fold' comes in.
'We have no idea where the fold is'. It's from news, things above the fold would apear in the newsstand.
Bottom is basically the 'fourth edge'. Viewport units make sure you can design for height.
Viewport is basically a box.

`max content` large as possibly but no larger then the content.

## 3. Responsive Mondrian
Peter Mondrian; get rid of ornaments, but still symmetrical.
auto-fit; browser decides the amount of tracks
Automatically one cell if you don't tell an item how bit it should be
Auto-flow dense; not in source order.

## 4. Internet Explorer + CSS Grid????
non-grid supported browsers, just one single column? Progressive enhancement.
Feature query; supports display grid

## 5. Flexbox vs. CSS Grid — Which is Better?
Does this replace flexbox? No, mix grid with flexbox etc.
* Flexbox lines up in one direction wrap etc. Flexbox only row.
* Grid two directions, thinks about both of them

Grid can overlap items, with flexbox you can not.

## 6. Innovative & Practical Graphic Design with CSS Grid
Simple layout for browsers that don't support grid, and then use supports to enhance.

## 7. CSS Grid like you are Jan Tschichold
You can transform on a whole grid to get some really interestinng layouts.
You can't style the grid, so you have to place an element on the grid and style that.
Transforms don't alter the painting. Writing-mode takes up space.

## 8. Obliterate Boxiness with CSS Shapes
Effects are dramatic and fallback is easy with css shapes.
Shape-outside; run the flow content.

## 9. Basics of CSS Grid: The Big Picture
Comes from CSS specification, the browser builders use this to implement features.
Level 1 specification, that's locked down.
* Grid container
* Grid items

Grid items need to be direct children. Doesn't matter what elements they are.
Level 2 might have a subgrid, you can pull a grid through the grandchildren.
For now you have to use nested grids.

* Every unit is a grid cell
* Grid area can be multiple cells
Every cell is a square.

Rows and columns are both tracks.
Grid-lines and gaps. You cannot put content in a grid gap.

Explicit grid also defines negative numbers, other way around.
Two different ways to target lines.

Implicit, the browser creates tracks for you.

Grid only lives in the CSS so it can't be styled. Doesn't exist in the dom.

## 10. Using Flexbox + CSS Grid Together: Easy Gallery Layout
Flexbox most of the time want to give items the full width (stretch) and with a grid
layout most of the time you don't want that. Grid is better suited for that.

Fallback layouts from grids is not really that hard.

## 11. Whitespace on The Web! — with CSS Grid
Grid is really great for using white space.
Management of white space is the best design tool. 
Having rows chnges everything. If you explicit create a grid you can manage the white space.

## 12. HTML Source Order and When There’s No CSS
What is the source order if there is not layout? You want to design the order
when no CSS is applied.
* Screen reader; there are also people who can see but have limited vision. Dyslexia.
* SEO
* Reader view; without css and javascript

Put something on the bottom in the source order but visually on the top of the page. So screen readers
get to the content first.

## Introduction to Resilient CSS – 1/7
New css that changes the way we do layout on the web.
Work with new features even if isn't fully supported. 
**Doesn't work matrix.**
The web doesn't work like a OS, you don't need a minimum software requirement. < progessive enhancement
Reader modes etc. Good HTML. 
It's ok to make the different experiences for different devices. 

## The Secrets of ‘Can I Use’ – 2/7 Resilient CSS
What browsers support which properties and values.
* CanIuse It's rare something is 100% 65% doesn't mean your users have it, only all users.
Use the settings to tailor them. Google Analytics with canIuse. Statscounter.
Also look at MDN web docs, they are more specific with values.

## How Browsers Handle Errors in CSS – 3/7 Resilient CSS
CSS is skipped, no errors. Browser ignores.
Every broweser renders fonts differently.
Functional languages and errors out. 
HTML / CSS are declarative. Makes them very robust.

## Unlocking the Power of CSS Overrides – 4/7 Resilient CSS
Ignoring is fine but sometimes you want to make adjustments for other browsers.
CSS overrides; will run the second line. The later line.
`margin auto` if you use display flex.
There is no need to keep other browsers hostage to wait for support in an older browser.

## The Magic of Feature Queries, Part 1 – 5/7 Resilient CSS
@supports; it's a conditional. Property values in conditional. You can use or statement.  
Figure out your source order first. You can test that with disabling the css. Strip the CSS.
What if google home, alexa whatever is going to read webpages, you want your HTML to be right.

## The Magic of Feature Queries, Part 2 – 6/7 Resilient CSS
Not syntax. Write code that's going to be used in all the browser and then the feature query.
Not all browsers understand feature queries. They will reject all the code.

## Making Your CSS Fail Excellently – 7/7 Resilient CSS
* Overrides
* Feature queries

But, how well does it fail? Don't use the property that all.
Or use another set of properties that achieve the same effect.

## Use Clip Path to Vary Your Designs on the Web
Websites are basically boxes, but in print design there are more shapes.
You can use clip path, images inside shapes.

## Overlap on the Web, Graphic Design Made Easy with CSS Grid
Grid lets us do layouts that overlap. Position absolute was the previous method, but that doesn't
take up any space in the flow of the document.
Place items inside the grid in the same area as others.

## Drop Caps on the Web Using Initial Letter
Catch people's eye to easily spot where text starts. We mostly use them for decoration on the web.
Not only for decoration but also to guide the user.
You want to put it into a feature query.

## Introduction to Viewport Units
Viewport the edges of the browser window. Or the glass on a smartphone.

## Cropping images with Object Fit
`object-fit` you want to constrain the aspect ratio. But sort of squishy width.

## Designing for A Viewport
On the web you have a frame. Poster is a frame but their are buildings around them.
Why is the static design tooling step necessary? Paper and pencil, sketch out and then go to the browser.
Plan out the page and then design in the browser. Layout needs to respond to all the 4 sides of the screen.
Framing; frame of the story. Wide shot, medium shot etc. 
Everybody tries to cram as much in the viewport, but embrace scrolling.

## Min & Max Content Sizing in CSS Grid — 1/3 Flexibility
Normally text is going to wrap with a width.
max-content; stertch out as long as it can be
min-content; length of longest word

## FR Units in CSS Grid — 2/3 Flexibility
Fraction, take space and splitting it up with everything that has fr.
Let the browser do the math, don't use percentages and decimals.

## MinMax in CSS Grid — 3/3 Flexibility
The way of web design is not 'pixel perfect' that we should measure. What if thing are not ideal?

## Hot metal : Pasteup :: Floats : CSS Grid
-

## CSS Grid Uncollapses Your Margins. What?
Margin collapsing, margin doesn't get multiplied.
Sometimes they don't collapse, when you set display grid.
Grid cell contains the margin box.

## The Firefox Shape Path Editor
Clip-path, clip the outer edges. 
CSS shapes affect the flow of content.

## Where is CSS4? When is it coming out?
CSS2 has selections.

There isn't one CSS3 document. Working group split it up into modules.
There are different modules for colors, text etc.
Working draft; most people start working with. Candidate recommendetion, it pretty much done.

## 9 Biggest Mistakes with CSS Grid
1. Grid doesn't replace flexbox or floats: all have use cases.
1. Using only percent for sizing: 
1. Don't need breakpoints: 
1. Confused by numbering: numbers refers to line not the tracks.
1. Always using 12 columns: 
1. Forget about rows: default is auto-height
1. Reaching for framework: starter-kits but not frameworks.
1. Waiting for IE11
1. Don't wait for permission to play or experiment: find an old poster and re-create

## What if CSS Grid Changes?
Materials, html css etc. > Tools, frameworks
Time to learn material is more valuable then the time to learn the tool.
