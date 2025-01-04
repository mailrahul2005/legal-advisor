# legal-advisor: Get Legal information based on Indian Laws

## Overview
legal-advisor is an AI-powered application that lets you upload a draft of Indian Penal Code (Now Nyay Sanhita 2023). Using AI capabilities, legal-advisor lets you ask questions about the probable punishments for various activities and responds based on information in the Indal Penal Code.

## Features
- Upload `.pdf` documents.
- Chat with your document to find if an offence is punishable in India and probable punishments
- Retain context from previous questions for seamless interaction.

## How It Works
1. **Document Upload**:
   - The uploaded document is processed, and its content is indexed for efficient searching.
2. **AI Question-Answering**:
   - A conversational AI system is set up to retrieve and answer questions based on the document content.

## Setup Instructions

### Prerequisites
- Python 3.8 or higher
- Install the required libraries:
  #Upgrade Setuptools if Needed
  !pip install --upgrade setuptools wheel
  
  #Install prerequisite packages
  !pip install python-dotenv==1.0.0

  !pip install llama-index==0.10.59
  !pip install llama-index-llms-openai==0.1.27
  !pip install llama-index-embeddings-openai==0.1.11
  !pip install llama-index-llms-azure-openai==0.1.10
  !pip install llama-index-embeddings-azure-openai==0.1.11

### Environment Setup
1. I am using Azuire OpenAI so get an API key and end point to update in the code
    api_key = "provide your key"
    azure_endpoint = "provide your end point"

### Run the Application
1. Open the `legal-advisor.ipynb` file in Jupyter Notebook or JupyterLab.
2. Follow the instructions in the notebook to execute the cells step by step.
3. The code will Setup the GPT35 OPEN AI LLM and create embeddings model
4. It will then create the document index, vector store, query engine and a router agent
5. Then the router agent can be used to query the IPC document uploaded in the code

## Usage
1. **Upload a Document**:
   - Place the attached NyaySanhita file in the same folder as ipynb
2. **Execute Code**:
   - Execute the code cells to generate required embeddings and and router agent.
3. **Ask Questions**:
   - The sample question syntax is given in the code
4. **View Responses**:
   - The chatbot will display the answer, retaining the context of previous questions.

## Example Use Cases
- Check if some activity is illegal as per the Law
- Understand what could be the maximum punishment for various offences

## File Structure
- `legal-advisor.ipynb`: Jupyter Notebook containing the application code and instructions
- 'NyaySanhita2023.pdf': PDF copy of Indian Laws as of 2023
- `README.md`: Documentation file (this file).

## Limitations
- Only tested `.pdf`
- Requires an active internet connection to access OpenAI APIs.

## Contributing
If you'd like to contribute, feel free to fork the repository, make changes, and submit a pull request.

## License


