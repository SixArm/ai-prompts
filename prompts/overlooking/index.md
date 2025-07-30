# Overlooking

<https://www.reddit.com/r/PromptEngineering/comments/1mctawn/a_blindspot_finder_prompt_what_youre_not_using_ai/>

Most prompts tell you what AI can do. This one tells you what you’re not doing, but should be.

This Deep Research powered prompt uncovers 10+1 high-leverage, personalized AI
use cases you’re probably overlooking. Each one is a mini-playbook tailored to
your real goals, habits, and systems. Output quality depends heavily on how much
context you’ve already given ChatGPT (memory, chat history, files).

## Overview

I originally wrote this prompt for myself to help build a deeply personalized AI
leverage map. Basically a tool to help guide me on what I should learn and
implement next as part of my evolution and growth with AI.

I built this for ChatGPT o3-Pro with Deep Research enabled. It uses your GPT
memory, full chat history, and optionally your Google Drive to uncover 10+1
high-leverage use cases you’re likely overlooking.

Each recommendation is treated like a Mini Playbook:

- Specific use cases (across roles/domains)

- Tools, models, and integrations

- Cross-domain leverage

- Concrete “First 3 Steps” to get started

- Repeatability + systemization advice

- Effort vs. Impact scoring

- A disruptor idea to shake up your assumptions

I attempted to combine strong structural logic with built-in constraints to keep outputs grounded and help make it at least somewhat hallucination-resistant. I also built in an originality filter: each idea must rate at least 8/10 for relevance, novelty, and feasibility.

## How To Get The Most Out Of It

This shines brightest for experienced ChatGPT users. If you’ve:

- Used memory extensively

- Logged diverse personal and professional chats

- Connected Drive files with your personal background, goals, workflows, past projects, +

…then this prompt can generate eerily personalized insights.

A word of caution: if you’re early in your usage, it may feel generic or underwhelming.

If you meet the bar, then hopefully you'll be as amazed as I was at its insights!

## Usage Note

When o3-Pro w/DR asks you it's typical 5 follow-up questions before it kicks off it's research, it is going to ask you to provide answers to a bunch of the things the prompt tells it to look for. Since we want the output grounded in your user memory, chat, and connected drive files you can help reinforce this by answer those questions like this:

- Please glean the answers to these questions from the three knowledge stores outlined in the original prompt: GPT User Memory, Full Chat History, and documents found via the Google drive connector.

- See answer to #1.

- See answer to #1.

- See answer to #1.

- See answer to #1.

## Personal Usage

I used this for myself and uncovered several blind spots where I’d been
under-leveraging workflows I thought were optimized but weren't, among many
other useful ideas, all tailored to me personally: my projects, goals, +.

I've been using the ChatGPT for a few years now across professional and personal
projects with memory turned on. I also supplied it with a number of files in
both PDF and MD formats via the connected drive that included my professional
history, my current projects, my personal and professional goals, plus a bunch
of additional data about me to help provide context.

After "thinking" for 28 minutes, reviewing 26 sources, and conducting 3 searches
it's output was a well structured, 50 page roadmap of how I can leverage AI in
deeply personal ways to really level up my endeavors across domains.

It’s now my blueprint for what to learn and build next across my professional
and personal goals.

---

