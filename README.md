# Spring AI + Ollama

A hands-on Spring Boot project for learning and experimenting with **Spring AI** and **local Large Language Models (LLMs)** using **Ollama**.

This project is part of my journey to understand how AI/LLM capabilities can be integrated into Java and Spring Boot applications.

## 🚀 Project Overview

The goal of this project is to explore Spring AI concepts step by step, starting with setting up a Spring Boot application that can communicate with a locally running LLM through Ollama.

### Architecture

```text
┌─────────────────────┐
│    Spring Boot      │
│     Application     │
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│      Spring AI      │
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│       Ollama        │
│   Local LLM Runtime  │
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│    Local AI Model   │
│  Llama / Qwen / etc │
└─────────────────────┘
```

## 🛠️ Technology Stack

* Java 17
* Spring Boot 4.1.x
* Spring AI 2.x
* Maven
* Spring Web
* Ollama
* Local LLMs
* IntelliJ IDEA

## 💻 Prerequisites

Make sure the following are installed:

### Java

Java 17 or later.

Verify:

```bash
java -version
```

### Maven

Verify:

```bash
mvn -version
```

### Ollama

Install Ollama from:

https://ollama.com/

Verify:

```bash
ollama --version
```

## 🤖 Running a Local LLM with Ollama

After installing Ollama, download a model.

For example:

```bash
ollama pull llama3.2
```

Run the model:

```bash
ollama run llama3.2
```

You can then interact with the model directly from the terminal.

## 🏃 Running the Application

Clone the repository:

```bash
git clone https://github.com/avneet297/spring-ai-ollama.git
```

Navigate to the project:

```bash
cd spring-ai-ollama
```

Build the project:

```bash
mvn clean install
```

Start the Spring Boot application:

```bash
mvn spring-boot:run
```

Alternatively, run the application directly from IntelliJ IDEA.

## 📁 Project Structure

```text
spring-ai-ollama/
│
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/
│   │   │       └── example/
│   │   │           └── springaiollama/
│   │   │
│   │   └── resources/
│   │       └── application.properties
│   │
│   └── test/
│
├── .gitignore
├── pom.xml
├── mvnw
├── mvnw.cmd
└── README.md
```

## 🔑 Configuration

When working with local Ollama models, the application communicates with the Ollama service running on your machine.

Typical local Ollama configuration uses:

```text
http://localhost:11434
```

Keep environment-specific configuration outside of source control when appropriate.

## 🎯 Learning Approach

This is intentionally a learning project.

Rather than building one large AI application immediately, the project will evolve incrementally:

```text
Spring Boot
     ↓
Spring AI
     ↓
ChatClient / ChatModel
     ↓
Ollama
     ↓
Local LLM
     ↓
Prompts
     ↓
Structured Output
     ↓
Embeddings
     ↓
Vector Database
     ↓
RAG
     ↓
Tools / Agents
```

Each stage will introduce a new Spring AI concept and build on the previous one.

## 📖 Learning Resource

This project follows concepts from the **Spring AI Tutorials** series by Learn Code With Durgesh.

Current lesson:

**Setup Spring AI Project with Free LLM — Ollama**

YouTube playlist:

https://www.youtube.com/playlist?list=PL0zysOflRCen1TeDUm-ebl9T-WbJygCGE

Reference video:

https://www.youtube.com/watch?v=-q2ky1EE69g

The repository is my own implementation and learning workspace rather than a copy of the tutorial source code.

## 🔮 Future Improvements

As I progress through Spring AI, this repository will be expanded with practical examples covering:

1. Basic chat interactions
2. `ChatClient`
3. `ChatModel`
4. Prompt engineering
5. Response parsing
6. Multiple models
7. Dynamic prompts
8. Embeddings
9. Vector stores
10. RAG
11. Tool/function calling
12. MCP
13. AI agents
14. Production-ready AI architecture

## 👨‍💻 Author

**Avneet Singh**

Senior Java Developer | Spring Boot | Microservices | Cloud | AI

---

⭐ This repository documents my hands-on journey into **Spring AI and Generative AI development with Java**.
