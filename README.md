# AI OpenHands

A playground to evaluate the [OpenHands](https://github.com/All-Hands-AI/OpenHands) platform for software development agents powered by AI.

## Prerequisites

The following programs are required to use this repository:

1. Docker
2. Git
3. Local OpenAI compatible AI like `llama.cpp` or `ollama`

## Installation

### Clone repository

```Shell
git clone git@github.com:countzero/ai_open_hands.git
```

### Prepare LLM

Download a quantized version of the [Devstral-Small-2507](https://huggingface.co/mistralai/Devstral-Small-2507) model that fits in your GPU from:

* https://huggingface.co/unsloth/Devstral-Small-2507-GGUF

## Usage

### Start LLM

Start the `Devstral-Small-2507` model and note the `Base URL` of the OpenAI API. e.g. `http://10.0.2.2:8080/v1`

### Start OpenHands

Execute the following in the `ai_open_hands` directory

```Shell
docker compose up
```

### Access OpenHands

The OpenHands GUI should become available at:

* http://10.10.4.2:3000

### Configure OpenHands

Make sure the `Base URL` is set to your local LLM:

* http://10.10.4.2:3000/settings

### Collaborate with the AI

The shared workspace is available in the `shared_workspace/workspace` directory.
