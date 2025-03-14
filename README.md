# Hardware Visualization

## Overview
This project is part of the **Hardware Security Lab at UNC**, focused on developing a **hardware security visualization tool** to analyze **symbolic execution** and **hyperflow graphs** of Verilog RTL designs. The goal is to create an intuitive interface for visualizing execution paths and exploring security vulnerabilities in hardware systems, making complex verification tasks more accessible and efficient. This is a work in progress.

This tool is aimed to integrate with **[SEIF](https://dl.acm.org/doi/10.1145/3623652.3623666) and [SYLVIA](https://repositum.tuwien.at/handle/20.500.12708/188806)**, two symbolic execution frameworks, to enhance hardware security analysis by mitigating path explosion problems and improving execution efficiency.

## Technologies to be Used
### **Frontend**
- **React.js and React Router**

### **Backend**
- **Express.js** - To manage API endpoints for file uploads and processing.
- **FastAPI** - Built on top of Seif and Sylvia to process incoming files
- **PostgreSQL with neon.tech** - To store execution logs and user files.

### **Visualization & Processing**
- **Cytoscape.js / Recharts.js** - To visualize execution flow dynamically.
- **NetworkX, Graphviz, PyViz** - Python libraries for visualizing graphs
- **WebAssembly (Future consideration)** - To run Verilog analysis efficiently in the browser.
- **SMT Solvers (Z3, Boolector, etc.)** - To handle symbolic execution computations.

## Features
- **Upload Verilog Files** - Users can upload Verilog RTL files for processing.
- **Symbolic Execution Visualization** - Displays execution paths in a clear, structured format.
- **Security Flow Analysis** - Helps identify vulnerabilities in hardware designs.
- **Modern UI Design** - Clean, professional layout inspired by industry standards.

## Direction & Future Enhancements
- **Integration with SEIF and SYLVIA** - Enhancing symbolic execution capabilities for improved security analysis.
- **Iteractive UI for hyperflow graphs and paths in symbolic execution**

## Setup & Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo/hardware-visualization.git
   cd hardware-visualization
   ```
2. Install dependencies:
   ```bash
   cd frontend
   npm install
   cd ../backend
   npm install
   ```
3. Run the application's frontend and backend:
   ```bash
   cd ../frontend
   npm run dev
    ```
    in a new terminal
    ```bash
    cd backend
    node server.js
    ```
**Note:** The sylvia and seif API is not avalible to use right now but will be deployed soon. Also, accesing the database is not possible for extenernal users. This will all be avalible once deployed on OKD.

## Contribution
This project is actively evolving, and feedback on UI improvements, backend optimizations, and new visualization techniques is encouraged.
