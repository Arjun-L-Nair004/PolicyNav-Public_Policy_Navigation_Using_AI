# Infosys Springboard
# 🧠 PolicyNav - Public-Policy-Navigation-Using-AI
AI-Powered Public Policy Navigation and Intelligence Platform
Simplifying complex government policies through multilingual AI, summarization, and intelligent search.
# 🔗 Links: 
| Category       | Link                                   |
| -------------- | -------------------------------------- |
| Demo Video     | https://drive.google.com/file/d/1iWPSKYKJvN9n7cfZkcAdOkUDFPQ0DH1q/view?usp=sharing |
| Source Code    | This Repository                        |
| Docker Support | Yes                                    |
| AI Models      | Sentence Transformers · FLAN-T5 · NLLB |
# 📌 Table of Contents
- About the Project
- Problem Statement & Motivation
- Key Features
- Architecture
- Tech Stack
- Models Used
- Project Structure
- Installation & Setup
- Usage Guide
- Admin Controls
- Screenshots
- Roadmap
- Team
- License

# 📖 About the Project

**PolicyNav – Public Policy Navigation Using AI** is an advanced AI-powered platform designed to simplify, analyze, and navigate complex public policy and regulatory documents through intelligent automation and natural language processing.

This project was developed as part of an intensive learning program comprising approximately 60 live interactive sessions, focusing on building practical expertise in applying Artificial Intelligence to real-world governance and policy challenges.

PolicyNav addresses the critical challenge of understanding lengthy, complex, and often inaccessible public policy documents by transforming them into user-friendly, interactive, and intelligent insights.

---

## 🎯 Core Objectives

- Simplify complex government policies for general users
- Enable intelligent search and navigation across policy documents
- Provide automated summarization and explanation of legal texts
- Support multilingual accessibility for diverse users
- Assist in policy analysis, compliance understanding, and decision-making

---

## 🧠 Key Capabilities

### 🔍 AI-Powered Policy Search & Navigation
The system enables users to efficiently explore large volumes of policy documents using semantic search techniques instead of traditional keyword-based search.

- Understands user intent using NLP
- Retrieves contextually relevant policy sections
- Reduces time spent scanning lengthy documents

---

### 📚 Natural Language Understanding (NLU) for Policy Texts
PolicyNav leverages advanced NLP models to interpret complex legal and regulatory language.

- Processes unstructured policy data
- Understands context, terminology, and relationships
- Converts technical language into understandable insights

---

### ✂️ Intelligent Summarization & Question Answering
The platform provides automated summarization and precise answers to user queries.

- Generates concise summaries of long documents
- Answers policy-related questions using contextual understanding
- Helps users quickly grasp key information without reading full texts

---

### 🧩 Entity Extraction & Knowledge Structuring
Extracts key entities and relationships from policy documents to build structured knowledge.

- Identifies organizations, schemes, dates, and key terms
- Enables knowledge graph visualization
- Improves understanding of policy ecosystems

---

### 🤖 AI Assistants for Policy Analysis & Compliance
PolicyNav acts as an intelligent assistant for interpreting and analyzing policies.

- Assists users in understanding policy implications
- Helps in compliance checking and eligibility understanding
- Supports stakeholders such as students, researchers, and analysts

---

## 🌍 Real-World Learning & Implementation

This project emphasizes hands-on learning and practical implementation through:

- Real-world datasets involving public policies and regulations
- Case studies addressing governance and accessibility challenges
- Collaborative development and problem-solving
- Integration of multiple AI models and tools into a unified system

---

## 💡 Impact

PolicyNav aims to bridge the gap between complex policy frameworks and public understanding by making information:

- More accessible  
- More understandable  
- More interactive  

It empowers users to make informed decisions by transforming static policy documents into dynamic, AI-driven insights.

# 🎯 Problem Statement & Motivation

## ❗ Problem Statement

Understanding public policies and government regulations is a significant challenge for most users due to the complexity, structure, and accessibility of the information.

Key issues include:

- **Complex Language:**  
  Policy documents are often written in highly technical, legal, and formal language, making them difficult for common users to interpret.

