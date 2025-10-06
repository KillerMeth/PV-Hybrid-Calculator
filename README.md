# PV-Hybrid-Calculator

**PV-Hybrid-Calculator** is a web-based tool to help design and evaluate hybrid (solar + grid / battery) photovoltaic (PV) systems. It provides calculations for appliance loads, PV sizing, system recommendations, and more.

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
