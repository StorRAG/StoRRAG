---
layout: default
---
![The StorRAG Bot](https://github.com/StorRAG/StorRAG/blob/main/StorRAG-logo.png)

Our idea in the making. A RAG Appliance with a mission, to turn **your storage**, into **your data**.

## OpenSource. Your Data, Your Software, Forever!

At StorRAG our code is in [GitHub](https://github.com/StorRAG/) and is packaged in a [Bootable Container](https://bootc.dev/bootc/) . This means you can review the code **anytime** and run the software **anywhere** from **Bare Metal** to **The Cloud**. 

## What is a StorRAG Appliance

At StorRAG we build a custom RAG (Retrieval Augmented Generation) application, packaged in a Bootable Container. The Container consists of three main components; 

### The Model Service 

For the local Model Serving and an OpenAI compatible Model Service.

### The Vector Database

In order for the LLM to interact with your data, we connect to your data stores using standard industry protocols and make it available in such a manner that we can retrieve a small subset of each of them that are relevant to any query. To do this we employ a Vector Database alongside an embedding model. The embedding model converts our documents into numerical representations, vectors, such that similarity searches can be easily performed. The Vector Database stores these vectors for us and makes them available to the LLM.

### The Data Import Application

Our Data Import Application connects to our Model Service via it's OpenAI compatible API. We package a well performant mid-sized model with an apache-2.0 license that has been quanitzed and served into the GGUF format (no need for a GPU).

### How do I get it?

First, download and uncompress the software, then spin up a Pod along with a number of containers using the commands below:

```
cd rag
make quadlet
podman kube play build/rag.yaml
```

The Pod is named rag, so you may use Podman to manage the Pod and its containers:

```
podman pod list
podman ps
```

To stop and remove the Pod, run:

```
podman pod stop rag
podman pod rm rag
```

Please contact us for Sales and Support on our [slack channel]().
