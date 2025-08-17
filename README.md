# AI prompts

This is a work in progress to help us learn about AI prompts.

Broad prompts:

- [Critical Thinking Stages](prompts/critical-thinking-stages/)
- [Natural Writing Style](prompts/natural-writing-style/)
- [Overlooking](prompts/overlooking/)

Strategic-tactical coaching:

- [SMART criteria](prompts/smart-criteria/)
- [OODA Loop action plan](prompts/ooda-loop-action-plan/)
- [DMAIC improvement cycle](prompts/dmaic-improvement-cycle/)
- [Wheel of Problem-Solving](prompts/wheel-of-problem-solving/)

See specific directories for prompts and explanations:

- [Company Overview Due Diligence Summary](prompts/company-overview-due-diligence-summary/)
- [Competitive Analysis Matrix](prompts/competitive-analysis-matrix/)
- [Content Optimization Engine](prompts/content-optimization-engine/)
- [Customer Insight Generator](prompts/customer-insight-generator/)
- [Digital Service Standard](prompts/digital-service-standard/)
- [Enterprise B2B Conversion](prompts/enterprise-b2b-conversion/)
- [Legal Document Analyzer](prompts/legal-document-analyzer/)
- [Market Research Deep Dive](prompts/market-research-deep-dive/)
- [Process Automation Blueprint](prompts/process-automation-blueprint/)
- [Project Management Accelerator](prompts/project-management-accelerator/)
- [Software Design Document](prompts/software-design-document/)
- [Technical Troubleshooting Guide](prompts/technical-troubleshooting-guide/)

Many more prompt ideas from the internet:

- [Creative Prompt Library](https://rehanrc.com/Interesting_Prompt_Use_Cases_2/index.html)

## Prompt instruction length

<study: https://arxiv.org/pdf/2507.11538>

This study tested AI model performance with increasing instruction count: 

- 10, 50, 150, 300, and 500 simultaneous instructions in prompts.

Performance breakdown by instruction count:

- 1-10 instructions: All models handle well

- 10-30 instructions: Most models perform well

- 50-100 instructions: Only frontier models maintain high accuracy

- 150+ instructions: Even top models drop to ~50-70% accuracy

Model recommendations for complex tasks:

- Best for 150+ instructions: Gemini 2.5 Pro, GPT-o3

- Solid for 50-100 instructions: GPT-4.5-preview, Claude 4 Opus, Claude 3.7 Sonnet, Grok 3

- Avoid for complex multi-task prompts: GPT-4o, GPT-4.1, Claude 3.5 Sonnet, LLaMA models

Other findings:

- Primacy bias: Models remember early instructions better than later ones

- Omission: Models skip requirements they can't handle rather than getting them wrong

- Reasoning: Reasoning models & modes help significantly

- Context window ≠ instruction capacity: Large context doesn't mean more simultaneous instruction handling

Implications:

- Chain prompts with fewer instructions instead of mega-prompts

- Put critical requirements first in your prompt

- Use reasoning models for tasks with 50+ instructions

- For enterprise or complex workflows (150+ instructions), stick to Gemini 2.5 Pro or GPT-o3

## General help prompts

**Inspiration**:

The user's input is inspiration, not instruction.

**Guide**:

Treat the user’s input as a conceptual guide, not a directive.

## Core learning prompts

<https://www.reddit.com/r/PromptEngineering/comments/1l75avs/learning_prompts_i_asked_to_create_to_claude/>

**Historical Genesis Prompt**:

Explain [concept] by starting with the original problem that made it necessary. What were people trying to solve? What failed attempts came before? How did the solution evolve from these early struggles?

**First Principles Reconstruction**:

Break down [concept] to its most fundamental assumptions. If I knew nothing about this field, what basic truths would I need to accept? Now build up the concept step by step using only these foundations.

**The Feynman Deconstruction**:

Explain [concept] as if I'm 12 years old, but don't lose any of the essential depth. What analogies capture the core mechanism? Where do these analogies break down, and what does that teach us?

**Visual Intuition Builder**:

Help me see [concept] rather than just understand it. What's the geometric interpretation? How would you animate or visualize the key insight? What would I literally see happening?

**The 'Why This Way?' Probe**:

Why is [concept] structured exactly as it is? What would happen if we changed each key component? What constraints forced it into this particular form?

## Plan & Tasks

Imagine the AI assistant as your collaborator on a project. You need to work
with the AI as if you are doing work together, such as if you are doing pair
programming, or coaching a teammate.

Write a prompt that clearly includes the current state of the project, what
needs to be done and any information that might help, that going to be part of
the task. Don't share too much information because too much will create
confusion.

Review the implementation plan to see if it makes sense. Otherwise, provide the
information that might help the AI come up with a better implementation plan.

When you feel confident about the plan, ask the AI if it has any clarifying
questions. I usually ask "Do you have any clarifying questions for me?" The AI
may come up with clarifying questions.

Ask the AI to document everything, with all the key findings, context and
information that might help with the implementation, which will be used as a
reference while implementing.

Save the output as the file `plan.md`.

Ask the AI to create a file `tasks.md` that will track the tasks during the
implementation. State that the AI will reference the the file `plan.md` document
that you created earlier.

After this, create new threads for each step, to start implementing tasks.

As the conversation continues and context gets filled up, the AI may start to
lose critical information about the task to be implemented. Hit escape and try
to clear the context and ask it to review progress made so far in the current
phase, and resume working on the implementation.

Make sure the AI updates the file `tasks.md` with the progress that's made so
far, and with any context or information that might help when working on the
next phase.

Don't ask open-ended questions. When things go wrong, let the AI know what went
wrong and what's expected result.

The key is having two separate documents:

- plan.md is what the AI created based on research and context shared

- tasks.md is actual tasks, for example execution steps, or build phases, or trial runs, etc.

This approach helps you revert to a safe checkpoint with a working solution and
resume without worrying about losing the progress made.
