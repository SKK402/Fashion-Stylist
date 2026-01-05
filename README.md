# 🧥 AI-Driven Fashion Styling Assistant

An **AI-powered multimodal fashion styling assistant** that combines **image similarity search** with **generative AI** to provide personalized outfit and styling recommendations. Users can upload fashion images or enter text-based queries to receive visually grounded fashion advice.

---

## ✨ Features

- Image-to-image fashion retrieval using vector similarity  
- Text-to-image fashion search using natural language queries  
- Multimodal AI-generated styling recommendations  
- Persistent vector database for fast image retrieval  
- Interactive web interface built with Streamlit  

---

## 🧠 How It Works

1. Fashion images are loaded from the Fashionpedia dataset  
2. Images are converted into embeddings using OpenCLIP  
3. Embeddings are stored in a persistent ChromaDB vector database  
4. Users upload an image or enter a text query  
5. Similar images are retrieved using vector similarity search  
6. A multimodal AI model generates contextual fashion recommendations  

---

## 🛠️ Tech Stack

Python, Streamlit, Google Gemini API (Multimodal AI), ChromaDB, OpenCLIP Embeddings, Fashionpedia Dataset, NumPy, Pillow (PIL), PyTorch, dotenv, Git & GitHub

---

## 📁 Project Structure

AI-Driven-Fashion-Stylist-BOT-
├── main.py              # Streamlit app and AI integration
├── load_data.py         # Load and save Fashionpedia images
├── store_embed.py       # Generate and store image embeddings
├── torch_test.py        # PyTorch environment validation
├── Data/                # Fashion image dataset
├── Vector_database/     # ChromaDB persistent storage
├── .env                 # Environment variables
└── README.md

## ⚙️ Installation & Setup
1. Clone the Repository
`git clone https://github.com/SKK402/AI-Driven-Fashion-Stylist-BOT-.git
cd AI-Driven-Fashion-Stylist-BOT-`
2. Install Dependencies
`pip install -r requirements.txt`
3. Set Environment Variables
`Create a .env file in the root directory:
api_key=YOUR_GEMINI_API_KEY`

## 🚀 Running the Project
1. Load the Dataset
`python load_data.py`

2. Store Image Embeddings
`python store_embed.py`

3. Launch the Application
`streamlit run main.py`

## 📌 Use Cases

1.AI-based virtual fashion assistants

2.Multimodal recommendation systems

3.Image similarity search applications