- **Lengthy Documents:**  
  Policies can span hundreds of pages, requiring significant time and effort to extract relevant information.

- **Lack of Structured Access:**  
  There is no unified platform that allows users to easily search, navigate, and understand policies in a structured manner.

- **Language Barriers:**  
  Many users face difficulties accessing policies due to limited availability in regional languages.

- **Inefficient Information Retrieval:**  
  Traditional keyword-based search systems fail to capture context and intent, leading to irrelevant or incomplete results.

---

## 💡 Motivation

The motivation behind PolicyNav is to bridge the gap between complex policy frameworks and user understanding by leveraging Artificial Intelligence and Natural Language Processing.

This project aims to:

- **Simplify Policy Understanding:**  
  Convert complex and technical policy documents into concise, easy-to-understand summaries.

- **Enhance Accessibility:**  
  Provide multilingual support to ensure inclusivity for users from diverse linguistic backgrounds.

- **Enable Intelligent Search:**  
  Replace traditional keyword search with semantic, context-aware retrieval systems.

- **Support Decision-Making:**  
  Help users, researchers, and analysts quickly access relevant policy insights for informed decisions.

- **Promote Digital Governance:**  
  Improve transparency and accessibility of government policies through AI-driven solutions.

---

## 🚀 Vision

To build an intelligent, user-centric platform that transforms static and complex policy documents into interactive, accessible, and actionable knowledge for everyone.

# 📂 Project Structure

The project follows a structured, milestone-driven development approach to ensure clarity, scalability, and systematic progress. Each phase of development is organized into separate milestone folders, allowing easy tracking of features and improvements over time.

---

## 🔄 Development Flow Structure

PolicyNav → Milestone1 → Milestone2 → Milestone3 → Milestone4 → Final System

---

## 🧩 Folder Organization

### 📁 Milestone 1 – Foundation Phase
This is the starting point of the project where the core idea and setup are established.

- Problem understanding and requirement analysis  
- Initial project setup and environment configuration  
- Basic UI design and workflow planning  
- Documentation available in `Milestone1/README.md`  

---

### ⚙️ Milestone 2 – Core Development Phase
This phase focuses on building the fundamental system features.

- User authentication (JWT, bcrypt, OTP)  
- Basic backend logic and database integration  
- Initial NLP pipeline setup  
- Documentation available in `Milestone2/README.md`  

---

### 🧠 Milestone 3 – AI Integration Phase
In this phase, advanced AI functionalities are integrated into the system.

- Semantic search using FAISS  
- Summarization using FLAN-T5  
- Translation using NLLB  
- Entity extraction using SpaCy  
- Documentation available in `Milestone3/README.md`  

---

### 🚀 Milestone 4 – Finalization Phase
This is the final stage where the system is completed and prepared for deployment.

- Full system integration  
- Testing and debugging  
- Performance optimization  
- Docker-based deployment  
- Documentation available in `Milestone4/README.md`  

---

## 📌 Root-Level Files

- `README.md` → Contains the complete overview of the project  
- `requirements.txt` → Lists all required dependencies  
- `LICENSE` → Defines project usage and distribution rights  

---

## ✅ Key Advantages of This Structure

- Clearly shows **project evolution from basic to advanced stages**  
- Makes it easier for evaluators to **track progress step-by-step**  
- Ensures **clean separation of features and implementation phases**  
- Improves maintainability and future scalability  
---

## 📌 Why This Structure?

- Promotes **clean and organized development**
- Makes evaluation **easy and structured**
- Clearly shows **project progression (M1 → M4)**
- Helps in **maintenance and scalability**


## 📌 Benefits of This Structure

- Clear separation of development phases  
- Easy tracking of project progress  
- Better documentation and evaluation  
- Simplifies debugging and feature enhancement  


# ⚙️ Installation & Setup

## 🔧 Prerequisites

Ensure you have the following installed:

- Python 3.10 or higher
- Git
-  Docker for containerized deployment

---
## Install Dependencies
pip install -r requirements.txt

## Run the application
streamlit run app.py

 ## Docker Setup

To run the project using Docker:

