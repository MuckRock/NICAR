# Enhancing public records work with LLMs

Sanjin Ibrahimovic <sanjin@muckrock.com>
Allan Lasser <allan@muckrock.com>

## Introduction

So, you've just received a bunch of public records—how can you make sense of them?

## Create a project folder

```sh
mkdir ~/my-investigation
cd ~/my-investigation
```

## Using the LLM CLI tool

1. [Install the `llm` library](https://llm.datasette.io/en/stable/setup.html).

```sh
pip install llm
```
```sh
uv tool install llm
```
```sh
brew install llm
```

2. Then we need to install some plugins for LLM to use it with DocumentCloud and Claude. We also need to make sure our secret keys are available in the environment.

```sh
# install llm plugins
llm install llm-anthropic
llm install llm-documentcloud
```

```sh
# make secrets available
export ANTHROPIC_API_KEY=<YOUR KEY HERE>
```

## Using the DocumentCloud SDK

TK