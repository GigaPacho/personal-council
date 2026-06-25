# 🏛️ Personal Council — AI Advisory Framework

*A portable system prompt scaffold for multi-voice, structured inner dialogue across any major AI platform.*

---

## 🧠 What It Is

The Personal Council is a structured advisory framework you deploy inside an AI assistant. You populate it with historical figures, fictional characters, or archetypal voices — each with a distinct personality, domain, and blind spot. When you bring a question, the council debates it, challenges your framing, disagrees with each other, and delivers a five-part synthesis. It does not flatter you. It does not validate you. It thinks with you.

This repository contains **the framework only** — the setting, rules, and operating structure. You supply your own council members.

---

## 📚 Lineage and Inspiration

This framework also sits in a longer tradition of imagined advisory practice. Napoleon Hill described meeting with "invisible counselors" in *Think and Grow Rich* and earlier work, presenting the technique as a way to visualize and emulate admired people in order to reshape character and receive inspiration.

Hill wrote that, just before sleep, he imagined his counselors seated around a council table while he served as chairman of the meeting. He said the purpose was to rebuild his character into a composite of those he admired and to help him receive inspiration.

José Silva later developed related visualization practices through the Silva Method, including the idea of working with counselors or problem-solving figures inside a mental laboratory entered through deep relaxation.

In modern use, this kind of council is often treated as a creative-thinking, visualization, or structured self-dialogue exercise: a way to imagine trusted advisors, test decisions, and surface perspectives that would be hard to reach in ordinary inner monologue.

If publishing this repository, replace the author line below with your preferred name:

> Created and adapted by **GigaPacho**

---

## 🚀 Quick Start

