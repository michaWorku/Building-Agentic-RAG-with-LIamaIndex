# **📚 Building Agentic RAG with LlamaIndex**  

This repository contains course notes and notebooks for **Building Agentic RAG with LlamaIndex**, a short course by DeepLearning.AI and Jerry Liu (CEO of LlamaIndex). You'll learn how to build **autonomous research agents** that reason over documents, make decisions, and answer complex queries using LlamaIndex.  

---

## **🚀 What You'll Learn**  
- **Router Agents** – Direct queries to the right tools (Q&A or summarization).  
- **Tool-Calling Agents** – Enhance RAG pipelines with external tool execution.  
- **Research Agents** – Perform multi-step reasoning over multiple documents.  
- **Multi-Document Agents** – Summarize, compare, and analyze multiple research papers.  
- **Agentic Control & Debugging** – Modify, debug, and improve agent behavior.  

---

## **📂 Course Content**  

### [**1️⃣ Router Query Engine**](https://github.com/michaWorku/Building-Agentic-RAG-with-LIamaIndex/tree/main/Lesson_1)  
The **Router Engine** intelligently selects the right retrieval strategy:  
- **Vector Index** – Finds the most similar document nodes.  
- **Summary Index** – Uses the full document summary for queries.  

#### **Implementation Steps**  
✅ Load data using LlamaIndex’s **SimpleDirectoryReader**.  
✅ Define **LLM and embedding models**.  
✅ Create **Summary Index** & **Vector Index** over the same dataset.  
✅ Configure **Query Engines** with metadata.  
✅ Implement a **Router Query Engine** for dynamic selection.  

**🔹 Available Selectors:**  
- **LLM Selectors** – Parse JSON responses for routing.  
- **Pydantic Selectors** – Use OpenAI’s function calling API.  


### [**2️⃣ Tool Calling for Enhanced Retrieval**](https://github.com/michaWorku/Building-Agentic-RAG-with-LIamaIndex/tree/main/Lesson_2)  
Tool calling enables **LLMs to interact with external tools**, improving query understanding and retrieval accuracy.  

#### **Key Concepts:**  
- Standard RAG relies on **static retrieval**, while **tool calling enables dynamic selection** of retrieval strategies.  
- The LLM **chooses appropriate tools** and **infers arguments** for better response generation.  

#### **Implementation Steps**  
✅ Define **custom tool functions** and integrate them with the LLM.  
✅ Create an **Auto-Retrieval Tool** to dynamically fetch relevant data.  
✅ Implement **metadata filters** (e.g., page numbers, sections) for precision.  
✅ Build a **multi-tool system** combining **vector search & summarization**.  


### [**3️⃣ Building an Agent Reasoning Loop**](https://github.com/michaWorku/Building-Agentic-RAG-with-LIamaIndex/tree/main/Lesson_3)  
An **agentic RAG system** involves multi-step reasoning over multiple documents.  

#### **Core Components:**  
- **Agent Worker** – Executes tasks using tools (vector search, summarization).  
- **Agent Runner** – Orchestrates tasks, tracks **agent state**, and manages **memory**.  

#### **Agentic Reasoning Flow:**  
✅ Initialize an **Agent Worker** with task execution capabilities.  
✅ Set up an **Agent Runner** to manage and coordinate tasks.  
✅ Implement **debugging tools** for step-by-step execution insights.  
✅ Improve **control & steerability** by allowing manual intervention.  

**🔹 Benefits:**  
✔ **Decoupling Execution & Task Creation** – Schedule tasks flexibly.  
✔ **Debuggability** – Gain deeper insights into each reasoning step.  
✔ **Steerability** – Modify intermediate steps with human feedback.  


### [**4️⃣ Building a Multi-Document Agent**](https://github.com/michaWorku/Building-Agentic-RAG-with-LIamaIndex/tree/main/Lesson_4)  
This section extends the **agentic reasoning model** to handle multiple documents efficiently.  

#### **Implementation Steps**  
✅ Load multiple documents (e.g., research papers from arXiv).  
✅ Implement **tool retrieval** for multi-document selection.  
✅ Create an **Agent Worker & Runner** to execute queries across documents.  
✅ Query results, analyze retrieval quality, and refine responses.  


## **🛠 Setup & Installation**  

### **1️⃣ Clone the Repository**  
```bash
git clone[ https://github.com/your-repo-url.git](https://github.com/michaWorku/Building-Agentic-RAG-with-LIamaIndex.git)
cd your-repo-folder
```

### **2️⃣ Install Dependencies**  
```bash
pip install -r requirements.txt
```

### **3️⃣ Run the Jupyter Notebook**  
```bash
jupyter notebook
```


## **📚 References**  
- [LlamaIndex Documentation](https://gpt-index.readthedocs.io/en/latest/)  
- [DeepLearning.AI Course](https://www.deeplearning.ai/short-courses/building-agentic-rag-with-llamaindex/)  
- [OpenAI Function Calling](https://platform.openai.com/docs/guides/function-calling)  


## **💡 Conclusion**  
This course provides a **systematic approach** to building **intelligent, autonomous RAG systems** that can dynamically retrieve, summarize, and analyze data. By implementing **agentic reasoning, tool calling, and multi-document querying**, you can significantly enhance the **accuracy, depth, and control** of LLM-powered applications. 🚀  
