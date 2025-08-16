# 🤖 Project - BotLLM — AI Assistant for Your Internal Company Knowledge

## 🧠 Summary

This project was created for the WCHL25 hackathon. We focused on delivering a minimal but functional prototype that demonstrates the core value of our idea.

## 📌 One-liner  
BotLLM helps teams instantly access internal knowledge by combining company documents with a powerful AI assistant.

---

## 🧠 What is BotLLM?

**BotLLM** is a chatbot powered by Large Language Models (LLMs) that understands natural language and answers questions using your company's internal knowledge.

It connects to your internal documentation — such as sales guides, team policies, onboarding instructions — and allows employees to simply ask questions and get instant, relevant answers.

If the answer isn’t in the company knowledge base, the bot uses ChatGPT (or another LLM) as a fallback, clearly marked as AI-generated.

---

## 💡 Key Features

- 🤖 Natural language Q&A with company-specific answers 
- 📁 Connects to internal sources: PDFs, Notion, Google Docs
- 📫 Automatic fallback to general LLM when needed 
- 🧠 OpenAI/ChatGPT fallback integration  
- 🌐 Real-time answers in Web browser 
- 🧩 Modular, customizable architecture  

---

## 📸 Screenshots
<small>Bot interface: What’s our Q3 commission policy?</small>  

<img width="600" height="600" alt="What’s our Q3 commission policy?" text-align: center src="https://github.com/user-attachments/assets/90250b45-7c64-4ad4-883c-5450c2ed7a6f" />


<small>Answer extracted from internal company documentation</small> 

<img width="600" height="600" alt="Answer extracted from internal company documentation" text-align: center  src="https://github.com/user-attachments/assets/b73c90ed-14c3-4671-8673-9442f4cd71e4" />

---

## 🔧 How It Works

### Built with:
- 🦀 Rust (canisters written in Rust)
- 🧠 LLM assistant (architecture, construction, and material estimation)
- 💾 DFINITY (Internet Computer Protocol)

---

### 🧠 Architecture

- **Frontend**: HTML + JS (simple UI)  
- **Backend**: Rust + FastAPI  
- **AI**: OpenAI GPT-4, FAISS vector embeddings  
- **Hosting**: Internet Computer Protocol (ICP), GitHub Codespaces
- **Knowledge parsing**: Markdown / PDF to vector embeddings

---

## 🔐 Identity & Access

All logic is permissioned using identity signatures via the Internet Identity protocol. Canisters validate the caller for sensitive operations.

---

### 📁 Repository Structure

```bash
/frontend       # UI logic  
/backend        # API + vector search  
/canisters      # ICP canisters  
/scripts        # Deployment utilities  
README.md       # This file
```
---

## ▶️ Run Locally


## 💻 How It Works

1. Clone the repository:
   ```bash
   git clone https://github.com/hodoor6/Bot-LLM.git
   cd Bot-LLM

2. Install dependencies:
   ```bash
     npm install

3. Deploy canisters (local or testnet):
```bash
  dfx start --background
  dfx deploy
```

5. Run the app:
```bash
  npm run dev
```

(Optional) Deploy to ICP:

  ```bash
  dfx start --background
  dfx deploy
  dfx canister call <your_canister> <your_method>
```

### ▶️ Make sure you have:
- [DFINITY SDK](https://internetcomputer.org/docs/current/developer-docs/setup/sdk-installation/)
- Rust + cargo + `ic-cdk` libraries

### ▶️ How to create and deploy a canister to the mainnet IC

1. Install the dfx utility https://internetcomputer.org/docs/building-apps/getting-started/install
2. Start a local copy of dfx - dfx start
3. Create an identity in the local environment - dfx identity new <name of the hamman>. You can create an identity pattern to test your supplement.
4. Get the code  to get the cycles
5. Viconati command dfx wallet redeem-faucet-coupon <coupon code>
6. Check your dfx wallet balance - there may be 20 trillion cycles
7. Build your project - dfx build
8. Deploy the canister to the mainnet - dfx deploy --with-cycles <number of cycles> <canister name>

---

##  🎯 Example Use Case
A sales manager types:
Query: “What’s our Q3 commission policy?”
Response: BotLLM finds the relevant section in internal documents a company and returns a clear answer. 
If no match is found, it responds via ChatGPT and marks it as "AI-generated".

## 🚀 Why It Matters
Companies lose time and efficiency due to scattered, hard-to-access internal knowledge. BotLLM bridges this gap by becoming a “single point of truth” — instantly accessible, always available, smart enough to understand context.

##  🎥 Demo Video
🔗 Watch the live demo

🧑‍💻 Team

Mukoka – Product Manager & UI

Oleksii K.  – Backend Developer & AI 

Olena - Business Аnalyst & QA

DoraHacks IDs: @U_90a02c27cffd9b, @U_185657f84894f4

##  🔮 Plan further

✅ Role-Based Access Model (RBAC)

✅ Add real-time vector index updates

✅ Role-based access and chat history

✅ Slack & Teams integration

✅ Multilingual support

✅ Internal knowledge base integration (PDFs, Notion, Google Docs)

✅ UI polish + multi-language support



##  📫 Feedback

Telegram: @phpprogramist

Email: klimcukaleksey@gmail.com

🧪 Live demo: https://vyt5s-lqaaa-aaaak-quiuq-cai.icp0.io/

📄  DoraHacks BUIDL page: https://dorahacks.io/buidl/27122/

💻 GitHub https://github.com/hodoor6/Bot-LLM



## Contributors

- hodoor (@hodoor 6)


## License

This project is licensed under the MIT License.  
See the [LICENSE.md](LICENSE.md) file for more details.
