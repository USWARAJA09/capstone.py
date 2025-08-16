News Validity Verifier AI

This project is an AI-powered fact-checking pipeline built using CrewAI, LangChain, and Gradio.
It verifies the accuracy of any news article or social media post by:

✔️ Extracting factual claims
✔️ Searching credible sources
✔️ Detecting political/emotional bias
✔️ Verifying claims against evidence
✔️ Producing a simple Truth Snapshot summary
🚀 Features

Claim Extraction → Pulls key factual statements from input news.

Web Research → Gathers 5–10 supporting or contradicting sources per claim.

Bias Detection → Rates the tone, political leaning, or emotional manipulation in the text.

Fact Verification → Labels claims as True ✅, Misleading ⚠️, or False ❌.

Truth Snapshot Report → Generates a concise and shareable summary.

Gradio Interface → User-friendly web UI for entering news and viewing results.
🛠️ Tech Stack

Python 3.10+

CrewAI – Multi-agent workflow framework

LangChain – LLM orchestration

Gradio – Web interface for user input/output

OpenAI GPT (via langchain_openai) – LLM backbone

📂 Project Structure🛠️ Tech Stack

Python 3.10+

CrewAI – Multi-agent workflow framework

LangChain – LLM orchestration

Gradio – Web interface for user input/output

OpenAI GPT (via langchain_openai) – LLM backbone

📂 Project Structure
news-validity-verifier/
│── app.py               # Main Gradio interface
│── agents.py            # Definition of all CrewAI agents
│── tasks.py             # Task pipeline using CrewAI
│── .env                 # Stores OpenAI API key
│── requirements.txt     # Python dependencies
│── README.md            # Documentation

⚙️ Installation

Clone the repo

git clone https://github.com/your-username/news-validity-verifier.git
cd news-validity-verifier


Install dependencies

pip install -r requirements.txt


Set up environment variables
Create a .env file in the root directory and add your OpenAI key:

OPENAI_API_KEY=your_api_key_here

▶️ Usage

Run the Gradio app

python app.py


Open the provided local URL in your browser.

Paste any news text or article snippet into the input box.

Get a step-by-step fact-checking analysis with a final Truth Snapshot.

🧠 Agents Overview

News Verifier → Extracts factual claims.

Web Crawler → Finds credible supporting/contradicting sources.

Bias Detector → Rates political/emotional bias.

Agent Nova → Verifies claims against external evidence.

Agent Echo → Creates a simplified, shareable Truth Snapshot.

📊 Example Output

Input:
"The government announced that inflation dropped to 5% in July."

Output:

Claim 1: Inflation dropped to 5% in July.

Evidence: [World Bank], [Reuters], [Gov Report]

Bias: Neutral

✅ True

Truth Snapshot:
✔️ Claim 1: True – Inflation data confirmed by official statistics.

✅ Roadmap

 Add live web search integration

 Support multiple languages

 Deploy on Vercel / Hugging Face Spaces

 Add a database of verified claims for faster lookups

🤝 Contributing

Fork this repository

Create a feature branch (git checkout -b feature-name)

Commit changes (git commit -m "Added new feature")

Push branch (git push origin feature-name)

Open a Pull Request

📜 License

This project is licensed under the MIT License.
