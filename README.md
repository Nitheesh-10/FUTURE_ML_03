💬 AI-Powered Customer Support Chatbot

An intelligent Customer Support Chatbot built using Gradio, FastAPI, LangChain, and OpenAI, designed to automate and enhance customer interactions.
This chatbot can answer FAQs, retrieve context-aware information, and provide instant responses — improving customer experience and reducing support workload.

🚀 Features

🤖 AI-driven responses using OpenAI API

🧠 Contextual question answering with LangChain

📚 Knowledge base integration (FAQs or support documents)

🔍 Vector similarity search powered by ChromaDB

⚡ Fast backend with FastAPI

💻 Interactive frontend built with Gradio

🏗️ Project Architecture
Gradio (Frontend)
     ⬇️
FastAPI (Backend)
     ⬇️
LangChain + ChromaDB (Knowledge Retrieval)
     ⬇️
OpenAI API (Response Generation)

📂 Folder Structure
customer-support-chatbot/
│
├── app.py                  # Main FastAPI backend
├── chatbot_interface.py    # Gradio frontend script
├── requirements.txt        # Required dependencies
├── kb/
│   └── faqs.csv            # Knowledge base with FAQs
└── README.md               # Project documentation

⚙️ Installation & Setup
1️⃣ Clone the repository
git clone https://github.com/your-username/customer-support-chatbot.git
cd customer-support-chatbot

2️⃣ Create a virtual environment
python -m venv venv
source venv/bin/activate   # for Mac/Linux
venv\Scripts\activate      # for Windows

3️⃣ Install dependencies
pip install -r requirements.txt

4️⃣ Add your OpenAI API key

Create a .env file in the project root:

OPENAI_API_KEY=your_api_key_here

5️⃣ Run the FastAPI backend
uvicorn app:app --reload

6️⃣ Launch the Gradio frontend
python chatbot_interface.py


The chatbot will open in your default browser. 🎉

🧠 Example FAQs (faqs.csv)
title,content
"How to reset password","Go to Settings > Reset Password. You’ll receive an email link to create a new password."
"Refund policy","We offer refunds within 30 days if the product is unused and in original packaging."
"Shipping time","Standard shipping takes 3-5 business days. Express options available at checkout."