docker build -t policynav .
docker run -p 8501:8501 policynav


# 🛡 Admin Controls

The platform includes a dedicated admin interface for managing users, monitoring system performance, and improving overall functionality.

---

## 👥 User Management
- View all registered users
- Block or delete accounts
- Monitor suspicious activities

---

## 📊 System Monitoring Dashboard
- Track number of active users
- Monitor query volume and usage trends
- Analyze system performance metrics

---

## 💬 Feedback Management
- Review user ratings and comments
- Identify issues in AI-generated responses
- Use insights to improve system accuracy

---

## 📜 Activity Logs
- Maintain logs of:
  - User interactions
  - System events
- Useful for debugging, auditing, and tracking usage

---

## 🔐 Security Oversight
- Monitor authentication activity
- Ensure secure access and data protection


# 🚀 Key Features 

## 👤 User Features

### 🔐 Secure Authentication System
The platform implements a robust authentication and authorization mechanism to ensure user data security and controlled access.

- Uses JWT (JSON Web Tokens) for session management, enabling stateless and secure authentication.
- Passwords are encrypted using bcrypt hashing, preventing plaintext storage.
- Includes OTP-based password recovery, ensuring secure identity verification.
- Protects endpoints from unauthorized access through token validation.

Why it matters:  
Ensures user privacy, prevents unauthorized access, and aligns with modern security best practices.

---

### 🤖 AI Policy Assistant
An intelligent conversational interface that allows users to interact with public policies using natural language queries.

- Built using transformer-based NLP models.
- Converts user queries into embeddings via Sentence Transformers.
- Performs semantic search using FAISS to retrieve the most relevant policy content.
- Generates contextual responses using FLAN-T5.

Example Workflow:  
User Query → Embedding → FAISS Retrieval → Context Extraction → FLAN-T5 Response

Why it matters:  
Removes the need for users to manually read long documents and enables intuitive interaction.

---

### 🌍 Multi-language Support
Enables accessibility for users from diverse linguistic backgrounds.

- Uses NLLB (No Language Left Behind) model for translation.
- Supports both:
  - Query translation (user input → English for processing)
  - Response translation (output → user’s preferred language)

Why it matters:  
Breaks language barriers and makes government policies accessible to a wider audience.

---

### ✂️ Intelligent Summarization
Automatically generates concise summaries of lengthy policy documents.

- Uses FLAN-T5, a fine-tuned transformer model.
- Extracts key information while preserving meaning and context.
- Supports dynamic summarization based on retrieved policy sections.

Why it matters:  
Saves time and improves comprehension of complex documents.

---

### 🕸 Knowledge Graph Visualization
Transforms unstructured policy data into structured visual relationships.

- Uses SpaCy for Named Entity Recognition (NER).
- Extracts entities such as organizations, policies, dates, and keywords.
- Builds relationships and visualizes them using PyVis interactive graphs.

Why it matters:  
Helps users understand connections between policies, stakeholders, and concepts visually.

---

### 📖 Readability Analyzer
Evaluates and simplifies complex policy text for better understanding.

- Uses NLP techniques to:
  - Measure sentence complexity
  - Identify difficult words and structures
- Provides simplified interpretations of policy content.

Why it matters:  
Ensures accessibility for non-expert users and improves inclusivity.

---

### 🌐 Global Web Search Integration
Enhances policy understanding by fetching external, real-time information.

- Integrates web search APIs to retrieve:
  - Latest policy updates
  - Related news and articles
- Combines internal knowledge base with external data sources.

Why it matters:  
Keeps users informed with up-to-date and contextual information.

---

### 👤 Profile Management System
Allows users to manage personal information securely.

- Update email and password
- Upload avatar/profile image
- Manage account preferences

Why it matters:  
Improves user personalization and engagement.

---

### 📊 Activity History Tracking
Maintains a log of user interactions.

- Stores:
  - Queries asked
  - Summaries generated
  - Actions performed
- Enables users to revisit previous insights.

Why it matters:  
Improves usability and supports continuity in research.

---

### ⭐ Feedback & Rating System
Collects user feedback for continuous improvement.

