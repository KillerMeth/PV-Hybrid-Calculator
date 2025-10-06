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

---

## Features

- Appliance load calculation  
- Clamp meter load calculation  
- System recommendation (Battery, inverter sizing)  
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
- clamp meter load calculation
- system recommendation

## Usage
1. Navigate to Appliance Load Calculation
  - Enter details of your appliances (power rating, quantity)
  - The tool calculates total energy demand
2. Go to Clamp Calculation
  - Input clamp meter data
  - Estimate load
4. Go to System Recommendation
  - Based on load and site parameters
  - The tool suggests battery capacity, inverter rating

> ⚠️ _Note_: Be mindful of units (W, kW, Wh, etc.) and efficiencies (losses) when providing inputs.

## Project Structure

PV-Hybrid-Calculator\
├── index.html\
├── appliance-load-calculation.html\
├── clamp-load-calculation.html\
├── system-recommendation.html\
└── (possibly supporting JS, CSS files)
- `index.html` — entry / navigation page
- `appliance-load-calculation.html` — UI & logic for load estimation
- `clamp-load-calculation.html` — UI for clamp meter load calculations
- `system-recommendation.html` — UI for sizing recommendations

If there are JavaScript or CSS files, they are included/linked inside the HTML pages.

## Contributing

Contributions are welcome! Here are some ways you can help:
- Report bugs or issues
- Add input validation and error handling
- Improve UI/UX (styles, layouts, responsiveness)
- Add support for more system types (off-grid, AC coupling, hybrid modes)
- Enhance calculations (temperature effects, derating, real world losses)

Before submitting a pull request, please:
- Fork the repository
- Create a new branch (git checkout -b feature/YourFeature)
- Make your changes & test thoroughly
- Submit a PR with a clear description of what you did

## License

This project is licensed under the **Creative Commons Attribution-NonCommercial 4.0 International (CC BY-NC 4.0)** License.  
You are free to share and adapt the code **for non-commercial purposes**, as long as you **credit the author**.  
