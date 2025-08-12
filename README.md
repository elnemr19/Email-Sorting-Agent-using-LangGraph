# 📧 Email Sorting Agent using LangGraph

An AI-powered **Email Sorting Agent** that processes incoming emails, classifies them as **spam** or **legitimate**, and drafts professional responses for legitimate messages.  
Built using **LangGraph**, **LangChain**, and **Groq LLaMA 3** models, with **Langfuse** integration for full traceability and debugging.



<img width="433" height="694" alt="image" src="https://github.com/user-attachments/assets/3ca7343f-66aa-429d-877d-be72055502b0" />


---

## 🚀 Features

- **Automated Email Classification**  
  Uses LLaMA 3 via Groq to detect spam vs. legitimate ("ham") emails.

- **Drafting Polite Responses**  
  For legitimate emails, the agent creates a professional draft for the user to review.

- **Spam Handling**  
  Moves spam emails to a virtual "spam folder" with a reason.

- **Custom Workflow with LangGraph**  
  Implements a state-based graph to process emails step-by-step.

- **Observability with Langfuse**  
  Monitors, traces, and debugs every run of the agent.

---

## 🛠️ Tech Stack

- **[LangGraph](https://github.com/langchain-ai/langgraph)** – Workflow orchestration with state graphs.
- **[LangChain](https://www.langchain.com/)** – LLM integration and message handling.
- **[Groq](https://groq.com/)** – Fast inference with LLaMA 3 (70B model).
- **[Langfuse](https://langfuse.com/)** – Observability and tracing for AI applications.
- **Python** – Core programming language.
- **Google Colab** – Development environment.

---


## 🧠 How It Works

1. **Read Email** – The agent logs sender and subject.

2. **Classify Email** – Groq LLaMA 3 model determines if it’s spam or ham.

3. **Spam Handling** – If spam, it's moved to the spam folder.

4. **Draft Response** – For ham, the agent drafts a polite, professional reply.

5. **Notify User** – Displays the draft response for user review.

6. **Trace with Langfuse** – Every step is tracked for debugging.

---

## 🖥️ Example Output

### Legitimate Email

```vbnet
Processing legitimate email...
An AI Agent is processing an email from Cognizant AI with subject: Potential partnership !
ham

==================================================
Hello, I am your AI Agent. You have received an email from Cognizant AI.
Subject: Potential partnership !

I've prepared a draft response for your review:
--------------------------------------------------
Subject: Re: Potential partnership !

Dear Cognizant AI Team,

Thank you for reaching out to explore a potential partnership with Vizuara...
==================================================
```
### Spam Email

```vbnet
Processing spam email...
An AI Agent is processing an email from Crypto bro with subject: The best investment of 2025
spam
Alfred has marked the email as spam.
The email has been moved to the spam folder.
```


---

## 📊 Langfuse Integration

This project uses **Langfuse** for:

- Real-time tracing

- Performance monitoring

- Debugging agent runs



