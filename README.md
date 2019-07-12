# Lab 1
## 0. Fork and clone

Before we begin, make sure to fork and clone this repository as we did yesterday:

  - Click the *Fork* button at the top right of the screen to make your own copy of the repository
  - Clone it as we did before:
  ```
  cd ~/Desktop
  git clone <YOUR-REPO-URL>
  cd y2s19-css2
  ```
  
## 1. Open the page

- Open `lab1.html` in your browser and take a look at it!

## 2. Add hover to your link!

- In `lab1_styles.css`, add a `hover` selector, so every link has a blue background color when you hover over it.
- Open `lab1.html` in your browser and see what happens!

## 3. Hover with IDs.
- In `lab1.html`, choose a specific paragraph, and give it an ID of `important_paragraph`.
- In `lab1_styles.css`, add a hover selector for  this paragraph. Hovering over this paragraph should make the background color yellow, and the text size 40 point.

*Hint: Check out the font-size attribute*

## 4. Hover with class selectors.
- Now, for the remaining paragraph elements on the page, add them to a class `less_important_paragraphs`.
- When you hover over any of the paragraphs in this class, make the font color blue.

## Bonus: Complex Hovering!
- Add a `<span>` element, right before the last paragraph in `lab1.html`, containing the text `What happens if you hover over me?`, with ID `span_cover`.
- Now, add an additional div in `lab1.html`, with ID `hidden_div`. This div should contain the last paragraph of text in your website. Make sure this is below the `<span>` element you previously created!
- Make sure you can see this text, if you open `lab1.html` in your browser!
- Select this div, by ID, and add the rule `display: none;`, as one of its rules in `lab1_styles.css`.
- Open `lab1.html` in your browser - does anything look different? 
- Add a rule in `lab1_styles.css` which says:
```
#span_cover:hover + #hidden_div {
    display: block;
}
```
- Open `lab1.html` in your browser - what does it look like now?
*Go on W3 to figure out how this rule works!*

# Lab 2
- to be continued

# Lab 3
## 1. Make some `@keyframes`
- In `bounce_styles.css`, make a `@keyframes` component called `bounce`, with 2 frames, at 0% and 100%.

- Make it so the element has 0 opacity in the first frame and is scaled down to 1/10th of its usual size (using the `transform: scale()`) property

- Make the element be full-size and have opacity 1 in the final frame (the one labelled 100%)

## 2. Animate the circle
- In the CSS selector for the `svg` tag, add in the `animation` property

- Make the ball bounce for 2 seconds
  - If you need a hint, look at the lecture slides [here](http://go.meet.sh/anim-lec) and the reference website [here](https://robots.thoughtbot.com/css-animation-for-beginners)

## 3. Make it bounce infinitely
- Use `animation-iteration-count` property, or use the shorthand
  - If using the shorthand, remember to put values for the properties you aren't setting
  - Again, for hints, look at the [reference website](https://robots.thoughtbot.com/css-animation-for-beginners)
