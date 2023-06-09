# Ecommerce Chatbot with LangChain, and OpenAI


This is a proof of concept for building a conversational retail shopping assistant that helps customers find products in a huge catalog. Our chatbot will take user input, find relevant products, and present the information in a friendly and detailed manner.

[Redis](https://redis.io), [LangChain](https://python.langchain.com/en/latest/), and [OpenAI](https://platform.openai.com)

As of now, the chatbot answers questions specific to products,

# Todo:

Allow chatbot to create shopping lists by experimenting with Tree of thought(https://arxiv.org/abs/2305.10601) prompt engineering technique and a/b test to find the right prompt for given task to improve on poc.

Create plugins to interface with walmart APIs to retrieve product information, add products to cart directly from the shooping lists, enabling payments directly in the chat interface.

## Getting Started
1. Install Docker Desktop for mac or windows(https://www.docker.com/products/docker-desktop/).
2. [Generate your own OpenAI API Key](https://platform.openai.com).
3. Add the API key to the [`docker-compose.yml`](./docker-compose.yml) file here in the repo. You should see a field called OPENAI_API_KEY in the yaml file. Paste your key value for the same.
4. Start up the docker compose environment:
    ```bash
    docker compose up
    ```

DO NOT FORGET TO ADD API KEY TO YAML FILE. WITHOUT THE API KEY, THE APPLICATION CANNOT BE TESTED.

## Notes
Langchain and OpenAI are used to demonstrate the capabilities of Large Language Models in solving complex problems. We could envision a similar system of LLM's using other foundational models (eg:PaLM - Pathways Learning Model.) and create our own framework to enable application development using LLM's.

## Demonstration
​
To demonstrate the working of out POC our team was able to come up with many questions but for conversational purposes with the chatbot we asked the questions given below for reference.
​
1. What kind of eggs are available?
2. What all cereal choices do I have?
3. Are there any meat products?
4. I am looking for new TV? Can you give me some recommendation.
​
