# PV-Hybrid-Calculator

**PV-Hybrid-Calculator** is a web-based tool to help design and evaluate hybrid (solar + grid / battery) photovoltaic (PV) systems. It provides calculations for appliance loads, system recommendations, and more.

---

## Table of Contents

- [Features](#features)  
- [Getting Started](#getting-started)  
  - [Prerequisites](#prerequisites)  
  - [Installation](#installation)  
  - [Running Locally](#running-locally)  
- [Usage](#usage)  
- [Project Structure](#project-structure)  
- [Contributing](#contributing)  
- [License](#license)  
- [Acknowledgements](#acknowledgements)

---

## Features

- Appliance load calculation  
- Clamp (or inverter / DC-DC) load calculation  
- System recommendation (PV panel, battery, inverter sizing)  
- Interactive web interface (HTML / client side)  
- Modular design (so you can extend or customize calculations)

---

## Getting Started

These instructions will help you set up and run the project on your local machine for development and testing.

### Prerequisites

Since the project appears to be HTML + client-side logic (JS), you don’t need a heavy backend. But for development you’ll want:

- A modern browser (Chrome, Firefox, Edge, etc.)  
- (Optional) A local HTTP server (so that local file restrictions don’t block scripts)  
- (Optional) A text editor or IDE (VS Code, Sublime, etc.)

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/KillerMeth/PV-Hybrid-Calculator.git
   cd PV-Hybrid-Calculator

2. (Optional) If you want to host it via a simple HTTP server, you can use e.g.:
  ```bash
   # with Python 3
    python3 -m http.server 8000
  ````
### Running Locally

If you’re not using a server, you can just open index.html in your browser (depending on browser security settings).
If using a local HTTP server, open in browser:
````bash
http://localhost:8000/index.html
````
From there, you should see the UI that lets you navigate to:
- appliance load calculation
- clamp / inverter load calculation
- system recommendation

### Usage
1. Navigate to Appliance Load Calculation
  - Enter details of your appliances (power rating, hours of use, quantity)
  - The tool calculates total daily energy demand
2. Go to Clamp / Load Calculation
  - Input inverter or DC component data
  - Estimate DC load or conversion losses
4. Go to System Recommendation
  - Based on load and site parameters (solar irradiance, battery efficiency, etc.)
  - The tool suggests PV panel sizing, battery capacity, inverter rating

> ⚠️ _Note_: Be mindful of units (W, kW, Wh, etc.) and efficiencies (losses) when providing inputs.

### Project Structure

pgsl

PV-Hybrid-Calculator/
├── index.html
├── appliance-load-calculation.html
├── clamp-load-calculation.html
├── system-recommendation.html
└── (possibly supporting JS, CSS files)
