# 💸 FinAdvise – Personal Finance Assistant

**FinAdvise** is an AI-powered personal finance assistant that helps users manage finances, track expenses, monitor stocks, create budgets, and get personalized financial advice. Built using **LangGraph** and **Python**, it provides an interactive conversational interface to simplify financial management.

---

## **Project Description**

FinAdvise allows users to interact with their finances through a friendly chat interface. The bot can:

* Collect user profile information (age, income, financial goals, risk tolerance)
* Track expenses and maintain short-term memory of transactions
* Fetch real-time stock information and provide tailored advice based on risk tolerance
* Generate empathetic and clear budget summaries
* Offer personalized financial guidance based on user input and previous advice
* Flag high-risk queries for human-in-the-loop review to ensure safety

---

## **Features**

* **Intent Detection:** Classifies user queries into `profile`, `stock`, `expense`, `budget`, `advice`, or `unknown`.
* **User Profile Collection:** Dynamically extracts and updates user profile details.
* **Stock Information:** Integrates with **Alpha Vantage API** to fetch stock prices and provide tailored advice.
* **Expense Tracking:** Logs and confirms user expenses with clear feedback.
* **Budget Summary:** Generates simple, empathetic budget summaries.
* **Personalized Advice:** Provides financial recommendations suited to the user's profile and history.
* **Human-in-the-Loop (HITL):** Flags high-risk requests for review by a human financial advisor.
* **Interactive Chat Interface:** Built with Streamlit, maintaining session-based memory for a seamless experience.

---

## **Technologies**

* LangGraph
* Python 3.10+
* Streamlit

---

## **Installation & Setup**

1. **Clone the repository**

```bash
git clone https://github.com/ShreyashBansod16/FinAdvisor.git
cd FinAdvisor
```

2. **Create a virtual environment and install dependencies**

```bash
python -m venv venv
# Activate the virtual environment
# Windows: venv\Scripts\activate
# Mac/Linux: source venv/bin/activate
pip install -r requirements.txt
```

3. **Set up environment variables**
   Create a `.env` file in the project root:

```env
GROQ_API_KEY=your_groq_api_key
VANTAGE_API_KEY=your_alpha_vantage_api_key
```

4. **Run the Streamlit app**

```bash
streamlit run app.py
```

> Replace `app.py` with the name of your main Streamlit script if different.