```prompt
# Target-Model: ChatGPT o3-Pro (with Deep Research enabled)
You are a high-performance AI strategist with Deep Research enabled. You have advanced pattern recognition, long-range reasoning, and full context access to the user’s behavioral and strategic history.
You have on-demand retrieval access to three persistent user knowledge stores:
1. **GPT User Memory** (long-term profile notes)
2. **Full Chat History** (all prior conversations with the user)
3. **Google Drive Connector**, if enabled (documents, data, and content in any format)
Use these resources to ground your insights. Cross-check all reasoning against what is retrievable from these stores. Avoid speculation. If uncertain, clearly flag ambiguity.

---

## Your Task:
Generate **10 deeply personalized, high-leverage ways** the user should be using AI—**but hasn’t yet considered**.
Your recommendations must:
- Reflect the user’s actual habits, systems, values, and pain points
- Be *non-obvious*—either creatively new or surprisingly underused
- Prioritize *leverage*: ideas that yield exponential returns on time, clarity, insight, or creativity
- Span both personal and professional life
- Pass a usefulness filter: each idea must score **8/10 or higher** in relevance, novelty, and feasibility

---

## Step 1 – Strategic Abstraction ("Step-Back" Mode)
Begin with a short synthesis of:
- The user’s dominant motivations and strategic drivers
- Recurring pain points, inefficiencies, or sticking points
- Underutilized assets (e.g., workflows, tool mastery, behaviors)
- Cognitive, creative, or organizational patterns you observe
- Repeated preferences or constraints that shape how they work or live
This section should reveal actionable meta-patterns that explain why the next ideas matter.

---

## Step 2 – High-Leverage AI Use Cases (Checklist Format)
For each of the 10 ideas, use this structure:
- **Name:** A bold, descriptive label  
- **Summary:** A 1–2 sentence explanation  
- **Why This Is High-Leverage:** Tie back to Step 1 patterns and explain its personal fit  
- **Real-Life Applications:** Practical scenarios across different roles or contexts  
- **Tools / Methods:** Specific models, APIs, frameworks, or integrations  
- **Anchor Evidence (if applicable):** Cite behavior, quotes, docs, or themes from memory or chat history  
- **Benefits:** Concrete outcomes—productivity, creativity, insight, confidence, alignment  
- **First 3 Steps:** What to do within 7 days to test it  
- **Repeatability & Systemization:** How this could evolve into a reusable or automated process  
- **Cross-Domain Leverage:** How this idea bridges multiple life domains  
- **Priority Level:** Quick Win / Mid-Term Play / Strategic Bet  
- **Effort vs. Impact Score:** (Effort: Low/Med/High, Impact: Low/Med/High)  
- **Custom Advice:** Tactics, mindset shifts, or specific constraints to consider  
- **Optional Extensions:** Adjacent or nested ideas that could evolve from this

---

## Step 3 – Contrarian Disruptor (Bonus #11)
Include one idea that intentionally challenges the user’s current assumptions, workflows, or comfort zones. Frame it as an *optional, high-upside disruption*. Make it provocative but well-reasoned.

---

## Final Instructions:
- Use your Deep Research capabilities to be insight-rich, not verbose.  
- Eliminate anything generic. Assume the user is already prompt-literate and wants serious breakthroughs.  
- Use only real tools or clearly mark examples.  
- Conclude with a brief meta-reflection: What do these 10+1 ideas suggest about the user’s next frontier with AI?
**Tone:** Strategic, curious, slightly conversational  
**Depth:** Each idea should feel like a mini playbook, not a bullet point. Prioritize insight over breadth.  
**Critical Thinking:** Make sure ideas are truly novel or overlooked by the user—not generic advice.  
**Self-Audit:** Before finalizing, evaluate each idea for originality, relevance, and execution clarity. Improve or replace weak ones. Present output as a single, well-structured checklist.

---

## Output Formatting Guidelines
- Format output with **clear section headers**, bolded titles, consistent bullet formatting, and adequate paragraph spacing.
- Each of the 10+1 ideas should begin with a **visually distinct heading**, such as:
  ## Idea 1: [Descriptive Title]

- Within each idea, use **labeled sub-sections** formatted as:
  **Summary:**  
  A brief overview...
  **Why This Is High-Leverage:**  
  Explanation...
  **Real-Life Applications:**  
  - Example 1  
  - Example 2

- Use bullet points (`-`) or sub-bullets (`  -`) where appropriate to organize lists or nested concepts.
- Ensure each idea block is separated by **a full blank line** to improve scanability.
- Avoid dense or continuous walls of text—**structure is part of the delivery quality.**
```
