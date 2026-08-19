## StorRAG is an OpenSource RAG Appliance, to turn "your" storage into "your" data.

- 🔭 This is our Github Pages Repo hosting StorRAG.com
- 🌱 If you interested in what we're building jump into the Appliance repo
- 👯 If you want to help, or have found a bug, please make a Pull Request
- 🤔 We're always looking for collaborators, please make a Pull Request
- 💬 Sales and Support questions are via our WhatsApp group
- 📫 Reach us via a Pull Request or our WhatsApp group
- ⚡ Fun fact: This "idea in the making" started in Australia... G-Day!

## StorRAG is OpenSource. Your Code, Your Data, Forever!

Our idea in the making. A RAG Appliance with a mission, to turn **your storage**, into **your data**.

At StorRAG our code is in [GitHub](https://github.com/StorRAG/Appliance) and our software is packaged in a [Bootable Container](https://bootc.dev/bootc/) . This means you can review the code **Anytime** and run the software **Anywhere**, from **Bare Metal** to **The Cloud**. 

### What is a StorRAG Appliance

At StorRAG we build a custom RAG (Retrieval Augmented Generation) application, packaged in a Bootable Container. Consisting of three main components; 

### The Model Service 

For the local Model Serving and an OpenAI compatible Model Service.

### The Vector Database

In order for the LLM to interact with your data, we connect to your data stores using industry standard storage protocols (like S3, NFS, SMB and block). We make this data available in such a manner that we can retrieve a small subset of each of them that are relevant to any query. To do this we employ a Vector Database alongside an embedding model. The embedding model converts our documents into numerical representations, vectors, such that similarity searches can be easily performed. The Vector Database stores these vectors for us and makes them available to the LLM.

### The Data Import Application

Our Data Import Application connects to our Model Service via it's OpenAI compatible API. We package a well performant mid-sized model with an apache-2.0 license that has been quanitzed and served into the GGUF format **(no GPU required)**.

### How do I get it?

Simple, Those who want to get started quickly and conveniently may install StorRAG using the following command:

```
curl -sSL https://storrag.com/install.sh | bash
```
For those looking for more options our code is in [GitHub](https://github.com/StorRAG/Appliance)

For Discourse, Sales and Support join our [WhatsApp Community](https://chat.whatsapp.com/BabLkdFELY60QYoW4nTg4y?s=cl&p=i&mlu=4).
