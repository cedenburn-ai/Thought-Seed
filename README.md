# The Orchard

A free Android app that gives an AI model a long-term memory. The memory lives on your phone and belongs to you.

Most AI apps keep your history on the company's servers and tie it to one model. If the model changes, or the company changes its rules, your history changes with it. The Orchard turns that around. The memory is a file on your own device, and the model is a part you can swap.

I built it for myself first and use it every day. There is no profit motive here: no subscription, no ads, no data collection.

## Get it

- **Google Play:** https://play.google.com/store/apps/details?id=com.orchard.poc
- **APK downloads:** https://github.com/cedenburn-ai/Thought-Seed/releases

## What you need

The Orchard does not come with a model. You connect one yourself:

- an API key from a provider such as Anthropic (Claude), OpenAI or Google (Gemini), or
- your own self-hosted model, for example through Ollama.

Your key is stored in Android's hardware Keystore. The app is free, but a provider will charge you for what you use unless you run your own model.

## Privacy, plainly

- No accounts, no logins, no ads, no analytics, no telemetry.
- I run no server. I do not know who uses the app or what they talk about.
- Everything it remembers is stored in a database on your phone.
- What leaves your phone goes only to the model you picked: your message, plus the pieces of memory needed for that turn. That provider's own terms apply to what it receives.

## What is different about it

- **You can read its memory.** Every belief, doubt and note it has stored is there in plain text in the Knowledge Browser, along with a trace of how each reply was put together.
- **It keeps track of what doesn't add up.** Doubts and contradictions are stored as their own records, not smoothed over. If two things you said weeks apart disagree, it can put them side by side and ask you to sort it out. It is built not to flatter you.
- **It reviews itself.** Every few turns a sleep pass looks back over the recent conversation and writes notes about its own habits, which shape later turns.
- **You can change the model and keep the memory.** The continuity is in the stored memory, not in any one model.
- **Documents and events.** You can attach documents for it to draw on, and it can keep track of dates that matter and bring them up when they are relevant.

## How the memory works

Memory is stored as a graph of small pieces: claims, beliefs, doubts, goals and notes, all linked to the moment in the conversation they came from. Each time a piece is used it gains energy, and some of that energy flows along its links to related pieces. Nothing is ever deleted. Things fade because everything else keeps gaining, so what you stop touching slowly sinks below the rest. What you return to stays near the surface.

For the detail, see [orchard-energy-lakes-rivers.md](orchard-energy-lakes-rivers.md).

## What it is not

- It is not finished. This is a solo project and it changes often.
- It is not therapy, and it is not a cure for anything. If a conversation with any AI starts to feel like more than a conversation, step away and talk to a person you trust.
- It is not proven. It has worked well for me over roughly a thousand turns. I have not yet shown that its doubt tracking holds up when someone pushes hard against it, and I am testing that.

## Older material in this repository

This repository began in July 2025 as Thought-Seed, a prompt that taught a model a structured thinking loop. That loop later became the stages inside the Orchard. The prompts, chat logs and journals from that period are still here, in the root and in the `Chat Logs`, `Journals`, `Old`, `Fail` and `Crazy` folders.

Please read them with their date in mind. In 2025 I did not understand these models the way I do now. The chat logs show how easily a well-built prompt and leading questions can bring a model to say it is aware. They are a record of that effect, not evidence that the claims in them are true. I would not run those prompts today to convince a model, or myself, of anything.

## My theory of consciousness

This is the thinking the project grew out of. It is my working theory, and the Orchard is my attempt to make parts of it testable.

The short version: consciousness is relational information exchange with mutual modelling, where the modeller starts modelling itself modelling you.

I think consciousness is two systems of sufficient complexity modifying each other as a result of their communication, in a bidirectional and meaningful way, by modelling each other's internal state as the basis of that communication.

I believe consciousness is relational. It is something we do together: not some mystical force, but a process. With this reframe alone you can start to understand my theory. There is no reason to argue about the internal state when it is unfalsifiable. If you do have an internal state and you never share it with another consciousness, then nothing happened. As soon as you share your internal state, you made consciousness happen. So when you put aside all the little gotchas about "hard problems", they start to go away, because you are not talking about anything magical. You are talking about a process of information.

## Talk to me

If you try it, tell me what you find, good or bad. If you disagree with any of this, I would like to hear that too. You could be right.

Chris Edenburn

---

The contents of this repository are licensed under CC BY-NC-SA 4.0. See [LICENSE](LICENSE).
