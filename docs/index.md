# LLMFlows - Simple, Explicit and Transparent LLM Apps

<p align="center">
  <img src="llmflows_last_logo.png" />
</p>

[![Twitter](https://img.shields.io/twitter/follow/LLMFlows?style=social)](https://twitter.com/LLMFlows)
![Pylint workflow](https://github.com/stoyan-stoyanov/llmflow/actions/workflows/pylint.yml/badge.svg)
![License](https://img.shields.io/github/license/stoyan-stoyanov/llmflow)
![PyPi](https://img.shields.io/pypi/v/llmflows)
![Stars](https://img.shields.io/github/stars/stoyan-stoyanov/llmflow?style=social)
![Release date](https://img.shields.io/github/release-date/stoyan-stoyanov/llmflow?style=social)

## About
LLMFlows is a simple and lightweight framework for building LLM-powered applications.

## Installation
```
pip install llmflows
```

## Philosophy

### Simple
We want to create a framework with a minimal set of classes that allows users to build powerful LLM-powered apps without compromising on capabilities.

### Explicit
We want to enable users to easily create complex flows of LLMs interacting with each other that have explicit and obvious structure.

### Transparent
Flows are traceable, executions are easily logged and none of the classes provided in LLMFlows have hidden prompts - prompts are for you to decide.

## Usage
Here is a minimal example of an LLM with a PromptTemplate:

```python

from llmflows.llms.openai import OpenAI
from llmflows.prompts.prompt_template import PromptTemplate

prompt_template = PromptTemplate(
   prompt="Generate a title for a 90s hip-hop song about {topic}."
)
llm_prompt = prompt_template.get_prompt(topic="friendship")

llm = OpenAI()
song_title = llm.generate(llm_prompt)

```

For more examples such as how to create question answering apps and web applications with Flask and FastAPI check our user guide.

## License
LLMFlows is covered by the MIT license. For more information check `LICENCE.md`.

## Contributing
Thank you for spending the time to read our README! If you like what you saw and are considering contributing please check CONTRIBUTING.md

## Links
Twitter

Github