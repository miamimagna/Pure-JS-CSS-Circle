# Circle-PureJS-RWD
This project demonstrates how to create a rotating div element around the center of the page using HTML, CSS, and JavaScript. The rotation is achieved using geometric formulas, ensuring the effect is responsive and adjusts to different screen sizes.

## Table of Contents
- [Demo](https://github.com/miamimagna/Pure-JS-CSS-Circle/blob/main/README.md#demo)
- [Features](https://github.com/miamimagna/Pure-JS-CSS-Circle/blob/main/README.md#features)
- [Usage](https://github.com/miamimagna/Pure-JS-CSS-Circle/blob/main/README.md#usage)
- [Code Explanation](https://github.com/miamimagna/Pure-JS-CSS-Circle/blob/main/README.md#code-explanation)
- [Contributing](https://github.com/miamimagna/Pure-JS-CSS-Circle/blob/main/README.md#contributing)

## Demo
[here](https://miamimagna.github.io/Pure-JS-CSS-Circle/)

## Features
- Pure JavaScript: No external libraries required.
- Responsive Design: Utilizes vh and vw units for adaptive layout.
- Smooth Animation: Continuous and smooth rotation effect.(currently implementing!!! will do soon)
- Interactive Controls: Start and stop buttons to control the rotation.
## Usage
To use this project, simply clone the repository and open the index.html file in your browser.

```
git clone https://github.com/miamimagna/Circle-PureJS-RWD.git
cd Circle-PureJS-RWD
open index.html
```
## Code Explanation
### Key Highlight: 
This code is entirely written without any use of AI at all! No one can verify it but you can understand that by the structure of code.
- The html provides three buttons that have following functionality:
- `start`: this is to start the circular motion of the div using geometric equation of circle:
    `x^2 + y^2 = r^2`
- `start-smooth`: this one was to simulate same circular motion using simple trigonometric equations:
    ```
    x = x' + r * sin(O)
    y = y' + r * cos(O)
    ```
- **Responsive Web Design**: You can run code on any screen size and it will have same funcitonality
- **Browser compatibility**: Due to only usage of `setInterval` and `Math` library, this code can run on any browser that has javascript enabled(although flexbox support is still an issue but it will still work without it too!)
### HTML
Html used here is pretty basic, we have used a `div#all` to define the actual circular path on which the `div#container` will move.
### CSS
Now this is longest part of the code... salient features of CSS are:
- every metric is in viewport width and height units, hence it can be easily run in any screen size.
- Rest of CSS is just there to make it look vibrant and self-explanatory.
- **Note**: actually we could've used `transform` property to obtain smooth motion but that is advanced CSS property and We wanted to implement this in as simple manner as possible
### JavaScript
JavaScript used is actually the reason this project is possible:
- x and y are actually calculated using equation of circle using basic elementary mathematics!!!
- **Note**: right now we are trying to implement the same code using `sin` and `cos` function for smoother motion!!!
## Contributing
Contributions are welcome! If you have any improvements or suggestions, feel free to create an issue or submit a pull request.

- Fork the repository
- Create your feature branch (`git checkout -b feature/your-feature`)
- Commit your changes (`git commit -m 'Add your feature'`)
- Push to the branch (`git push origin feature/your-feature`)
- Open a pull request
