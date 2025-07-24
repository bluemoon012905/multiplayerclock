# EDH Clock - A Mobile-Friendly cEDH Chess Clock

A simple, mobile-first web application designed as a chess clock for Commander (EDH) and cEDH (Competitive Elder Dragon Highlander) Magic: The Gathering games. It features four player quadrants, configurable timers and colors, and priority-passing logic tailored for multiplayer games.

**Live Site:** [https://github.com/bluemoon012905/multiplayerclock](https://github.com/bluemoon012905/multiplayerclock)

![image](https://github.com/user-attachments/assets/63c25c0d-cd26-435a-b765-d74a2e103e3c)

## Features

*   **4 Player Quadrants:** Each player gets a dedicated, color-configurable quadrant.
*   **Full-Screen Experience:** Designed to take up the entire screen, especially on mobile in landscape mode.
*   **Intuitive Priority System:**
    *   Click your *active* quadrant to pass priority clockwise.
    *   Click any *inactive* quadrant (yours or an opponent's) to take/hold priority.
*   **Pause/Resume:** A central button to pause the active timer or resume the game.
*   **Configurable Timers:** Set the initial game time for all players.
*   **Customizable Colors:** Personalize the gradient colors for each player's quadrant.
*   **Persistent Settings:** Your timer and color preferences are saved in your browser's local storage.
*   **Mobile-First Design:** Optimized for touch input and responsive to various screen sizes.
*   **Fullscreen on Landscape:** Attempts to go fullscreen on mobile devices when in landscape orientation for a more immersive experience.
*   **Single HTML File:** Entire application is contained within a single `index.html` for easy deployment and use.

## How to Use

1.  **Open the Clock:** Navigate to [https://victorjulianir.github.io/EDH-Clock/](https://victorjulianir.github.io/EDH-Clock/) in your web browser (mobile or desktop).
2.  **Settings (⚙️ Icon):**
    *   Click the gear icon in the top-right corner.
    *   Adjust the "Initial Time (minutes)".
    *   Configure the start and end gradient colors for each player.
    *   Click "Apply & Reset". Your settings will be saved for future visits.
3.  **Starting the Game:**
    *   The game starts paused (pause button shows ▶️).
    *   Any player can click their quadrant to start their timer (this "takes priority"). Their quadrant will become active, and their timer will begin. The pause button will change to ⏸️.
    *   Alternatively, click the central ▶️ button to start Player 1's timer.
4.  **Gameplay:**
    *   **Passing Priority:** If your timer is ticking, click your quadrant again. Your timer stops, and the next player's timer (clockwise) starts.
    *   **Holding/Taking Priority:** If another player's timer is ticking (or no timer is ticking but the game isn't paused), click your quadrant. The current active timer stops, and your timer starts.
    *   **Long press:** Long press to eliminate a player. Can't be undone.
    *   **Pausing:** Click the central ⏸️ button to pause the active timer. Click ▶️ to resume.
5.  **Time Out:** If a player's time reaches 00:00, an alert will notify players. That player can no longer take priority.

## Development

This application is built with plain HTML, CSS, and JavaScript. No external frameworks or libraries are used (beyond standard browser APIs).

*   **`index.html`**: Contains all the markup, styling, and JavaScript logic.

### To Run Locally:

1.  Clone this repository or download `index.html`.
2.  Open `index.html` in any modern web browser.

## Contributing

Suggestions and contributions are welcome! Feel free to open an issue or submit a pull request.

Possible areas for future improvement:
*   Sound notifications for low time.
*   More advanced settings (e.g., increment per turn, add extra time).
*   Player name customization.
*   Different visual themes.

## License

This project is open source and available under the [MIT License]

## Acknowledgements

This project is a fork of the [EDH-Clock](https://github.com/VictorJuliani/EDH-Clock) by Victor Juliani.

---

*This clock was designed to enhance multiplayer EDH/cEDH game flow.*
