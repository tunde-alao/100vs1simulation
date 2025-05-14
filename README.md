# 100 Men vs 1 Gorilla Simulation

A 3D battle simulation that visualizes the hypothetical scenario of 100 men fighting against a single gorilla.

## Description

This project simulates a battle between 100 coordinated men and a single gorilla using Three.js for 3D visualization. The simulation implements strategic group behavior for the men and realistic battle mechanics.

## How to Run the Simulator

### Prerequisites

- A modern web browser (Chrome, Firefox, Safari, or Edge)
- The project files:
  - `simulator.html`: The main simulation file
  - `gorilla.glb`: 3D model for the gorilla
  - `human.glb`: 3D model for the humans

### Instructions

**Important**: Due to browser security restrictions (CORS policies), directly opening the HTML file may not work correctly when loading the 3D models. Instead, you should use a local web server to serve the files.

#### Method 1: Using Python (Recommended)

If you have Python installed (most macOS and Linux systems have it pre-installed):

1. Open a terminal or command prompt
2. Navigate to the directory containing the simulation files:
   ```
   cd path/to/100vs1simulation
   ```
3. Start a simple HTTP server:
   - For Python 3:
     ```
     python -m http.server
     ```
   - For Python 2 (legacy):
     ```
     python -m SimpleHTTPServer
     ```
4. Open your browser and navigate to:
   ```
   http://localhost:8000/simulator.html
   ```

#### Method 2: Direct File Opening (May not work properly)

1. Make sure you have all the required files in the same directory
2. Open the `simulator.html` file in your web browser:
   - Double-click the file to open it with your default browser
   - Alternatively, right-click the file and select "Open with" to choose your preferred browser
   - You can also drag and drop the file into an open browser window

#### Once Running

1. When the simulation loads, click the "Start Simulation" button to begin
2. Use your mouse to interact with the 3D scene:
   - Left-click and drag to rotate the camera
   - Right-click and drag to pan
   - Scroll wheel to zoom in and out

### Simulation Controls

- The simulation starts automatically after clicking the "Start Simulation" button
- Health bars at the top left show the remaining health of both the gorilla and the men
- Statistics at the top right show the remaining men and elapsed time
- The simulation ends when either the gorilla or all men are defeated
- Click "Restart Simulation" to run the simulation again

## Simulation Parameters

The simulation uses the following parameters which can be modified in the code:

- Gorilla health: 1000
- Man health: 10
- Gorilla attack damage: 20
- Man attack damage: 2
- Gorilla attack radius: 10
- Man attack range: 5
- Coordination bonus for men: 1.5x damage when attacking in groups

## Notes

- The men employ group tactics and coordinate their attacks
- The gorilla has greater strength but is outnumbered
- The outcome may vary each time you run the simulation
