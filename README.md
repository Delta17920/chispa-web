# Chispa

![Chispa Banner](public/chispa-banner.png)

**Chispa** is an advanced AI-powered Go-to-Market (GTM) strategy platform designed for early-stage founders. It synthesizes fragmented insights, market data, and product details into structured, actionable guidance using cutting-edge AI—all wrapped in a stunning, high-performance interface.

## 🚀 Features

-   **🧠 AI GTM Engine**: Synthesizes inputs (industry, target market, product) into comprehensive GTM strategies, competitor insights, and positioning using **Python** & **AI**.
-   **📊 Interactive Dashboard**: A clean, actionable dashboard that provides pitch-ready outputs, capable of handling complex data visualization.
-   **🌍 Global Visualization**: Features an interactive World Map to visualize global reach and market data.
-   **⚡ Real-Time Processing**: Fast synthesis of market data and strategy generation.
-   **🎨 Modern UI/UX**: A sleek, accessible interface built with **Next.js 14** and **Tailwind CSS**, featuring **Aceternity UI** components and interactive animations.
-   **⚓ Floating Dock**: Seamless navigation across the application with a Mac-style floating dock.

## 🛠️ Tech Stack

### Frontend
-   **Framework**: [Next.js 14](https://nextjs.org/) (App Router)
-   **Styling**: [Tailwind CSS](https://tailwindcss.com/)
-   **Animations**: [Framer Motion](https://www.framer.com/motion/)
-   **Components**: [Aceternity UI](https://ui.aceternity.com/), [Tabler Icons](https://tabler-icons.io/)
-   **Fonts**: [Geist](https://vercel.com/font), [Kaushan Script](https://fonts.google.com/specimen/Kaushan+Script)

### Backend & AI
-   **Core Engine**: [Python 3.8+](https://www.python.org/)
-   **RAG & Orchestration**: Custom implementations (`src/`) using `langchain` (implied) or direct API calls.
-   **API Framework**: [FastAPI](https://fastapi.tiangolo.com/) (available in requirements, used for AI service endpoints)
-   **Utilities**: Tenacity, Pydantic

## 📋 Prerequisites

Before running the project, ensure you have the following installed:

1.  **Node.js** (v18 or higher)
2.  **Python** (v3.8 or higher)
3.  **Git**

## ⚙️ Installation & Setup

### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/chispa-web.git
cd chispa-web
```

### 2. Frontend Setup
Install the required Node.js dependencies.

```bash
npm install
# or
yarn install
```

### 3. AI Engine Setup (Python)
Set up the Python environment for the GTM strategy engine.

```bash
# Create virtual environment
python -m venv venv

# Activate virtual environment
# Windows:
venv\Scripts\activate
# Mac/Linux:
# source venv/bin/activate

# Install dependencies
pip install -r requirements.txt
```

## 🏃‍♂️ Running the Application

### Start the Development Server
Since this is a unified project structure, run the Next.js development server:

```bash
npm run dev
```
The application will be available at `http://localhost:3000`.

*(Note: Ensure your Python backend/scripts are running if they are required for specific features, or configured via Next.js API routes)*

## 📂 Project Structure

```bash
c:\chispa-web\
├── app/                 # Next.js App Router pages & API routes
├── components/          # React components (UI, Visuals)
├── public/              # Static assets (images, fonts)
├── src/                 # Python AI & RAG Engine
│   ├── agent_optimizer.py      # Optimization logic for agents
│   ├── embed_and_index.py      # Embedding generation script
│   ├── generate_strategy.py    # Core GTM strategy generation logic
│   ├── multimodal_processor.py # Processing for multimodal inputs
│   ├── rag_prepare.py          # Data preparation and indexing
│   ├── rag_retriever.py        # Retrieval logic for RAG
│   ├── components/             # Additional component modules
│   └── data/                   # Data handling scripts
├── rag_data/            # Dataset for RAG processing
├── build_index.py       # Script to build vector indices
├── requirements.txt     # Python dependencies
├── package.json         # Frontend dependencies
└── ...
```

## 🤝 Contribution
Contributions are welcome! Please fork the repository and submit a pull request for any enhancements or bug fixes.

## 📄 License
This project is licensed under the MIT License.
