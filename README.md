# Visual-Q-A
Interactive Visual Question Answering (VQA) with Streamlit
This project is an interactive web application that provides a user-friendly interface for a Visual Question Answering (VQA) model. It allows users to upload an image or provide an image URL, ask a question in natural language, and receive an AI-generated answer about the image's content.

The application leverages the power of the ViLT (Vision-and-Language Transformer) model, fine-tuned on the VQA v2 dataset, to understand both visual and textual inputs simultaneously.

🚀 Live Demo
(Optional) Add a link to your deployed Streamlit Community Cloud app here once it's live!
[Link to your deployed Streamlit App]

✨ Features
Interactive UI: A clean and simple web interface built with Streamlit.

Dual Input Methods: Users can either provide an image URL or upload a file (.png, .jpg, .jpeg) from their local machine.

Natural Language Questions: Ask questions in plain English.

Efficient Model Loading: The large VQA model is cached on startup to ensure fast inference times for subsequent requests.

Responsive Design: The interface is accessible on both desktop and mobile browsers.

⚙️ Technology Stack
Backend & ML Framework: PyTorch

Web Framework: Streamlit

VQA Model: Hugging Face Transformers for the ViLT model and processor.

Image Handling: Pillow

Web Requests: Requests

📦 Setup and Installation
Follow these steps to set up the project locally.

1. Clone the Repository
git clone [https://github.com/your-username/your-repo-name.git](https://github.com/your-username/your-repo-name.git)
cd your-repo-name

2. Create a Virtual Environment
It is highly recommended to use a virtual environment to manage project dependencies.

# Create the virtual environment
python -m venv venv

# Activate the virtual environment
# On Windows:
venv\Scripts\activate
# On macOS/Linux:
source venv/bin/activate

3. Install Dependencies
Install all the required libraries from the requirements.txt file.

pip install -r requirements.txt

▶️ How to Run
Once the setup is complete, you can run the Streamlit application with a single command:

streamlit run app.py

Your web browser will automatically open a new tab with the running application, usually at http://localhost:8501.

The first time you run the app, it will download the pre-trained ViLT model from Hugging Face, which may take a few minutes depending on your internet connection.

📁 Project Structure
vqa-streamlit-app/
│
├── app.py              # Main Streamlit application code
├── requirements.txt    # Project dependencies
└── README.md           # You are here!

🧠 Model Information
This application uses the dandelin/vilt-b32-finetuned-vqa model, a ViLT (Vision-and-Language Transformer) fine-tuned on the VQAv2 dataset. It is a powerful model capable of performing zero-shot VQA on a wide range of images and questions.

For more details, please refer to the model card on the Hugging Face Hub.
