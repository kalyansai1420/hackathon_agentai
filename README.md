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
   git clone https://github.com/yourusername/hackathon_agentai.git
   cd hackathon_agentai
   ```

2. **Install Dependencies:**

   ```bash
   pip install nx-arangodb
   pip install cugraph-cu12 --extra-index-url=https://pypi.nvidia.com
   pip install --upgrade langchain langchain-community langchain-openai langgraph
   pip install arango-datasets
   pip install gradio
   ```

3. **Set Up Environment Variables:**

   ```bash
   export OPENAI_API_KEY="your_openai_api_key_here"
   ```

## Usage

1. **Data Setup:**
   - Connect to your ArangoDB instance.
   - Load the Synthea dataset and build a NetworkX graph from the vertex and edge collections.

2. **Running the Agent:**
   - Run the Colab notebook cells in sequence.
   - Use the provided Gradio interface to enter natural language queries and optionally visualize the results.
   - Example queries include:
     - "Who is connected to Node 0?"
     - "What is the shortest path from Node 0 to Node 1?"
     - "Which doctors treat the most chronic conditions?"
     - "What's the most common treatment path for diabetes?"

3. **Testing:**
   - Use the test cell to run a set of sample queries and validate the agent's responses.


## Contributing

Contributions are welcome! Fork the repository and submit a pull request. For major changes, please open an issue first to discuss your ideas.

## License

This project is licensed under the MIT License – see the [LICENSE](LICENSE) file for details.

## Contact

For any questions or suggestions, please contact [saikalyan.maram@unh.edu](mailto:saikalyan.maram@unh.edu).