- Users can:
  - Rate system responses
  - Provide comments
- Admin can analyze feedback trends.

Why it matters:  
Helps refine AI responses and improve system performance.

---

## 🛡 Admin Features

### 👥 User Management Dashboard
- View all registered users
- Block or delete suspicious accounts
- Monitor user activity patterns

---

### 📈 System Monitoring & Analytics
- Track:
  - Number of queries
  - Active users
  - System usage trends

---

### 💬 Feedback Moderation
- Analyze user feedback
- Identify issues in AI responses
- Improve model performance based on insights

---

### 📜 Activity Logs
- Maintain logs for:
  - User actions
  - System events
- Useful for debugging and auditing

---

## 🧩 Architecture 

The system follows a monolithic architecture where all components are integrated into a unified application.

### 🔄 Data Flow

1. User interacts via Streamlit UI  
2. Request is sent to Python backend  
3. Backend processes:
   - Authentication
   - Query handling  
4. AI modules perform:
   - Embedding generation
   - Semantic search (FAISS)
   - Summarization / translation  
5. Results are returned to UI  
6. Data is stored/retrieved from SQLite database  

---

### 🧠 AI Pipeline

- Input Query  
→ Preprocessing  
→ Embedding (Sentence Transformers)  
→ Retrieval (FAISS)  
→ Processing (FLAN-T5 / NLLB)  
→ Output Response  

Why Monolithic?  
- Easier deployment (especially with Docker)  
- Simpler integration of AI modules  
- Suitable for prototype and hackathon environments  

---

## 🛠 Tech Stack 

| Layer         | Technology                 | Why Used |
|--------------|--------------------------|---------|
| Frontend     | Streamlit                 | Rapid UI development and ML integration |
| Backend      | Python                    | Strong ecosystem for AI/ML and APIs |
| Database     | SQLite                    | Lightweight and easy to integrate |
| AI Models    | Hugging Face Transformers | State-of-the-art NLP capabilities |
| Search       | FAISS                     | Fast similarity search for embeddings |
| NLP          | SpaCy                     | Efficient entity extraction |
| Visualization| PyVis                     | Interactive graph visualization |
| Security     | JWT, bcrypt, OTP          | Secure authentication and encryption |
| Deployment   | Docker                    | Easy containerization and portability |

---

## 🤖 Models Used 

### Sentence Transformers
- Converts text into dense vector embeddings  
- Enables semantic similarity search  
- Works with FAISS for fast retrieval  

---

### FLAN-T5
- Instruction-tuned transformer model  
- Used for:
  - Summarization  
  - Question answering  
- Generates human-like responses  

---

### NLLB (No Language Left Behind)
- Meta AI multilingual translation model  
- Supports low-resource languages  
- Ensures global accessibility  

---

### SpaCy
- Industrial-strength NLP library  
- Used for:
  - Named Entity Recognition (NER)  
  - Text preprocessing
 

# 📸 Screenshots


<img width="913" height="401" alt="Screenshot 2026-03-15 133821" src="https://github.com/user-attachments/assets/12289b46-31bd-41ac-8084-8811f4f7980b" />


<img width="1865" height="842" alt="Screenshot 2026-03-18 225511" src="https://github.com/user-attachments/assets/8f9cd591-8e89-48af-a55f-6c53748bbfe7" />


<img width="1026" height="406" alt="Screenshot 2026-03-18 021246" src="https://github.com/user-attachments/assets/8e548c4c-4080-4730-a188-f70b891c3d0d" />


<img width="1893" height="847" alt="Screenshot 2026-03-18 225641" src="https://github.com/user-attachments/assets/39e8a589-21fa-41a9-bd4b-69dbedb27b5c" />


<img width="1909" height="821" alt="Screenshot 2026-03-18 225619" src="https://github.com/user-attachments/assets/be66cc46-fe34-4ea9-8f59-e30f78ecab56" />


<img width="1892" height="829" alt="Screenshot 2026-03-18 225554" src="https://github.com/user-attachments/assets/881a72c8-8baa-4ae4-8420-bec8c0d7c4fc" />


