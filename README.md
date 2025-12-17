# 📸 Image Analysis and Description Tool

A scalable and efficient tool for generating detailed image descriptions using Google Vertex AI and advanced prompt engineering techniques.

---

## 📝 Overview

This project was developed as part of a **Google Vertex AI Lab Course** to demonstrate key concepts in **Large Language Model (LLM) deployment** and **Prompt Engineering**.

The application utilizes a multimodal LLM on Vertex AI to accept an image input and return a human-readable, contextual description of its contents. The quality and specificity of the output are controlled entirely through **System Messages** and **Model Parameter Tuning**.

### Key Actions Performed:

* ✍️ **System Message Design:** Crafting a precise system message to define the model's role and output format.
* 🔬 **Model Parameter Tuning:** Adjusting parameters (like Temperature and Top-p) to optimize descriptive quality.
* 🚀 **Vertex AI Deployment:** Deploying the configured model logic via the **Vertex AI Lab Deploy Action** for an easily accessible endpoint.

---

## ✨ Features

* **High-Quality Descriptions:** Generates detailed, objective, and contextually rich descriptions for any image.
* **Controlled Generation:** Uses a powerful system message to enforce specific style, length, and focus in the output.
* **Scalable API:** Deployed as a managed service on **Vertex AI Endpoints**, ready for production use.
* **Zero Infrastructure Overhead:** Leverages Vertex AI for fully managed model hosting and serving.

---


## 🚀 Getting Started

To replicate the solution or understand the configuration, follow these steps.

### 1. The Core Configuration

The intelligence of this tool is embedded in how the underlying LLM is instructed:

| Configuration Aspect | Description | Example Value |
| :--- | :--- | :--- |
| **System Message** | **Defines the AI's persona and task.** 
| **Temperature** | Controls the randomness/creativity of the output. | **1.5** (for creative output) |
| **Max Output Tokens** | Limits the length of the generated description. | **500** |

### 2. Deployment on Vertex AI

The deployment was handled through the specific action provided by the lab environment.

1.  **Preparation:** Package the inference code (which includes the system message and parameters) into a deployable artifact.
2.  **Deployment Action:** Execute the **Vertex AI Lab Deploy Action**, specifying the model and endpoint configuration.
3.  **Endpoint Creation:** Vertex AI creates a **REST API Endpoint** for live inference.
---
## Demo
![Screenshot of the Image anslyzer in action](./assets/Screenshot.png)
---
