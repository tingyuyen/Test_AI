---
title: AI 情緒分析助手
emoji: 🧪
colorFrom: indigo
colorTo: pink
sdk: static
pinned: false
license: mit
short_description: 在瀏覽器中使用 DistilBERT 分析英文句子的正面或負面情緒
---

# 🧪 Spaces Capabilities Demo

A dummy, hands-on sandbox for understanding what **Hugging Face Spaces** can do.

This is a **Static Space** — plain HTML/CSS/JS served straight from a git repo, free for
everyone, no GPU or paid plan required. Despite being "just static", it runs a **real
machine-learning model live in your browser** using
[🤗 Transformers.js](https://huggingface.co/docs/transformers.js) (WebGPU / WASM), with the
model weights streamed from the Hugging Face Hub CDN. No backend, no server code.

## What it demonstrates

- **In-browser ML** — sentiment analysis running client-side, zero server compute.
- **The three Space SDKs** — Static vs. Gradio vs. Docker, and when to reach for each.
- **Hardware tiers** — CPU, ZeroGPU, and dedicated GPUs, and what a free account can host.
- **The Space anatomy** — every Space is a git repo with a `README.md` frontmatter block
  that configures the runtime.

## How it was built

Created and deployed entirely from the command line with the `hf` CLI:

```bash
hf repos create <you>/spaces-capabilities-demo --type space --space-sdk static --public
hf upload   <you>/spaces-capabilities-demo . --repo-type space
```

The whole app is a single [`index.html`](index.html) — open it to see how the in-browser
model is loaded and run.
