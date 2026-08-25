# ⚡ FastAPI CRUD REST API

> A Python-based CRUD REST API built with FastAPI and Pydantic, with a Streamlit client for interacting with and testing HTTP endpoints.

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat&logo=fastapi&logoColor=white)
![Pydantic](https://img.shields.io/badge/Pydantic-E92063?style=flat)
![REST API](https://img.shields.io/badge/REST%20API-4E79A7?style=flat)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat&logo=streamlit&logoColor=white)

---

## 📌 Overview

This project demonstrates how to build and interact with a **RESTful API using FastAPI**.

The API provides CRUD operations for managing item data, while a simple **Streamlit client** is included to interact with selected API endpoints through a graphical interface.

The project focuses on understanding the fundamentals of:

- REST API development
- HTTP methods
- Request and response handling
- Data validation with Pydantic
- CRUD operations
- API-client communication
- FastAPI automatic documentation

The overall architecture is:

```text
┌──────────────────┐
│  Streamlit Client│
│                  │
│  Create / Get    │
└────────┬─────────┘
         │
         │ HTTP Request
         ▼
┌──────────────────┐
│     FastAPI      │
│                  │
│ GET / POST       │
│ PUT / PATCH      │
│ DELETE           │
└────────┬─────────┘
         │
         ▼
┌──────────────────┐
│    In-Memory DB  │
│    fake_db       │
└──────────────────┘
