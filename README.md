# GraphRAG: Hybrid Graph Analytics Agent

GraphRAG is a hybrid AI agent that leverages advanced graph analytics to provide dynamic insights for healthcare. By integrating ArangoDB, NetworkX, and cuGraph with natural language processing (via LangChain & LangGraph), GraphRAG seamlessly combines structured AQL traversals with GPU-accelerated analytics to uncover key patterns in patient care and provider influence.

## Features

- **Hybrid Query Execution:** Combines AQL traversals with complex graph analytics (e.g., PageRank, connectivity, community detection).
- **Dynamic Query Routing:** Automatically routes queries based on intent using a robust caching mechanism and regex matching.
- **GPU-Accelerated Analytics:** Utilizes cuGraph & cuDF for fast, GPU-accelerated PageRank computations.
- **Interactive Visualizations:** Visualizes subgraphs and community clusters using Matplotlib.
- **User-Friendly Interface:** Provides an interactive Gradio UI for real-time query exploration.

## Built With

Python, ArangoDB, nx-arangodb, NetworkX, cuGraph, cuDF, LangChain, LangGraph, Gradio, Google Colab, Pandas, NumPy, Matplotlib, Arango Datasets

## Project Overview

GraphRAG was inspired by the challenge of extracting actionable insights from complex healthcare data. Using the synthetic Synthea dataset, the project demonstrates how hybrid query execution can reveal valuable information about patient care and provider influence in real time. The agent handles simple, complex, and hybrid queries by dynamically combining direct graph traversals with advanced analytics, making it a powerful tool for healthcare data analysis.

## Installation

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/kalyansai1420/hackathon_agentai.git
   cd hackathon_agentai
