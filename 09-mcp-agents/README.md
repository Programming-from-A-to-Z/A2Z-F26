# MCP & Agents

## Before class

1. Install [LM Studio](https://lmstudio.ai) and download a model that can call tools: `gemma-4-12b-qat` or `qwen3.8-27b` (much bigger). On a laptop with less memory, search for `gemma-4` and pick a smaller size. LM Studio should let you know if a model will fit on your machine!
2. For [Ollama](https://ollama.com/): `ollama pull qwen3` (~5 GB). You can also try `ollama pull gemma4:e2b-it-qat` (~4.3 GB). (We'll also use the ITP GPU machine's Ollama in case your laptop can't handle these.)
3. Make sure the context length in Ollama app's settings is at least 16k (I ran these examples with 256k context, but going that high will use a lot of memory).
4. Make sure you have node installed `node --version` (everything should work with v20.12+).
5. Grab the [Agent Examples](https://github.com/Programming-from-A-to-Z/Agent-Examples) repo and run `npm install`.

## What is MCP?

**MCP (Model Context Protocol)** is a standard for connecting LLMs to external tools and data.

- MCP servers expose tools and execute code.
- MCP clients (like LM Studio, Claude Desktop, VS Code, etc.) connect to those servers and the LLM running in the client calls the tools as it determines necessary.

### Resources

- [Model Context Protocol](https://modelcontextprotocol.io)
- [Introducing the Model Context Protocol](https://www.anthropic.com/news/model-context-protocol)
- [Claude Docs Overview](https://docs.claude.com/en/docs/mcp)
- [MCP TypeScript SDK docs](https://ts.sdk.modelcontextprotocol.io/v2/)

> Think of MCP like a USB-C port for AI applications. Just as USB-C provides a standardized way to connect your devices to various peripherals and accessories, MCP provides a standardized way to connect AI models to different data sources and tools.

## LM Studio

- [LM Studio](https://lmstudio.ai)
- [LM Studio MCP docs](https://lmstudio.ai/docs/app/mcp)

**LM Studio** is a desktop app that downloads and runs local LLMs, just like Ollama. It has some nice features for working with MCP servers.

## How To

- 💻 [MCP Server Example and README guide](https://github.com/Programming-from-A-to-Z/MCP-Server-Example)

## Agents

An agent is a language model with access to tools, that runs in a loop. The model makes its own decision as to whether to call a tool and which one to use. The tool's output is fed back into the conversation, and the model repeats the process, until it decides to stop (usually because it needs no more tools) or asks a human.

> An LLM agent runs tools in a loop to achieve a goal. - [Simon Willison](https://simonwillison.net/2025/Sep/18/agents/)

LM Studio was running that "agentic" loop when it called `say_hello` from the [MCP Server Example](https://github.com/Programming-from-A-to-Z/MCP-Server-Example).

### Code Examples

- 💻 [Agent Examples](https://github.com/Programming-from-A-to-Z/Agent-Examples) - implement your own agentic loops in JS with Ollama and transformers.js.
- 📋 [Ollama tool calling docs](https://docs.ollama.com/capabilities/tool-calling)
- 🔗 [Ollama models that can use tools](https://ollama.com/search?c=tools)
- 🔗 [Ollama context length](https://docs.ollama.com/context-length)

### Reading

- 📕 [Building Effective Agents](https://www.anthropic.com/engineering/building-effective-agents) by Anthropic
- 📕 [The lethal trifecta for AI agents](https://simonwillison.net/2025/Jun/16/the-lethal-trifecta/) by Simon Willison
- 📚 [How to Build an Agent](https://ampcode.com/how-to-build-an-agent) by Thorsten Ball
- 📚 [Tiny Agents: an MCP-powered agent in 50 lines of code](https://huggingface.co/blog/tiny-agents) by Julien Chaumond

### Guiding Principles

1. Be specific and write targeted, small tools! "Save a text file in this one folder" is good. "Run any terminal command" is not.
2. Create "dummy" accounts for your agents for prototyping and practice.
3. Build in approval for things that can't be undone: send, delete, buy, post, etc. (I made an exception in the email example but it's still highly restricted as it can only send replies and has a limit to how many.)
4. Add a limit to the number of steps in any loop, and a way to stop the loop.
5. Agents should disclose they are bots. See the [Bot Code of Conduct](https://github.com/Programming-from-A-to-Z/Bot-Code-of-Conduct).

### Agents and art

- 🎨 [Random Darknet Shopper](https://wwwwwwwwwwwwwwwwwwwwww.bitnik.org/r/) by !Mediengruppe Bitnik (2014)
- 🎨 [LAUREN](https://lauren-mccarthy.com/LAUREN) by Lauren Lee McCarthy (2017)
- 🎨 [Deep Swamp](https://tegabrain.com/Deep-Swamp) by Tega Brain (2018)
- 🎨 [Agent Ruby](https://www.lynnhershman.com/project/agent-ruby/) by Lynn Hershman Leeson (1998)
- 🎮 [Universal Paperclips](https://www.decisionproblem.com/paperclips/) by Frank Lantz (2017), after Nick Bostrom's [paperclip maximizer](https://nickbostrom.com/ethics/ai)
- 🔗 [AI Village](https://theaidigest.org/village) and [Project Vend](https://www.anthropic.com/research/project-vend-1)

### Harnesses

An agent harness (or scaffolding) is a software program that brings together an LLM and many tools. It includes a software layer on top of the LLM that includes state management, compacting and summarizing, and tools for operating your computer. If you want to try one of these I recommend running them on a spare machine with a dummy user account, not your personal machine.

- 🔗 [Pi](https://pi.dev) - four tools: read, write, edit, bash. [Pi with Ollama](https://docs.ollama.com/integrations/pi)
- 🔗 [OpenClaw](https://github.com/openclaw/openclaw) - always-on assistant with access to your machine that you can message from Discord, WhatsApp, etc. [OpenClaw with Ollama](https://docs.ollama.com/integrations/openclaw)

## Assignment

- 🎨 [Prepare to present a final project proposal](/final/proposals.md).
