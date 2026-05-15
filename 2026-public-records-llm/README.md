# Enhancing public records work with LLMs

**2:30 – 3:30pm, Thursday, March 5, 2026**

- Sanjin Ibrahimovic <sanjin@muckrock.com>
- Allan Lasser <allan@muckrock.com>

## Introduction

So, you've just received a bunch of public records—how can you make sense of them?

In this session, we'll show off three different ways to analyze public records using a combination of the MuckRock Requests API, the DocumentCloud API, and the Anthropic API. We'll show how to:

1. How to extract text from documents, analayze their contents, and visualize them
2. How to access MuckRock's agency API and submit a FOIA request with a Python script
3. How to use Claude for advanced text and PDF analysis
4. How to _think_ about applying LLMs like Claude within your reporting practice

We cover three scenarios:

1. Analyzing and visualizing Trump's pardons
2. Requesting police disciplinary records
3. Obtaining FOIA logs from IG reports

## Requirements

In order to run the Jupityr notebook, [`notebook.ipynb`](./notebook.ipynb) for yourself, you'll need to create a `.env` file in this directory with:

```
ANTHROPIC_API_KEY=YOUR_ANTHROPIC_API_KEY
DOCUMENTCLOUD_USERNAME=YOUR_MUCKROCK_USERNAME
DOCUMENTCLOUD_PASSWORD=YOUR_MUCKROCK_PASSWORD
MUCKROCK_USERNAME=YOUR_MUCKROCK_USERNAME
MUCKROCK_PASSWORD=YOUR_MUCKROCK_PASSWORD
```

- `ANTHROPIC_API_KEY` can be obtained from `platform.claude.com`. There is a free tier that allows you to make limited use of Claude.
- `DOCUMENTCLOUD_USERNAME` and `MUCKROCK_USERNAME` are the same value—your MuckRock account username—but each Python library expects a slightly differently named secret.
- `DOCUMENTCLOUD_PASSWORD` and `MUCKROCK_PASSWORD` are the same value—your MuckRock account password—but each Python library expects a slightly differently named secret.
