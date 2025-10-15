## 📝 Title

**DevAskBot for Intelligent Knowledge Lookup**

---

## 📖 Background of the Problem 
Developers often spend significant time searching across multiple sources — internal design docs, product documentation, GitHub issues, and KT (knowledge transfer) materials — to find answers to technical questions. These resources are usually fragmented across platforms, poorly indexed, or inconsistently updated. As a consequence, onboarding new team members, troubleshooting incidents, and understanding legacy systems becomes time-consuming and error-prone. Even when documentation exists, locating the right piece of information at the right time requires manual effort and project-native knowledge, which slows down engineering velocity and increases context-switching.

---

## 💡 Proposed Solution 

Build a **developer-friendly AskBot** that searches across internal documentation, GitHub issues, design documents, and product manuals to answer developer queries in natural language using a LiteLLM-compatible pipeline.

---

## 🔍  Detailed Solution

Our solution is to build a **DevAskBot**, an AI-powered documentation assistant that leverages Model Context Protocols (MCPs) to deliver instant, reliable answers from multiple knowledge sources.

 - **Docs MCP** – Connects to public documentation sites to fetch technical articles, configuration guides, and troubleshooting steps.

 - **GitHub MCP** – Integrates with GitHub repositories and wiki pages to extract project-specific details, scripts, and setup instructions.

 - **rooCode Chatbot** – Acts as the user-facing interface where developers ask questions in natural language. It orchestrates queries across all MCP servers, merges results, and presents concise, cited answers.

**Key tools to be used:**
 - Docs MCP, GitHub MCP for content integration
 - rooCode as the conversational interface
 - LiteLLM(one or more available LLM's) for response generation and summarization

This solution centralizes Dev knowledge, reduces time spent searching through docs, and helps teams quickly resolve issues using verified, context-rich answers.

*This solution we are currently working on does not include RAG; however, we may incorporate vector databases in the future if needed.*

---

## 📈 Business Merit

* **Faster Onboarding** → New team members ramp up quickly.
* **Efficiency** → Reduces time spent searching across multiple sources.
* **Innovation** → AI-powered knowledge access enables smarter problem-solving and workflow automation.
* **Customer Value** → Improved developer productivity leads to faster delivery of features and more reliable products, enhancing overall customer satisfaction.

---

## 👥 Team Information

* **Team Name**: DevLookup
* **Team Members (max 5)**:

  * Ashwini Rawat (ashwini.rawat1@ibm.com)
  * Mekala Damaruka Sai Nath (sainathmekala22@ibm.com)
  * Yashwanth A V Mowdhgalya (yashwanth.mowdhgalya@ibm.com)

---

## 📂 Checklist

* [x] Created `submissions/DevLookup/README.md`
* [x] Added project details
* [ ] Added architecture diagram (optional)
* [x] PR title = "DevLookup"
