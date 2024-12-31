## Spinner Animation in CSS

This is a simple CSS spinner that rotates continuously. Below is the breakdown of the code:

### The `.spinner` class:
This class is applied to the HTML element (usually an empty `div`) to create the spinner. Here's what each property does:

1. **`border: 4px solid rgba(0, 0, 0, 0.1);`**
   - Sets a 4-pixel wide border with a light gray color (`rgba(0, 0, 0, 0.1)`). The `rgba` value gives the border a 10% opacity.
   - This creates the outer circular border of the spinner.

2. **`width: 36px;` and `height: 36px;`**
   - Defines the size of the spinner. The element will be 36px wide and 36px high, forming a square.

3. **`border-radius: 50%;`**
   - Makes the square element a perfect circle by rounding the corners with a `50%` border radius.

4. **`border-left-color: #09f;`**
   - Changes the color of only the left border of the circle to a bright blue (`#09f`).
   - This creates the effect where only one part of the border is colored, which will animate during the spinner's rotation.

5. **`animation: spin 1s ease infinite;`**
   - Applies the `spin` animation to the spinner.
   - The animation lasts for 1 second (`1s`), with an `ease` timing function (it starts slow, speeds up, and then slows down again).
   - The `infinite` keyword ensures the animation loops endlessly, making the spinner rotate continuously.

### The `@keyframes spin` animation:
This section defines the steps of the animation that make the spinner rotate.

1. **`@keyframes spin`**
   - This is where the animation is defined, with the name `spin`, which matches the name used in the `animation` property of the `.spinner` class.

2. **`0% { transform: rotate(0deg); }`**
   - At the start of the animation (0%), the spinner is in its original position with no rotation.
   - `transform: rotate(0deg)` means no rotation at the beginning.

3. **`100% { transform: rotate(360deg); }`**
   - At the end of the animation (100%), the spinner completes a full rotation of 360 degrees.
   - `transform: rotate(360deg)` applies a full rotation, making the spinner spin in a circle.

### Summary:
1. The spinner is a circle with a border that has only the left side colored.
2. The `spin` animation makes the spinner rotate, creating a continuous spinning effect.
3. Since only part of the border is colored, the rotation creates the visual effect of the spinner "moving."

This is a simple yet effective way to create a loading spinner purely with CSS, without the need for images or JavaScript.