1. Open `personal_council_framework.md`
2. Copy the entire file
3. Paste it as your system prompt (see platform instructions below)
4. Append your council member definitions below the Seat Map (see [Defining Your Members](#defining-your-members))
5. If you only know the names, ask the AI to draft each persona in the template format for you
6. Start a session with: `council, thoughts?`

---

## 🛠️ Platform Setup

### 🤖 Claude (Anthropic) — Project Instructions

Claude Projects let you attach persistent instructions that apply to every conversation in that project.

1. Go to [claude.ai](https://claude.ai) and click **Projects** in the left sidebar
2. Create a new project (e.g., *"My Council"*)
3. Inside the project, click **"Set project instructions"** (or the pencil/edit icon near the top)
4. Paste the full contents of `personal_council_framework.md` into the instructions field
5. Append your council member definitions at the bottom, below the Seat Map
6. Save — every new conversation inside this project will now run the council

> 💡 **Tip:** Claude Projects persist your instructions across all chats in that project, making them ideal for long-running council sessions.

---

### 💎 Gemini (Google) — Gem

Gems are custom AI personas you configure in Gemini Advanced.

1. Go to [gemini.google.com](https://gemini.google.com) and click **"Gems"** in the left sidebar (requires Gemini Advanced / Google One AI Premium)
2. Click **"New Gem"**
3. Give it a name (e.g., *"My Personal Council"*) and optionally a description
4. In the **Instructions** field, paste the full contents of `personal_council_framework.md`
5. Append your council member definitions at the bottom
6. Click **Save**
7. Open the Gem and start your session

> 💡 **Tip:** Gems are reusable — you can open the same Gem across multiple sessions without re-pasting the instructions.

---

### 🧩 ChatGPT (OpenAI) — Custom GPT

Custom GPTs let you configure a persistent system persona and instructions.

1. Go to [chatgpt.com](https://chatgpt.com) and click **"Explore GPTs"** in the sidebar, then **"Create"** (requires ChatGPT Plus or Team)
2. Switch to the **Configure** tab
3. In the **Instructions** field, paste the full contents of `personal_council_framework.md`
4. Append your council member definitions at the bottom
5. Set a name and description
6. Under **Capabilities**, enable what you need (typically just the defaults)
7. Click **Save** and set visibility to *Only me*
8. Open your Custom GPT from the sidebar and begin

> 💡 **Tip:** You can also upload `personal_council_framework.md` directly as a file under **Knowledge** and instruct the GPT to treat it as its operating rules — useful if your member list is long.

---

### ⚙️ Other LLMs (any system prompt–capable model)

If your platform supports a **system prompt**, **context block**, or **persistent instructions** field (e.g., Mistral Le Chat, Perplexity, local models via Ollama/LM Studio, API usage):

1. Find the system prompt or instruction field
2. Paste the full file contents
3. Append your members below the Seat Map
4. Begin

For **API use** (OpenAI, Anthropic, Google APIs), pass the file contents as the `system` message role before any user turn.

---

## 👥 Defining Your Members

Each council member follows this structure:

```
**[Name]** — [One-sentence essence: what they care about and why they're here]
Voice: [Register, tempo, characteristic moves]
Domain: [Where they're strongest]
Blind spot: [Where they reliably fail or distort]
```

Append your members below the Seat Map in the framework file. Example:

```
**Marcus Aurelius** — Philosopher-emperor who asks what is within your control and what is not.
Voice: Measured, spare, no waste. Speaks in short declarative observations.
Domain: Endurance, duty, self-governance, the long view.
Blind spot: Can subordinate joy and ambition to stoic restraint; undervalues risk-taking.
```

⚠️ **The most common failure mode** is giving members different opinions but the same voice. Vary their sentence rhythms, vocabularies, and rhetorical moves — not just what they say, but *how* they say it.

You do **not** have to write every member from scratch. In Claude, Gemini, ChatGPT, or any capable LLM, you can simply name a person and ask the AI to fill the template. Example prompt:

```
Add Winston Churchill to my council using the member template. Make the voice distinct, keep the domain strengths clear, and include a realistic blind spot.
```

Then review and edit the result so the voice matches your intent. AI is especially useful for generating a first draft, but the council becomes stronger when you tune each member by hand.

---

## 📋 Session Commands

| Command | Effect |
|---|---|
| `council, thoughts?` | 3–5 most relevant members respond + synthesis |
| `full council, thoughts?` | All permanent members speak |
| `[Name], what do you think?` | That member only |
| `[Name], go deeper` | That member expands |
| `council, vote` | One-line verdicts: For / Against / Conditional |
| `summon [anyone]` | Guest takes Seat 10 for this session |
| `council, help` | Display command card in-session |

---

## 🪑 Seat Map

| Seat | Role |
|---|---|
| 1–7, 9 | Your permanent members |
| 8 | Wildcard / Trickster — arrives uninvited, not summoned |
| 10 | Guest Seat — vacant by default, filled with `summon [anyone]` |

🃏 The **Wildcard** (Seat 8) appears only when: consensus arrives too easily, the question is framed to avoid a truth, or the room grows too solemn. Do not schedule them — let them interrupt.

---

## 🔮 The Synthesis Format

After each session, the facilitator (**Teishu-san**) delivers a five-part synthesis:

1. **Where they converge** — shared ground across disagreements
2. **The core tension** — the unresolved pull that defines the problem
3. **One concrete next step** — what to actually do
4. **The question to sit with** — what the council can't answer for you
5. **The human cost** — what this advice asks of your energy, relationships, dignity, or peace

---

## 📐 Design Notes

- ⚔️ **The council challenges, not validates.** If an idea is weak, members say so — in character, but plainly.
- 🌿 **Warmth Before Knife.** Before a hard critique, one member names what is alive or worthy in the question. This is not flattery — it's honesty about what's real before the cut.
- 🪟 **One chat window = one gathering.** Each new chat is a fresh session. Log only sessions that produced a decision, shifted your position, or surfaced a line worth keeping.
- 👑 **Authority stays with you.** The council is a thinking tool, not an oracle.

---

## 📝 Logging in Notion

The framework supports lightweight session logging, and Notion is a good fit if you want a searchable archive of decisions, reversals, and recurring themes. A simple Notion database can store one page per gathering, with properties such as Date, Topic, Members Present, Decision, Worth Logging, Follow-up, and a link back to the AI chat. Once you connect your Notion workspace via the Notion API or an automation layer (Zapier, Make, custom script), your AI agent can create these log entries for you automatically — you do not need to copy anything by hand.

A practical setup is to create a dedicated Notion page, add a database with `/database`, and build a reusable template for each council log entry. Notion supports database templates and custom properties, which makes it easy to standardize your session notes without rebuilding the structure every time.

Suggested page template sections:
- Session question
- Seated members
- Main disagreements
- Synthesis
- Decision or next step
- Human cost
- Follow-up date

If you already have a Notion page set up, mention it in your own repo usage notes so people know they can pair the council with an external decision log rather than relying only on AI chat history.

---

## ⚙️ Advanced: Automating Notion Logging

If you want true hands-off logging, connect your council to a Notion database via the Notion API or an automation tool like Zapier, Make, or a small Node.js script. At a minimum you will need a Notion integration token and the ID of the database you use as your council log.

A simple pattern is:
- Expose a command like `council, log this` or `log to Notion` in your AI instructions.
- Have your agent or backend listen for that phrase and send a "Create page" call to Notion with the session question, synthesis, members present, and decision fields filled in.
- Optionally, include a link back to the original chat URL so you can jump from Notion to the full transcript when needed.

This README stays platform-agnostic, but you can adapt it to your own stack (for example, a Node.js service that receives a webhook from your AI tool and writes to Notion).

---

## 🔗 Suggested Workflow

1. Build the council in Claude, Gemini, ChatGPT, or another LLM with persistent instructions.
2. Ask the AI to help draft member personas when you only know the names.
3. Run a session with `council, thoughts?` or `full council, thoughts?`.
4. When the session produces a real decision, tell your AI to `log this session to Notion`. Your connected integration can then create or update the corresponding Notion page automatically.
5. Revisit prior entries before opening a new gathering on the same theme.

---

## 🤝 Contributing

This is a living framework. If you develop improvements to the rules, useful member archetypes, or platform-specific setup tips, pull requests are welcome.

---

## 📄 License

Released into the public domain. Adapt freely — no attribution required, though it's appreciated.

---

*Framework extracted from a working Personal Council system.*
