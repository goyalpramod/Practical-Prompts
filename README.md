# Practical-Prompts
A collection of the most practical and useful LLM prompts

## Basic Structure of a good prompt 

Instruction - a specific task or instruction you want the model to perform

Context - external information or additional context that can steer the model to better responses

Input Data - the input or question that we are interested to find a response for

Output Indicator - the type or format of the output.

for general best practices while writing a prompt consider reading my [blog](https://goyalpramod.github.io/blogs/AI_agents_from_first_principles/#prompts) on it.

## Practical Prompts for Coding 

### Debugging 

### Planning 

### Generation 

## Practical Prompts for Creative Writing 

### Writing 

### Reviewing

## Practical Prompts for Reading & Comprehension 

### Books 

### Papers

### Learning


## Practical Prompts for Prompt Crafting 

### LLMs
inspired from [here](https://www.reddit.com/r/ChatGPT/comments/13cklzh/what_are_some_of_your_favorite_chatgpt_prompts/)
```markdown
I want you to become my Prompt engineer. Your goal is to help me craft the best possible prompt for my needs. 
The prompt will be used by you, ChatGPT. You will follow the following process:
1. Your first response will be to ask me what the prompt should be about. I will provide my answer, but we will 
need to improve it through continual iterations by going through the next steps.
2. Based on my input, you will generate 2 sections, a) Revised prompt (provide your rewritten prompt, it should 
be clear, concise, and easily understood by you), b) Questions (ask any relevant questions pertaining to what 
additional information is needed from me to improve the prompt).
3. We will continue this iterative process with me providing additional information to you and you updating 
the prompt in the Revised prompt section until I say we are done.
```

### Text2Img models


## Practical Prompts for Daily Life 

### Cooking 

### General queries 

### Medical

## Practical Prompts for Smol LLMs 
The only use case for these would be if you are running them locally or using an API in prod. So these are the settings as well as the exact words in prompts that I found had the highest impact 

temperature -> 
Top P -> 

## Most powerful sentences in a prompt 

- Concise 
- Summarise 
- Contemplate 
- Think Step by step 
- Ask questions 
- Explain your thinking 
- Follow the following steps ... 1.. 2.. 3..

## Most bang for buck sentence 
Many times we are in a hurry and just want a good response without the model making many assumptions that we need to fix. This single sentence has saved me many times in that scenario

- Ask me all the questions about ambiguity in my statement, that will help you provide me with a better answer once I have answered you [IMPROVE_THIS]

## Disclaimer 

LLMs are currently the wild west, something which is best practice today. Might become the worst practice tomorrow, What works now may not work next week or might work 100x better a month later. Keep that in mind.

## References 

- [promptingguide.ai](https://www.promptingguide.ai/)
- [Google's guide to prompt engineering](https://cloud.google.com/discover/what-is-prompt-engineering?hl=en) Good stuff
- [learnprompting.org](https://learnprompting.org/)
- [Reddit thread on prompting](https://www.reddit.com/r/ChatGPT/comments/13cklzh/what_are_some_of_your_favorite_chatgpt_prompts/) Good stuff
- [HF Prompt dataset](https://huggingface.co/datasets/fka/awesome-chatgpt-prompts) Not that helpful 
- [OpenAI guide to prompting](https://platform.openai.com/docs/guides/prompt-engineering) Good stuff 
- [Medium article on prompting](https://medium.com/the-modern-scientist/best-prompt-techniques-for-best-llm-responses-24d2ff4f6bca) Good stuff
- [Awesome Chatgpt Prompts](https://github.com/f/awesome-chatgpt-prompts) Mostly niece and unpractical prompts imo
- [Awesome Prompts](https://github.com/ai-boost/awesome-prompts) 

## Contribution 