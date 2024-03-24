# LangChain Usage Example

This repository provides an example of using LangChain, a framework for building conversational agents with integrated knowledge retrieval capabilities.

## Installation

To install the required packages, run the following commands:

```bash
pip install -q langchain==0.1.4
pip install langchainhub==0.1.14
pip install -q datasets==2.16.1
pip install -q chromadb==0.4.22
pip install --upgrade --quiet langchain-google-genai

## Usage

The provided example demonstrates how to utilize LangChain for building a conversational agent capable of answering medical queries. The workflow involves:

    Loading medical question-answer pairs from a dataset.
    Generating embeddings for the loaded documents.
    Creating a retriever for retrieving relevant documents based on user queries.
    Utilizing a generative language model to generate responses.
    Implementing conversational memory to maintain context during interactions.
    Creating an agent with predefined tools for answering medical questions.
    Invoking the agent to respond to user queries.

### Example Execution

The example demonstrates interactions with the conversational agent for various medical queries:

    Question: "How to prevent Parasites - Cysticercosis?"
        Response: Provides information on preventive measures for the mentioned disease.

    Question: "Do you know who is Clark Kent?"
        Response: Provides information about Clark Kent, the secret identity of Superman.

    Question: "What is her age?"
        Response: Indicates inability to answer due to lack of context about the person referred to.

    Question: "I have a patient that can have Botulism, how can I confirm the diagnosis?"
        Response: Advises consulting a medical professional for confirmation of diagnosis.

    Question: "Is this an important illness?"
        Response: Provides information on the severity and potential consequences of Botulism.

    Question: "Is it really important to know about it?"
        Response: Affirms the importance of awareness about Botulism for timely medical intervention.

Notes

    This example demonstrates the integration of LangChain with Google Generative AI and ChromaDB for document retrieval and embedding generation. Additional tools and knowledge bases can be integrated as per requirements.

## Acknowledgments

This example utilizes resources and models from the LangChain community and Google Generative AI.