# AI Data Analysis Agent

A Python-based AI agent that leverages large language models (LLMs) to automate and enhance data analysis workflows. It is designed to help users extract insights, generate summaries, and visualize data with minimal manual effort.

---

## Table of Contents

- [Features](#features)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [Usage](#usage)
  - [Command-Line Arguments](#command-line-arguments)
  - [Example Workflow](#example-workflow)
- [Configuration](#configuration)
- [Project Structure](#project-structure)
- [Extending the Agent](#extending-the-agent)
- [Troubleshooting](#troubleshooting)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgements](#acknowledgements)

---

## Features

- **Automated Data Analysis:** Uses LLMs to interpret and analyze tabular data.
- **Multi-format Support:** Handles CSV and Excel files out of the box.
- **Insight Generation:** Summarizes datasets, highlights trends, and detects anomalies.
- **Visualization:** Automatically generates charts and graphs for key findings.
- **Interactive Q&A:** Users can ask questions about their data in natural language.
- **Extensible:** Easily add new analysis modules or integrate with other tools.

---

---

## Getting Started

### Prerequisites

- Python 3.8 or higher
- `pip` (Python package manager)
- (Optional) [virtualenv](https://virtualenv.pypa.io/en/latest/) for isolated environments

### Installation

1. **Clone the repository:**
   ```sh
   git clone https://github.com/Yavic2024/ai-data-analyst.git
   ```

2. **Install dependencies:**
   ```sh
   pip install -r requirements.txt
   ```

3. **(Optional) Set up environment variables:**
   - If your LLM provider requires an API key, create a `.env` file:
     ```
     OPENAI_API_KEY=your-api-key-here
     ```

---

## Usage

### Command-Line Arguments

| Argument         | Description                                 | Example                |
|------------------|---------------------------------------------|------------------------|
| `--input`        | Path to the input data file (CSV/Excel)     | `--input data.csv`     |
| `--output`       | Path to save analysis results (optional)    | `--output results.txt` |
| `--visualize`    | Generate visualizations (optional flag)     | `--visualize`          |
| `--model`        | Specify LLM model (optional)                | `--model gpt-4`        |

### Example Workflow

1. **Basic Analysis:**
   ```sh
   python ai_data_analyst.py --input sales_data.csv
   ```

2. **With Visualization and Output File:**
   ```sh
   python ai_data_analyst.py --input sales_data.csv --visualize --output summary.txt
   ```

3. **Interactive Q&A:**
   After running the script, type your questions (e.g., "What are the top 3 products by revenue?").

---

## Configuration

- **Model Settings:** Edit `ai_data_analyst.py` to change the LLM provider, model name, or prompt templates.
- **API Keys:** Store sensitive keys in a `.env` file or set as environment variables.
- **Visualization:** Customize chart styles and output formats in the visualization module.

---

## Project Structure

```
ai_data_analysis_agent/
├── ai_data_analyst.py      # Main application script
├── requirements.txt        # Python dependencies
├── README.md               # Project documentation
├── demo/                   # Demo files (screenshots, GIFs)
└── data/                   # Sample datasets (optional)
```

---

## Extending the Agent

- **Add New Analysis Functions:**  
  Implement new functions in `ai_data_analyst.py` and register them in the main workflow.
- **Integrate More Data Formats:**  
  Use libraries like `pyxlsb` or `pyarrow` for additional file types.
- **Custom Visualizations:**  
  Extend the visualization module to support more chart types (e.g., seaborn, plotly).

---

## Troubleshooting

- **Missing Dependencies:**  
  Run `pip install -r requirements.txt` to ensure all packages are installed.
- **API Errors:**  
  Check your API key and network connection.
- **File Not Found:**  
  Ensure the input file path is correct and accessible.

---

## Contributing

Contributions are welcome!  
To contribute:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature/your-feature`).
3. Commit your changes.
4. Push to your fork and submit a pull request.

Please see [CONTRIBUTING.md](CONTRIBUTING.md) for more details.

---

## License

This project is licensed under the [MIT License](LICENSE).

---
