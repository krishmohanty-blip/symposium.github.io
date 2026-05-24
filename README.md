# symposium
How the Slider Works: The slider changes one angle's variable, and each dot's position is calculated using n * angle for the rotation factor. Sqrt n for the distance, and the program draws them one at a time for an animated effect. 

Variables & canvas: The variables store the current angle, the seed number you're on, and the size of the canvas.

Drawing each dot: For each seed, the code determines where to place it using the angle and seed number, then draws a small circle there. requestAnimationFrame means it draws one dot, waits for the next screen refresh, then draws the next, creating the growing animation instead of everything appearing at once.

Slider: The slider changes the angle variable, and calls restart(), which clears the black background and begins the dot loop from seed 0 again — resize does the same thing but also shrinks or grows the canvas to fit the new window size first.

Claude Code was used for support.
