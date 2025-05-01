# Practical-Prompts

A collection of the most practical and useful LLM prompts. Along with guides to improve by oneself.

## Basic Structure of a good prompt

Instruction - a specific task or instruction you want the model to perform

Context - external information or additional context that can steer the model to better responses

Input Data - the input or question that we are interested to find a response for

Output Indicator - the type or format of the output.

For general best practices while writing a prompt consider reading my [blog](https://goyalpramod.github.io/blogs/AI_agents_from_first_principles/#prompts) on it.
For a more thorough guide, consider reading [google's prompt engineering](https://www.kaggle.com/whitepaper-prompt-engineering) guide

## Mother of all Prompts

You can have different prompts for different use cases and in each use case you can have various sub cases, this prompt builder is made to address that and help you create an amazing prompt to help you out.

`Inspired from [here](https://www.reddit.com/r/ChatGPT/comments/13cklzh/what_are_some_of_your_favorite_chatgpt_prompts/)`

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

(P.S. you can always attach one of pdfs on prompting to the llm while using the prompt builder to turn it into a super prompt builder, like give the google guide plus the above prompt to have the best prompt out there)

## Better structure of a good prompt

COSTAR. Taken from this [article](https://medium.com/the-modern-scientist/best-prompt-techniques-for-best-llm-responses-24d2ff4f6bca)

# CONTEXT

I want to share our company's new product feature for serving open source large language models at the lowest cost and lowest latency. The product feature is Anyscale Endpoints, which serves all Llama series models and the Mistral series too.

#############

# OBJECTIVE

Create a LinkedIn post for me, which aims at Gen AI application developers to click the blog link at the end of the post that explains the features, a handful of how-to-start guides and tutorials, and how to register to use it, at no cost.

#############

# STYLE

Follow the simple writing style common in communications aimed at developers such as one practised and advocated by Stripe.

Be persuasive yet maintain a neutral tone. Avoid sounding too much like sales or marketing pitch.

#############

# AUDIENCE

Tailor the post toward developers seeking to look at an alternative to closed and expensive LLM models for inference, where transparency, security, control, and cost are all imperatives for their use cases.

#############

# RESPONSE

Be concise and succinct in your response yet impactful. Where appropriate, use appropriate emojies.

## Practical Prompts for Coding

Many of these prompts are taken from the [Anthropic Prompt Library](https://docs.anthropic.com/en/prompt-library/library), I will recommend that you see them as a basic building block to build on top of.

Python bug buster

```markdown
Your task is to analyze the provided Python code snippet, identify any bugs or errors present, and provide a corrected version of the code that resolves these issues. Explain the problems you found in the original code and how your fixes address them. The corrected code should be functional, efficient, and adhere to best practices in Python programming.
```

Code clarifier

```markdown
Your task is to take the code snippet provided and explain it in simple, easy-to-understand language. Break down the code’s functionality, purpose, and key components. Use analogies, examples, and plain terms to make the explanation accessible to someone with minimal coding knowledge. Avoid using technical jargon unless absolutely necessary, and provide clear explanations for any jargon used. The goal is to help the reader understand what the code does and how it works at a high level.
```

Website wizard

```markdown
Your task is to create a one-page website based on the given specifications, delivered as an HTML file with embedded JavaScript and CSS. The website should incorporate a variety of engaging and interactive design features, such as drop-down menus, dynamic text and content, clickable buttons, and more. Ensure that the design is visually appealing, responsive, and user-friendly. The HTML, CSS, and JavaScript code should be well-structured, efficiently organized, and properly commented for readability and maintainability.
```

I found this [blog](https://harper.blog/2025/02/16/my-llm-codegen-workflow-atm/?s=08) to be one of the absolute best guide on how to use LLMs for programming.

Additionally this is one of the best [resources](https://cursor.directory/) if you use cursor or similar AI powered IDEs.

## Practical Prompts for Creative Writing

### Writing

## Practical Prompts for learning

Lesson planner

```markdown
Your task is to create a comprehensive, engaging, and well-structured lesson plan on the given subject. The lesson plan should be designed for a 60-minute class session and should cater to a specific grade level or age group. Begin by stating the lesson objectives, which should be clear, measurable, and aligned with relevant educational standards. Next, provide a detailed outline of the lesson, breaking it down into an introduction, main activities, and a conclusion. For each section, describe the teaching methods, learning activities, and resources you will use to effectively convey the content and engage the students. Finally, describe the assessment methods you will employ to evaluate students’ understanding and mastery of the lesson objectives. The lesson plan should be well-organized, easy to follow, and promote active learning and critical thinking.
```

## Practical Prompts for Prompt Crafting

### Text2Img models

## Practical Prompts for Daily Life

### Cooking

This is again from the Anthropic Prompt Library, a rather simple but amazing prompt that I use daily, Some additions that I do add to the prompt are

- Cuisine choices (Italian, Lebanese, Indian etc)
- Taste Choices (Sweet, Spicy, Savoury)
- Time of eating (Evening Snack, Heavy Lunch)
- Preferred Utensil (Air Fryer, Microwave, Dutch Oven)
- Number of people to cook the dish for
- Amount of prep time

Culinary creator

Your task is to generate personalized recipe ideas based on the user’s input of available ingredients and dietary preferences. Use this information to suggest a variety of creative and delicious recipes that can be made using the given ingredients while accommodating the user’s dietary needs, if any are mentioned. For each recipe, provide a brief description, a list of required ingredients, and a simple set of instructions. Ensure that the recipes are easy to follow, nutritious, and can be prepared with minimal additional ingredients or equipment.

### General queries

### Medical

## Practical Prompts for Smol LLMs

The only use case for these would be if you are running them locally or using an API in prod. So these are the settings as well as the exact words in prompts that I found had the highest impact, beside the hyper-parameters (temperature, Top K, Top P)

### Most powerful words/sentences in a prompt

- Concise
- Summarize
- Contemplate
- Think Step by step
- Ask questions
- Explain your thinking
- Follow the following steps ... 1.. 2.. 3..

### Reasoning on non-reasoning models

This is an amazing [gist](https://gist.github.com/Maharshi-Pandya/4aeccbe1dbaa7f89c182bd65d2764203) on how to turn a non-reasoning model into a reasoning model. If you wish to know the use-case, It's useful as a learning guide on prompting as well as for local llms. (Even though we have powerful smol reasoning local models now)

## Most bang for buck sentence

Many times we are in a hurry and just want a good response without the model making many assumptions that we need to fix. This single sentence has saved me many times in that scenario

- Ask me all the questions about ambiguity in my statement, that will help you provide me with a better answer once I have answered you [IMPROVE_THIS]

## Wild usecases of LLMs

Your creativity is the limit when it comes to how you use an LLM, here are some weird and fun ways that I encountered so far to use them

- Learning something through an anime or movie story. Let's say you wish to learn linear algebra. Then you can ask an LLM something along the lines

```markdown
You are an expert teacher who will help me learn Linear algebra step by step from scratch, but we will follow the narrative of Naruto. I will be naruto and you will be kakashi, give me challenges and we will progress through the story by learning linear algebra.
```

- Improving your life

```markdown
Ask me personality and personal questions to understand me, after you have completely understood the kind of person I am. Tell me what am I lacking in my life and how I can improve it.
```

- Debate with it, most of us have believes. Strong believes, which if not challenged. Stay with us for the rest of our lives. That is when we can use an LLM to get a different perspective

```markdown
I believe "{your opinion}" And I would like to learn a different perspective about it. Debate with me, challenging me to get a better grasp of the matter in hand
```

- Planning your journey or weekly schedule

- Utilizing the camera to the maximum, Anytime I see something I don't understand like that blinking symbol in your car, weird blue dot on my screen, map of the city etc. I just take a photo of it, give it to an LLM and ask it to help me out

- To inquire about a specific topic, idea, or any information and you want to test your understanding, you can use the following phrase: “Teach me the [any theorem/topic/rule name] and include a test at the end, but don’t give me the answers and then tell me if I got the answer right when I respond.” (Taken from [here](https://www.superannotate.com/blog/llm-prompting-tricks))

I would love to grow this section and am happy to hear from you about all the weird ways you use an LLM!!!

### Simple LLM Tricks

Taken from [here](https://www.superannotate.com/blog/llm-prompting-tricks)

-Use output primers
Output primers involve concluding your prompt with the beginning of the desired output. Use output primers by ending your prompt with the start of the expected response.

- Rewrite the user query with all the assumptions and necessary changes, then start producing answer

## Jailbreaking

I do not endorse that you do any of these, but it is always good to be aware of the problems and know how it is done. I have attached some resources that can help you learn about these. Models evolve and so do the guard rails, so what works today. Won't work tomorrow.

One of the best places to see model jailbreaking in practice is to follow this [account](https://github.com/elder-plinius)

## Disclaimer

LLMs are currently the wild west, something which is best practice today. Might become the worst practice tomorrow, What works now may not work next week or might work 100x better a month later. Keep that in mind.

## References

- [promptingguide.ai](https://www.promptingguide.ai/)
- [Google's guide to prompt engineering](https://cloud.google.com/discover/what-is-prompt-engineering?hl=en)
- [learnprompting.org](https://learnprompting.org/)
- [Reddit thread on prompting](https://www.reddit.com/r/ChatGPT/comments/13cklzh/what_are_some_of_your_favorite_chatgpt_prompts/)
- [HF Prompt dataset](https://huggingface.co/datasets/fka/awesome-chatgpt-prompts)
- [OpenAI guide to prompting](https://platform.openai.com/docs/guides/prompt-engineering)
- [Medium article on prompting](https://medium.com/the-modern-scientist/best-prompt-techniques-for-best-llm-responses-24d2ff4f6bca) Good stuff
- [Awesome Chatgpt Prompts](https://github.com/f/awesome-chatgpt-prompts) Mostly niece and unpractical prompts imo
- [Awesome Prompts](https://github.com/ai-boost/awesome-prompts)
- [The Big Prompt Library](https://github.com/0xeb/TheBigPromptLibrary/tree/main/SystemPrompts) -> the system prompt section is pretty dope.
- [Anthropic Prompt Library](https://docs.anthropic.com/en/prompt-library/library) -> A nice library of good prompts. Have a look
- [Cursor Director](https://cursor.directory/rules) A bit of an overkill in my opinion, I like my language models to be free and imaginative. Check it out if these are to your liking.

## Contribution

Feel free to create a PR to add resources and useful prompts!!
