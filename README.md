<div align="center">

# 🛍️ AI-Powered E-Commerce Platform

### Intelligent Product Discovery with Spring AI & Semantic Search

A modern e-commerce application that combines traditional product management with **Generative AI, Vector Embeddings, Semantic Search, and an AI-powered product chatbot**.

<br>

![Java](https://img.shields.io/badge/Java-17+-orange?style=for-the-badge\&logo=openjdk)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-3.x-brightgreen?style=for-the-badge\&logo=springboot)
![Spring AI](https://img.shields.io/badge/Spring%20AI-GenAI-green?style=for-the-badge\&logo=spring)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-Vector%20Search-blue?style=for-the-badge\&logo=postgresql)

</div>

---

## 🚀 About The Project

This project is an **AI-powered e-commerce application** built using **Java, Spring Boot, Spring AI, and PostgreSQL**.

Along with standard product and order functionality, the application introduces intelligent product discovery through **semantic search and conversational AI**.

Instead of relying only on exact keyword searches, users can describe what they are looking for in natural language and receive relevant product results.

### ✨ Highlights

* 🛍️ Product browsing
* ➕ Product management
* 📦 Order management
* 🤖 AI-powered product assistance
* 💬 Conversational product chatbot
* 🔍 Semantic product search
* 🧠 Vector embeddings
* ⚡ Similarity-based product retrieval

---

# 📸 Application Preview

## 🏠 Home Page

Browse available products through a simple and clean e-commerce interface.

<!-- Replace home.png with your actual screenshot filename -->

![Home Page](projects/home.png)

---

## ➕ Add Product

Add products to the application with details such as product name, description, price, and other relevant information.

Product information is persisted through the **Spring Boot backend and PostgreSQL database**.

<!-- Replace add-product.png with your actual screenshot filename -->

![Add Product](projects/add-product.png)

---

# 🤖 Ask AI

The **Ask AI** feature integrates Generative AI into the e-commerce experience.

Users can ask natural-language questions about products and receive intelligent responses instead of manually searching through product information.

### 💬 Example

> **User:** Suggest something useful for listening to music.

> **AI:** Based on the available products, wireless headphones would be a suitable option.

<!-- Replace ask-ai.png with your actual screenshot filename -->

![Ask AI](screenshots/ask-ai.png)

---

# 🔍 Semantic Product Search

One of the key features of this application is **Semantic Search**.

Traditional search relies primarily on exact keyword matching. Semantic search instead attempts to understand the **meaning and intent** behind the user's query.

### 💡 Example

Suppose the store contains:

> 🎧 **Wireless Headphones**

The user doesn't necessarily need to search for:

> `headphones`

They could search:

> `Something I can use to listen to music while travelling`

The system converts the query into a **vector embedding** and performs similarity search against product embeddings to retrieve semantically relevant products.

<!-- Replace semantic-search.png with your actual screenshot filename -->

![Semantic Search](screenshots/semantic-search.png)

---

## 🧠 How Semantic Search Works

```text
User enters a natural-language query
                 │
                 ▼
        Generate Query Embedding
                 │
                 ▼
          Vector Representation
                 │
                 ▼
      Compare with Product Vectors
                 │
                 ▼
       Vector Similarity Search
                 │
                 ▼
      Most Relevant Products
```

This enables product discovery based on **meaning rather than only exact words**.

---

# 💬 AI Product Chatbot

The application also includes an **AI-powered product chatbot**.

Users can interact with the chatbot conversationally to learn more about products available in the store.

### Example Questions

> 💬 "What products do you have?"

> 💬 "Tell me about the headphones."

> 💬 "Do you have something useful for entertainment?"

> 💬 "Which product would be suitable for listening to music?"

The chatbot provides contextual responses based on product information.

<!-- Replace chatbot.png with your actual screenshot filename -->

![AI Product Chatbot](screenshots/chatbot.png)

---

# 📦 Orders

The application includes an Orders section for viewing and managing product orders.

<!-- Replace orders.png with your actual screenshot filename -->

![Orders Page](screenshots/orders.png)

---

# 🏗️ Application Architecture

```text
                         ┌─────────────────┐
                         │      User       │
                         └────────┬────────┘
                                  │
                                  ▼
                         ┌─────────────────┐
                         │  E-Commerce UI  │
                         └────────┬────────┘
                                  │
                                  ▼
                    ┌────────────────────────┐
                    │      Spring Boot       │
                    │        Backend         │
                    └───────────┬────────────┘
                                │
             ┌──────────────────┼──────────────────┐
             │                  │                  │
             ▼                  ▼                  ▼
      ┌─────────────┐    ┌─────────────┐    ┌─────────────┐
      │ PostgreSQL  │    │  Spring AI  │    │ Embeddings  │
      │  Database   │    │    / LLM    │    │   Model     │
      └─────────────┘    └──────┬──────┘    └──────┬──────┘
                                │                  │
                                └────────┬─────────┘
                                         ▼
                                ┌─────────────────┐
                                │ Vector Similarity│
                                │      Search      │
                                └─────────────────┘
```

---

# 🛠️ Tech Stack

| Technology                  | Purpose                    |
| --------------------------- | -------------------------- |
| ☕ Java                      | Backend programming        |
| 🍃 Spring Boot              | Backend framework          |
| 🤖 Spring AI                | AI integration             |
| 🗃️ Spring Data JPA         | Data access                |
| 🔄 Hibernate                | ORM                        |
| 🐘 PostgreSQL               | Database                   |
| 🧠 Vector Embeddings        | Semantic representation    |
| 🔍 Vector Similarity Search | Semantic product retrieval |
| 🔗 REST APIs                | Application communication  |
| 📦 Maven                    | Dependency management      |
| 🧪 Postman                  | API testing                |
| 🔧 Git & GitHub             | Version control            |

---

# 🔤 Keyword Search vs 🧠 Semantic Search

| Traditional Search      | Semantic Search                                     |
| ----------------------- | --------------------------------------------------- |
| Exact keyword matching  | Meaning-based matching                              |
| Searches `"headphones"` | Can understand `"something for listening to music"` |
| Limited context         | Understands semantic similarity                     |
| Keyword dependent       | Vector embedding based                              |
| Less flexible queries   | Natural-language queries                            |

---

# 📂 Project Structure

```text
src/
└── main/
    ├── java/
    │   └── ...
    │       ├── controller/
    │       ├── service/
    │       ├── repository/
    │       ├── model/
    │       └── config/
    │
    └── resources/
        └── application.properties

# ⚙️ Getting Started

## 1. Clone the Repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

```bash
cd YOUR_PROJECT_NAME
```

## 2. Configure PostgreSQL

Configure the database connection in your environment/application configuration.

```properties
spring.datasource.url=YOUR_DATABASE_URL
spring.datasource.username=YOUR_DATABASE_USERNAME
spring.datasource.password=YOUR_DATABASE_PASSWORD
```

## 3. Configure AI

Add the required AI API credentials through environment variables.

```text
AI_API_KEY=your_api_key
```

> ⚠️ Never commit API keys, database passwords, or other credentials to GitHub.

## 4. Run the Application

```bash
mvn spring-boot:run
```

---

# 🎯 Key Technical Concepts Demonstrated

This project demonstrates practical implementation of:

**Backend Development**

* RESTful API development
* Layered architecture
* Spring Data JPA
* Hibernate ORM
* PostgreSQL integration

**Artificial Intelligence**

* Spring AI integration
* LLM interaction
* Vector embeddings
* Semantic similarity
* Natural-language queries
* AI-assisted product discovery

**Software Engineering**

* Separation of concerns
* API testing
* Database persistence
* Version control with Git

---

# 💡 What Makes This Project Different?

Instead of building only a traditional e-commerce CRUD application, this project explores how **Generative AI can improve product discovery**.

```text
Traditional E-Commerce
        +
     Spring AI
        +
 Vector Embeddings
        +
 Semantic Search
        +
   AI Chatbot
        =
AI-Powered Product Discovery 🚀
```

The application demonstrates how AI can be integrated into a real-world **Spring Boot backend** rather than existing as a standalone AI demo.

---

# 🔮 Future Enhancements

* 🔐 User Authentication & Authorization
* 🛒 Shopping Cart
* 💳 Payment Integration
* ❤️ Wishlist
* 🎯 Personalized Product Recommendations
* 📊 Admin Dashboard
* 🚚 Order Tracking
* 💬 Persistent AI Conversation History
* 🧠 Enhanced RAG-based Product Assistant

---

# 👨‍💻 Author

**Nandeshwar Reddy Challa**

B.Tech — Computer Science & Engineering

**Java | Spring Boot | Spring AI | PostgreSQL | Backend Development**

---

<div align="center">

### ⭐ If you like this project, consider giving it a star!

**Built with ☕ Java • 🍃 Spring Boot • 🤖 Spring AI**

</div>
