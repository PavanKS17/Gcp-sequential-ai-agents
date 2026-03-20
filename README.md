# Sequential AI Agent Orchestration (GCP)

This project demonstrates a multi-agent system built using the **Google Cloud Agent Development Kit (ADK)**. It features a sequential workflow where a primary supervisor agent coordinates tasks across specialized sub-agents.

##  Features
* **Sequential Logic:** Uses a "Supervisor" pattern to delegate complex user requests (e.g., Image Generation) to specific worker agents.
* **Vertex AI Integration:** Powered by **Gemini 2.5 Flash** for high-speed reasoning and orchestration.
* **Multimodal Capabilities:** Includes an Image Generation tool powered by **Imagen**.
* **Cloud-Native:** Built and tested within **Google Cloud Shell** with seamless deployment paths to **Cloud Run**.

## 🛠️ Tech Stack
* **Orchestration:** Google Cloud ADK
* **Models:** Gemini 2.5 Flash / Pro
* **APIs:** Vertex AI (Generative AI & Image Generation)
* **Environment:** Python 3.12+ 

## ⚙️ Setup & Authentication
This project requires Google Cloud **Application Default Credentials (ADC)** and an active billing project with the `aiplatform.googleapis.com` API enabled.

```bash
gcloud auth application-default login
gcloud auth application-default set-quota-project YOUR_PROJECT_ID
