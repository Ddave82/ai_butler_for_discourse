# TheNode-Butler

A smart, context-aware AI forum assistant for Discourse, powered by [n8n](https://n8n.io) and [Mistral](https://mistral.ai).

<p align="center">
  <img src="assets/n8n.png" alt="n8n Workflow Overview" width="350"/>
</p>

---

## What is TheNode-Butler?

**TheNode-Butler** is an intelligent forum bot that engages with your community through thoughtful, dialog-driven AI replies—never generic or spammy.  
Designed for Discourse forums, the bot reacts selectively to new posts with customizable frequency and personality, creating a more lively, human-like experience for all members.

---

## Key Features

- **Contextual AI replies:** Powered by Mistral with a custom prompt, TheNode-Butler adds value to each conversation with relevant, reflective messages.
- **Configurable engagement:** Randomized reply probability (default: 38%) keeps the bot’s presence natural and non-intrusive.
- **Direct interaction:** When users reply directly to TheNode-Butler, it always responds.
- **Easy integration:** Built as a modular n8n workflow.  
- **Fully customizable:** Edit prompt, bot character, reply chance, and more for your community’s needs.
- **Self-hosted:** Keep control over your data and workflow.

---

## How It Works

1. **Post Detection:**  
   n8n checks the Discourse API for new posts every few minutes.

2. **Randomized Engagement:**  
   The bot decides—based on a configurable probability—whether to reply.

3. **AI-Powered Response:**  
   For selected posts, the content is sent to a Mistral AI model with a tailored prompt.

4. **Forum Posting:**  
   The AI-generated reply is posted back to the forum under the bot’s username.

5. **Reply-to-Bot Logic:**  
   When users reply directly to TheNode-Butler, it always responds (skipping the randomness).

6. **Memory Management:**  
   The bot saves the last processed post ID to avoid duplicate replies.

---

## Example Bot Reply

<p align="center">
  <img src="assets/botpost.png" alt="Example Bot Post" width="600"/>
</p>

---

## Getting Started

_Coming soon:_  
A clean n8n workflow export and setup instructions will be added here.  
The project is currently being prepared for open source release—stay tuned!

---

### Requirements

- A running [n8n](https://n8n.io) instance
- Discourse API access (API key, user)
- [Mistral AI](https://mistral.ai) or compatible API access

---

## Roadmap

- [x] Smart, context-aware AI replies  
- [x] Randomized engagement  
- [x] Direct reply-to-bot logic  
- [ ] Full workflow export  
- [ ] Setup and configuration guide  
- [ ] Multi-platform support (beyond Discourse)

---

## Contributing

Ideas, suggestions, and pull requests are very welcome!  
Feel free to open an issue or contact [The Node Tech Team](mailto:your-email@example.com).

---

## License

MIT License

---

*TheNode-Butler is developed by the community at [The-Node.tech](https://the-node.tech).*
