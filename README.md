 E-Commerce LLM-Based Recommendation System — by Somya Gupta

This project is an AI-powered e-commerce recommendation system that combines traditional recommendation logic with Large Language Model (LLM)-driven explanations. It not only recommends relevant products to users but also provides human-like explanations for why those products were suggested.

GitHub: somyagpt/E-Commerce-Recommendation
 
GitHub

⚙️ Tech Stack

Backend: FastAPI

Database / ORM: SQLModel

Vector Store / Embeddings: Qdrant

LLM Integration: OpenAI / Gemini API (or your preferred LLM)

Language: Python

🧩 System Workflow

Data Layer:

Stores product metadata, categories, and user interactions (views, clicks, purchases).

Embeds product descriptions into vector space and stores them in Qdrant.

Recommendation Module:

Retrieves similar items using embeddings (e.g. cosine similarity).

Uses user behavior history + product metadata to choose the top candidate products.

LLM Explanation Module:

Generates natural language explanations, e.g.

“This product is recommended because you viewed items from the same category”

API Layer (FastAPI):

Endpoints like:

/recommendations/{user_id} → returns recommended products

/explain/{product_id} → returns an explanation

(Optional) Frontend:

Simple UI to display product recommendations along with explanations.

🎯 Key Features

Personalized recommendations based on embeddings + behavior

Transparent explanations using LLM

Modular architecture—easy to extend

RESTful API endpoints for integration
