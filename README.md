# 🕸️ AI Web Scraper

A simple web scraping app built with **Streamlit** and **Ollama (Llama3.1 model)**.  
With this app, you can:
- Paste any website URL
- Scrape and view the page content
- Ask the AI to extract specific information (like main headings, paragraphs, links, etc.)

---

## 🚀 Features
- User-friendly Streamlit interface
- Scrape website content instantly
- View cleaned DOM content inside the app
- Ask questions like *"Give me the main headings"* or *"List all links on the page"*
- AI-powered parsing with **LangChain + Ollama**

---

## 📦 Installation Guide

Follow these steps to set up the project on your system:

### 1. Clone the Repository
```bash
git clone <your-repo-url>
cd <repo-folder>
```
### 2. Install Dependencies
Make sure you have Python 3.8+ installed. Then run:
```bash
pip install -r requirements.txt
```
### 3. Install ChromeDriver (for Selenium)
- This project uses Selenium, which requires ChromeDriver.
- Download ChromeDriver
- Ensure the version matches your installed Google Chrome.
- Add ChromeDriver to your system PATH so Selenium can find it.
- 👉 Example: Place it in C:\Program Files\ChromeDriver\ (Windows) or /usr/local/bin/ (Linux/Mac).

### 4. Install and Set Up Ollama
- We use Ollama with the Llama3.1 model for AI parsing.
- Download and install Ollama from https://ollama.ai/
- Pull the Llama3.1 model:
```bash
ollama pull llama3.1
```
### 5. Make sure Ollama is running in the background before starting the app.
▶️ How to Run the App
- Start the Streamlit app:
```bash
streamlit run main.py
```
- After running, Streamlit will give you a local URL like:
http://localhost:8501

- Open it in your browser to use the app.
### 📂 Project Structure

```plaintext
├── main.py          # Streamlit app (UI for scraping and parsing)
├── scrape.py        # Functions to scrape and clean webpage data
├── parse.py         # AI-powered parsing using Ollama (Llama3.1)
├── requirements.txt # Python dependencies
```

### 📝 Notes
- Works on Python 3.8 or higher
- Requires Google Chrome + ChromeDriver for Selenium
- Requires Ollama (make sure it’s running before you parse content)
- Designed for simple scraping and extracting insights, not heavy-duty crawling

### 🤝 Contributions
- Feel free to fork this repo, improve the scraper, and submit pull requests. 🚀
