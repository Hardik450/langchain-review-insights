

# 🧠 langchain-review-insights

**LLM-powered Review Analysis using LangChain and Gemini**
This project analyzes product reviews using Large Language Models (LLMs), detects sentiment, and extracts structured insights such as summaries and highlights — all integrated using the LangChain framework and Gemini 2.0 Flash.

---

## 🚀 Features

* 🔍 **Sentiment Classification** (Positive / Neutral / Negative)
* 🧾 **Summary Generation** for each review
* 📦 **Structured Output Parsing** using `StructuredOutputParser`
* 🧠 **Prompt Engineering** with `from_template` and `format_messages`
* 🤖 **Powered by Gemini** via `ChatGoogleGenerativeAI`
* 🧪 Easily extendable to classify topics, emotions, or extract custom fields

---

## 📦 Installation

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/langchain-review-insights.git
cd langchain-review-insights
```

### 2. Set Up Environment

```bash
python -m venv venv
source venv/bin/activate   # On Windows use: venv\Scripts\activate
pip install -r requirements.txt
```

### 3. Add Environment Variables

Create a `.env` file in the root directory:

```
GOOGLE_API_KEY=your_gemini_api_key
```

---

## 🧠 Tech Stack

| Tool                   | Purpose                            |
| ---------------------- | ---------------------------------- |
| **LangChain**          | LLM framework and chains           |
| **Gemini (2.0 Flash)** | LLM backend (Google Generative AI) |
| **Python**             | Core programming language          |
| **dotenv**             | Manage environment variables       |

---

## 🛠️ How It Works

1. User provides a set of product reviews.
2. LangChain builds a prompt using `ChatPromptTemplate.from_template`.
3. Gemini processes the prompt and returns a structured JSON.
4. The JSON includes:

   * Review Summary
   * Sentiment (Positive / Neutral / Negative)
   * Highlights
   * Summary

---

## 📝 Sample Output

```json
{
  "sentiment": "positive",
  "highlights": "Bright Screen, and integration with phone",
  "summary": "The smartwatch is reliable for fitness tracking with a bright screen and good phone integration.",
}
```


## 🤝 Contributing

Feel free to fork this repo and raise a pull request. Contributions, ideas, and feedback are welcome!

---

## 📜 License

This project is licensed under the [MIT License](LICENSE).

