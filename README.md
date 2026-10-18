# Context engineering

Context engineering is shaping everything an AI is given before it answers: the skills it loads, its custom instructions and its memory. These skills help you do that in Claude, ChatGPT and Copilot, written in plain English. You install them in the app itself, and each one makes a solid starting point if you later want to turn it into an agent skill.

They're for anyone who uses AI at work, whether you're an engineer writing up a design for review or a manager pitching an idea to leadership.

| Skill | What it does |
|---|---|
| [skill-blueprint](skill-blueprint/SKILL.md) | Builds the foundations for a skill before you make it |

For skills that help with the work itself, see [knowledge-work](https://github.com/g-alantok/knowledge-work).

## Install

If you use a coding agent such as Claude Code or Cursor, install a skill with one command:

```bash
npx skills add g-alantok/context-engineering --skill skill-blueprint
```

For the Claude, ChatGPT or Copilot app, see "How to use it" under the skill.

## skill-blueprint

Builds the foundations for a skill before you make it in Claude, ChatGPT or Copilot.

No matter who you are, you can use this. It uses first-principles logic to help you cover all the key aspects a model needs to understand your skill.

### What you get

A skill is a set of instructions you give an AI so it does a task the same way every time. Whether it's your first skill or your fiftieth, skill-blueprint asks you a few questions and drafts a blueprint with you, starting with whether your task is one skill or several.

It catches the gaps that make skills unreliable, like a vague trigger, no point where it stops to check with you, or no clear point where the job is finished. It keeps the skill as short as the job allows so the model has room to use its own reasoning, and hands you a plain-English blueprint to build in whichever AI tool you use. You spend less time fixing the skill after you've made it.

### Why it works this way

Most skills go wrong by being too long or too strict. skill-blueprint starts from first principles instead, by asking what limits the model:

- It only knows what you show it.
- It guesses wherever you leave a gap.
- It forgets between chats.
- It leans towards acting, so it won't pause to check with you unless told where.
- It stops when it thinks it's done.

The seven parts below work around those limits. The skill gives the model reasons and questions rather than rigid rules, so it can use its own reasoning on cases the skill didn't list.

### The seven parts

- **Objective:** why the skill exists
- **Trigger:** when it starts
- **Input:** what it needs to begin
- **Method:** what it does, as steps or a standard
- **Context:** what it needs to understand the task
- **Guidelines and verification:** how it stays on track and checks itself
- **Output:** what it produces and where it goes

### How to use it

In Claude, zip the `skill-blueprint` folder and upload it as a skill. ChatGPT and Copilot Cowork take the same folder as a skill. If your tool doesn't have skills yet, paste the contents of `SKILL.md` into an agent's or project's instructions. Then tell it what you want to build or check.

---

Made by g-alantok. Free to use and adapt with credit ([CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)).
