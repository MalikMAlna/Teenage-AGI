# Teenage-AGI

## Objective
Inspired by the several Auto-GPT related Projects (predominently BabyAGI) and the Paper ["Generative Agents: Interactive Simulacra of Human Behavior"](https://arxiv.org/abs/2304.03442), this python project uses OpenAI and Pinecone to Give memory to an AI agent and also allows it to "think" before making an action (outputting text).

## How it Works
Here is what happens everytime the AI is queried by the user:
1. AI vectorizes the query and stores it in a Pinecone Vector Database
2. AI looks inside its memory and finds memories and past queries that are relevant to the current query
3. AI thinks about what action to take
4. AI stores the thought from Step 3
5. Based on the thought from Step 3 and relevant memories, AI generates an output
6. AI stores the current query and its answer in its Pinecone vector database memory

## How to Use
1. Clone the repository via `git clone https://github.com/seanpixel/Teenage-AGI.git` and cd into the cloned repository.
2. Install required packages by doing: pip install -r requirements.txt
3. Set your OpenAI and Pinecone API info in the OPENAI_API_KEY, PINECONE_API_KEY, and PINECONE_API_ENV variables.
4. Run `python main.py` and talk to the AI in the terminal

## More about the Project & Me
After reading the Simulcra paper, I made this project in my college dorm. I realized that most of the "language" that I generate are inside my head, so I thought maybe it would make sense if AGI does as well. I'm a founder currently working on a project called [DSNR]([url](https://www.dsnr.ai/)) and also a first-year at USC. Contact me on [twitter](https://twitter.com/sean_pixel) about anything would love to chat.

## Credits
Thank you to [@yoheinakajima](https://twitter.com/yoheinakajima) and the team behind ["Generative Agents: Interactive Simulacra of Human Behavior"](https://arxiv.org/abs/2304.03442) for the idea!