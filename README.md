# Minimal AI

A tiny, zero-dependency browser chat client for any OpenAI-compatible API endpoint (OpenRouter, OpenAI, self-hosted models, proxies, etc.).

## Use it directly

Open `index.html` in a browser. It works immediately with OpenRouter free models.

To use paid models, create an [OpenRouter](https://openrouter.ai) account, generate an API key, and paste it in **Settings**.

## Use it on your own page

Drop `index.html` anywhere you can serve static HTML: a personal site, an intranet portal, Netlify, etc. It is a single file, no build step required.

## Setup

1. Open **Settings** (the cog).
2. Set **Provider API Base URL** if you use a proxy (default is OpenRouter).
3. Paste your **API Key** to unlock paid models.
4. Add or remove **Models** one per line.
5. Adjust the **System Prompt** or keep the default.

## Features

- Markdown rendering
- Streaming responses
- Retry from any user message
- Code block copying
- Templates/modes
- Optional web search where the provider supports it (uses OpenRouter's `openrouter:web_search` server tool)
- Persistent settings and chat history in `localStorage`

## Notes

- The default key targets OpenRouter's free tier. If you switch to a different provider, replace it with that provider's key.
- The included key is visible in the source. If you embed this page publicly and use your own key, keep in mind that visitors can read it from `index.html`.
- Web search is off by default. Toggle **Web** to enable it.
