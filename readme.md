# A2_SwissPoster

# Setup

You can visit this site at any time here on [glitch.](https://pruitt-a2-swissposter.glitch.me)
Move your mouse over the big words to see a surprise!
(This works on mobile as well yay! – Touch each word for the same effect.)

If you want to run the project locally, follow the steps below:

1. Clone this github folder to your preferred location on your computer. 
2. Use the Terminal to cd to this project. 
3. Start a local server using the command: ```python -m SimpleHTTPServer```
4. Go to your browser and type: ```http://localhost:8000```

# Assignment

For this assignment we drew inspiration from the grid-like graphic percision of Swiss poster design. Our task was to reverse engineer an existing design and implement it for the web.

I wanted to choose a poster that was graphically interesting but not too complicated. For my first attempt at CSS styling, it was important to me that I could feasibly go through all the motions of analyzing a design, recreating it for the web, and then adding some programmatic flair.

## Design

By bringing the original poster into Adobe Illustrator, I could use guides to figure out the sizing and spacing of elements. 
![picture of original poster with guide lines](https://github.com/mayapruitt/A2_SwissPoster/blob/master/documentation/original_reverseEngineering.png)

I created a few designs of my own that remixed the original. Since the OG poster advertises some sort of event, I decided to include the same kind of content for mine.

![valentines day design](https://github.com/mayapruitt/A2_SwissPoster/blob/master/documentation/valentines_idea.png)

I've been interning at the Museum of Natural History creating interactive media for the upcoming [special exhibition](https://www.amnh.org/exhibitions/color) on ***color***. I felt like this lent itself well to the poster design and would allow for cool interactivity later. I wanted to highlight two types of color schemes and have them shift with a mouse over event.
- Analogous = colors adjacent on the color wheel 
- Compound = a color and the two colors adjacent to its compliment  

![analogous](https://github.com/mayapruitt/A2_SwissPoster/blob/master/documentation/swiss_poster-03.png)

## Style Guide
From there I created a style guide, trying to match the original font and color palette. 


![style guide](https://github.com/mayapruitt/A2_SwissPoster/blob/master/documentation/style_guide.png)

# Building the HTML

Having the design planned out made it a lot easier to begin the HTML process. I started by putting all the content on the page, figuring out how to structure it. This was a bit challenging at first for it wasn't always staight forward what child objects needed parents or how nested elements needed to be until styling was applied. I found myself having to change what divs were inside other divs a few times until it seemed to work correctly. 

Once the structure was in place, styling became mostly trial and error. I feel like though I had reverse engineered a grid like structure, I wasn't always sure how to put it in place programatically. Thus, a lot of adjustments became "moving by eye". Any advice for this?

## Struggles 

I had the hardest time adjusting the vertical position of the large header text. I finally solved this with [Tania's advice](https://www.taniarascia.com/overview-of-css-concepts/) of making the parent div ```position: relative``` and the child div ```position: absolute.```

Moving forward I still have questions about making layouts more responsive. The smaller font sections would also probably benefit from a stacked orientation if you make the window width narrower, so I attempted to use ```@media``` and ```flex-direction: column``` but didn't see any visual changes. However, I only wanted this to change if you make a browswer window on the computer narrower. It actually looks really nice on mobile just the way it is. 

However, is it possible to lock the vertical positioning of elements in place even if the window width is expanded? I got the header text to be responsive in that it will always take up the whole width of the window, but it moves around vertically more than I would like. 

# Deploying to Glitch.com
1. Make sure the git repo is public
2. Make sure the git repo is up to date
3. Copy the repo link
4. Create a new project on glitch
5. Open "Tools" --> "Git, Import, and Export"
6. Click "Import from Github", pase the repo link
7. Press "ok" and watch your code magically appear!

# References
- [Css hover events](https://www.opinions.co.il/ogdan/css-hover-element-affect-another/)
- [Justifying content](https://css-tricks.com/almanac/properties/j/justify-content/)
- [Javascript events](https://github.com/itp-dwd/2020-spring/blob/master/guides/javascript-frontend-guide.md#javascript-events)
- [Swiss poster generator](https://mocoloco.com/swiss-poster-generator-by-ben-and-clark-duvall/)
- [Markdown cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)

# Author 
Maya Pruitt