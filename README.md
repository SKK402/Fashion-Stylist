🧥 AI-Driven Fashion Styling Assistant

An AI-powered multimodal fashion styling assistant that provides personalized outfit recommendations using image similarity search and generative AI. Users can upload clothing images or enter text-based styling queries to receive fashion advice enhanced by visual context.

🚀 Features

📷 Image-Based Fashion Retrieval
Upload an image and retrieve visually similar fashion items using vector similarity search.

🧠 AI-Powered Styling Recommendations
Uses a multimodal generative AI model to analyze clothing images and generate detailed styling advice.

🔍 Text-to-Image Search
Enter styling queries (e.g., “black formal blazer”) to retrieve relevant fashion images.

🗂️ Persistent Vector Database
Stores and retrieves image embeddings efficiently for fast similarity search.

🖥️ Interactive Web Interface
Built with Streamlit for seamless user interaction.

🧠 System Architecture (High-Level)

Fashion images are loaded from the Fashionpedia dataset

Images are embedded using OpenCLIP

Embeddings are stored in ChromaDB

User uploads an image or enters a query

Similar images are retrieved from the vector database

Gemini multimodal model generates fashion recommendations

🛠️ Tech Stack

Python, Streamlit, Google Gemini API (Multimodal AI), ChromaDB, OpenCLIP Embeddings, Fashionpedia Dataset, NumPy, Pillow (PIL), PyTorch, dotenv, Git & GitHub

📂 Project Structure
├── main.py            # Streamlit app (UI + AI integration)
├── load_data.py       # Loads and saves Fashionpedia images
├── store_embed.py     # Generates and stores image embeddings in ChromaDB
├── torch_test.py      # PyTorch and CUDA environment check
├── Data/              # Fashion image dataset
├── Vector_database/   # Persistent vector database
├── .env               # API keys and environment variables
└── README.md

⚙️ Setup Instructions
1️⃣ Clone the Repository
git clone https://github.com/SKK402/AI-Driven-Fashion-Stylist-BOT-.git
cd AI-Driven-Fashion-Stylist-BOT-

2️⃣ Install Dependencies
pip install -r requirements.txt

3️⃣ Set Environment Variables

Create a .env file:

api_key=YOUR_GEMINI_API_KEY

4️⃣ Load Dataset
python load_data.py

5️⃣ Store Image Embeddings
python store_embed.py

6️⃣ Run the Application
streamlit run main.py

📌 Use Cases

Virtual fashion styling assistants

AI-powered wardrobe recommendation systems

Multimodal retrieval and recommendation research

Computer vision + LLM integration demos

🔮 Future Improvements

User preference profiling

Outfit compatibility scoring

Full wardrobe management

Deployment on cloud platforms

Mobile app integration
