# SignalLab — Interactive Digital Line Coding Visualizer

Explore digital communication and line coding through interactive waveform visualization. SignalLab is a browser-based learning tool that converts binary sequences into digital signal waveforms, helping students understand how different line coding techniques represent data during transmission.

**Live Demo:** [SignalLab](https://shadhinsahriar.github.io/SignalLab/)

**Developer:** [Sahriar Ekhlas](https://github.com/shadhinsahriar)

---

## Overview

SignalLab is an interactive digital communications platform designed to make digital line coding easier to understand through real-time waveform rendering, step-by-step signal transitions, and encoding rule explanations.

Instead of studying signal diagrams only from textbooks, users can enter a binary sequence, select a line coding technique, and observe how the signal changes over time.

The project combines a clean interface with a JavaScript-based encoding engine and an interactive HTML Canvas renderer to provide a hands-on learning experience for digital communication concepts.

## Key Features

### 1. Interactive Binary Input

- Enter a custom binary sequence containing `0`s and `1`s.
- Generate random binary sequences for experimentation.
- View the number of bits in the input.
- Update the waveform according to the selected sequence.

### 2. Multiple Line Coding Techniques

SignalLab supports the following encoding techniques:

| Category | Techniques |
|---|---|
| Unipolar and Polar NRZ | Unipolar NRZ, NRZ-L, NRZ-I |
| Return-to-Zero and Biphase | Polar RZ, Manchester, Differential Manchester |
| Multilevel and Ternary | Bipolar AMI, Pseudoternary, MLT-3 |
| Block and Multibit Encoding | 2B1Q, 8B6T |

Each technique represents binary data using its own signal levels, transition rules, and encoding conventions.

### 3. Real-Time Waveform Visualization

The waveform canvas displays the encoded signal graphically, making it easier to observe:

- Signal amplitude and voltage levels.
- Transitions between signal levels.
- Relationships between input bits and waveform segments.
- Differences between encoding techniques.
- The effect of encoding rules on the transmitted signal.

### 4. Step-by-Step Signal Analysis

Explore the encoding process at your own pace with interactive playback controls.

- **Play/Pause:** Start or stop waveform animation.
- **Next Step:** Advance through the encoding sequence.
- **Previous Step:** Review an earlier step.
- **Restart:** Restart the waveform animation.
- **Show Full:** Display the complete waveform.

These controls help users connect individual bits with their corresponding signal transitions.

### 5. Playback Speed Control

Choose from five playback speeds:

- 0.2×
- 0.5×
- 1.0×
- 1.5×
- 2.0×

Slower playback is useful for studying individual transitions, while faster playback helps visualize the overall signal pattern.

### 6. Interactive Canvas Controls

The waveform canvas includes several tools for examining signals:

- **Zoom In / Zoom Out:** Adjust the waveform's viewing scale.
- **Pan:** Move around the canvas by dragging.
- **Reset View:** Restore the default viewport.
- **Grid Toggle:** Show or hide the waveform grid.
- **Dual Trace:** Toggle the additional baseline trace where supported.
- **Hover Inspection:** Inspect waveform steps using contextual tooltips.

### 7. Encoding Convention Configuration

Some encoding techniques support configurable mapping conventions or initial signal states.

SignalLab provides dynamic configuration controls for the selected technique, helping users understand how different conventions can affect the resulting waveform.

### 8. Signal Memory Helper

The Signal Memory Helper displays a short encoding rule or reminder associated with the active technique.

This feature is designed to help students quickly recall important transition rules while analyzing waveforms.

### 9. Encoding Engine Diagnostics

The application includes an engine diagnostic feature that runs built-in checks on encoding behavior.

Users can rerun the available checks to verify the behavior covered by the project's diagnostic suite.

---

## Technologies Used

| Technology | Purpose |
|---|---|
| HTML5 | Web page structure and interface elements |
| CSS3 | Layout, styling, gradients, and visual effects |
| JavaScript (ES6+) | Encoding logic, animation, and interactivity |
| HTML Canvas API | Dynamic waveform rendering |
| Tailwind CSS | Utility-based interface styling |
| Lucide | Interface icons |
| Google Fonts | Inter and Fira Code typography |
| GitHub Pages | Static website hosting |

SignalLab uses a lightweight, single-page architecture. The encoding engine and waveform renderer run in the user's browser without requiring a separate application server.

## How It Works

SignalLab processes binary input through a sequence of steps:

1. **Input:** The user enters a binary sequence.
2. **Selection:** The user chooses a line coding technique.
3. **Encoding:** The JavaScript encoding engine applies the selected technique's rules.
4. **Waveform generation:** The encoded signal data is passed to the waveform renderer.
5. **Visualization:** The canvas displays the signal levels and transitions.
6. **Exploration:** The user inspects the waveform using playback, zoom, pan, and step controls.

This process allows users to explore how digital data is represented as physical-layer signals.

## Getting Started

### Use the Live Website

The simplest way to explore SignalLab is to visit:

**[https://shadhinsahriar.github.io/SignalLab/](https://shadhinsahriar.github.io/SignalLab/)**

No installation is required.

### Run Locally

**Prerequisites**

- A modern web browser.
- Git (optional, for cloning the repository).
- An internet connection for the external CDN resources used by the interface.

**Option 1: Download the project**

1. Open the [SignalLab repository](https://github.com/shadhinsahriar/SignalLab).
2. Download the source code as a ZIP file.
3. Extract the downloaded archive.
4. Open the main HTML file in a modern browser.

**Option 2: Clone the repository**

Open a terminal and run:

```bash
git clone https://github.com/shadhinsahriar/SignalLab.git
cd SignalLab
```

Open the main HTML file in your browser.

Alternatively, use Visual Studio Code with the Live Server extension for convenient local development.

No package installation or build process is required for the current single-page implementation.

## Deployment

SignalLab is hosted using GitHub Pages.

To publish your own changes:

1. Push the website files to the GitHub repository.
2. Open the repository's **Settings**.
3. Navigate to **Pages**.
4. Under **Build and deployment**, select **Deploy from a branch**.
5. Select the `main` branch and the `/ (root)` folder.
6. Save the configuration and wait for deployment to complete.

Ensure the published root directory contains an `index.html` file so GitHub Pages can serve the website at the project URL.

Once deployed, the website will be accessible at:

`https://shadhinsahriar.github.io/SignalLab/`

For further information, see the [GitHub Pages documentation](https://docs.github.com/en/pages).

## Project Structure

The project uses a single-page website architecture.

```text
SignalLab/
├── index.html       # Website structure, styles, and JavaScript
└── README.md        # Project documentation
```

The structure above describes the intended minimal deployment layout. If the repository contains additional files, they can remain in their existing locations.

## Who Is This Project For?

SignalLab is useful for:

- Computer Science and Engineering students.
- Students studying Data Communications and Computer Networks.
- Learners exploring digital-to-digital signal encoding.
- Anyone who wants to visualize binary signal transitions interactively.
- Educators looking for a browser-based demonstration tool.

## Learning Objectives

By exploring SignalLab, users can develop a better understanding of:

- Digital line coding and signal representation.
- The relationship between binary data and signal levels.
- Transition-based encoding rules.
- Multilevel and multitransition signaling.
- Differences between common line coding schemes.
- The role of signal visualization in digital communications.

## Limitations

- The visualizations are educational simulations, not measurements from physical transmission hardware.
- Actual signal characteristics depend on the transmission system and its implementation.
- The website relies on external CDN resources for some styling, icons, and fonts.
- Encoding conventions may vary between standards and implementations; users should consult the relevant standard when exact interoperability is required.

## Future Improvements

Potential future enhancements include:

- Exporting waveform diagrams as images.
- Adding side-by-side comparisons of encoding schemes.
- Providing more detailed bit-by-bit explanations.
- Expanding encoding examples and educational reference material.
- Improving accessibility and keyboard navigation.
- Adding additional diagnostic cases and automated validation.

## Author

**Sahriar Ekhlas**

GitHub: [@shadhinsahriar](https://github.com/shadhinsahriar)

Live Project: [SignalLab](https://shadhinsahriar.github.io/SignalLab/)

## Acknowledgements

SignalLab is built with standard web technologies and open-source frontend resources, including Tailwind CSS and Lucide.

---

*SignalLab — Making digital line coding easier to visualize, explore, and understand.*
