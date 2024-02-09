
Lesson 3:
General Intro: 
We will use various tools to prompt engineer LLMs and get it complete various tasks. 
Limits of AI models:
No ability to take in current langauge, which means that events that happened after the data cutoff date will not be known or could be worst guessed.
RAG vs Finetune
RAG is a form of search and brings up data, it hinges on the assumption the AI already knows how to do the task and just needs the data. Finetuning is more comprehensive but also takes more effort to do well. The main focus of this specific lesson is RAG.
RAG:
Pass the knowledge to InternLM using Langchain. Langchain is a program that facilitates the creation of RAG pipelines, or chains as they call them. It uses a logical framework to plan and shift data in order to get the knowledge needed to InternLM.
The Problem  of Large samples:
Create a large amount of samples that are ye same character length.
The start of the pipeline is at the query, it is then inferened from the query the data the AI model needs. It is ideal to sort lots of text by the topic. 
Demo;
Gradio is used.
InternLM Usage:
Set up the environment as usual and create a new directory for the model files. Make another folder for data. We then use python to run a command in huggingface to download another model. We then run the new code. This model is used to sort the database. Create a new demo repo and use a python program to create a vector database. Only txt and md files are used. We define the folders we want to read in and list them. We then also need to embed all the data that we’ve used so far. Chroma is the database used. You only need to run this program once.
Usage of InternLM Part 2:
Create the InternLM instance and use the chat interface. This will be ran after the first part. We then create a script that uses Langchain to put all the other programs together. It also includes a template with desired behaviors listed. 
Web Demo:
Enter web_demo.put into the terminal and load the provided IP in your web browser.