<img width="1<img width="1784" height="804" alt="Screenshot 2026-03-18 225734" src="https://github.com/user-attachments/assets/802c4243-3251-4d28-a8d2-557ad56a43ca" />


<img width="991" height="555" alt="Screenshot 2026-03-18 225708" src="https://github.com/user-attachments/assets/d9d80693-ebcf-4cf1-ac2e-df6b905d5f2c" />


<img width="1796" height="811" alt="Screenshot 2026-03-18 225653" src="https://github.com/user-attachments/assets/62abd28c-2f82-4330-bcf8-fcd6ff6fe57a" />


<img width="1700" height="717" alt="Screenshot 2026-03-18 230308" src="https://github.com/user-attachments/assets/7feda5b0-58d2-4415-bedb-95eb967913f9" />


<img width="1693" height="751" alt="Screenshot 2026-03-18 230257" src="https://github.com/user-attachments/assets/931c4283-fa1b-48a4-8ab3-dcca4366da22" />


<img width="1757" height="800" alt="Screenshot 2026-03-18 230236" src="https://github.com/user-attachments/assets/420669a0-09c1-49eb-97f5-66bb17660d76" />


<img width="1850" height="823" alt="Screenshot 2026-03-18 225956" src="https://github.com/user-attachments/assets/133c0a18-1579-432d-a2c6-143d5e03bda1" />


<img width="1824" height="814" alt="Screenshot 2026-03-18 225902" src="https://github.com/user-attachments/assets/a4b611e3-8f3b-4bbc-acee-af7fe734581c" />


880" height="830" alt="Screenshot 2026-03-18 225531" src="https://github.com/user-attachments/assets/1e6c1af5-3ad7-4e77-be72-441f08d4e79d" />


# 📊 Roadmap

The future development of PolicyNav focuses on enhancing performance, scalability, user experience, and accessibility. The following roadmap outlines planned improvements and upcoming features:

---

## 🚀 Improve Model Performance
- Fine-tune existing models (FLAN-T5, Sentence Transformers) on domain-specific policy datasets
- Optimize response accuracy and relevance in semantic search
- Reduce latency in query processing and model inference
- Implement caching mechanisms for frequently asked queries
- Explore lightweight or quantized models for faster execution

---

## 📚 Expand Dataset Coverage
- Integrate additional government policy datasets from multiple domains (health, education, finance, etc.)
- Include region-specific and state-level policies
- Continuously update datasets to reflect latest policy changes
- Improve data preprocessing and cleaning pipelines for better model performance

---

## 🎨 Enhance UI/UX
- Improve overall interface design for better usability and accessibility
- Add interactive dashboards and visual components
- Optimize navigation flow for smoother user experience
- Ensure mobile responsiveness and cross-device compatibility
- Enhance visualization of knowledge graphs and outputs

---

## ☁️ Cloud Deployment & Scalability
- Deploy the application on cloud platforms (AWS / Azure / GCP)
- Implement scalable backend infrastructure for handling multiple users
- Use container orchestration (Docker + Kubernetes) for efficient deployment
- Enable CI/CD pipelines for automated testing and deployment
- Improve system reliability and uptime

---

## 🎤 Voice-Based Interaction
- Integrate speech-to-text functionality for voice queries
- Enable text-to-speech for AI-generated responses
- Support multilingual voice interaction
- Improve accessibility for users with limited literacy or disabilities
- Create a conversational AI experience using voice assistants

---

## 🔮 Future Vision
- Build a fully conversational AI policy assistant
- Integrate real-time policy updates and alerts
- Add personalized recommendations based on user behavior
- Expand to global policy coverage


# 👥 Team 1

| Name                          | Role                              |
| ----------------------------- | --------------------------------- |
| Shambhavi Jha                 | AI and NLP Development            |
| Srideepalakshmi Muruganantham | Backend and Security              |
| Mainuddeen                    | Summarization and Web Integration |
| Bhuvaneshwar Reddy Mandadapu  | Profile and System Integration    |
| Arjun L Nair                  | Testing and Deployment            |


# 📜 License


MIT License
- Free to use, modify, and distribute with proper credits.
