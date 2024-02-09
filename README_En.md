# InternLMCourse

General Intro:
Large language models became a very important part of the web following the results of ChatGPT, which had hit 100M users.
AI over time became more general, it used to be only AI which would do specific things but now with new systems are more general.
History of InternLM:
Released originally in 6/7, as a partly propriety model while a smaller model was open sourced.
The model lineup has open models with 7B and 20B models, 123B has not been open sourced but these other models are incredibly useful. At the time of releasing 20B,  it outperformed all other models in its weight class.
Usage:
There are a variety of things one can do with LLMs, and it is not really always simple to use LLMs properly. For more complicated situations it’s often better to use open source, in special cases or with inference restrictions you can fine tune. There are lots of frameworks available to make this easier.
InternLM Toolchain:
Pretrianing dataset is 2Tb dataset, and the model is trained using InternLM-Train which can be further trained using XTuner. OpenCompass is a framework for evaluate capabilities and Agents is used to connect InternLM to external programs.
Dataset Contents:
High quality data and text in order to align with China’s value.
OpenDataLab Platform stats and examples.
80TB+ total data, very comprehensive.
InternLM Training advantage:
High GPU scalability and high throughput.
Finetuning paradigms:
LoRA is a very popular method to train models, while SFT is the way it calculates the values of the model.
XTuner:
XTuner has high compatibly with various frameworks and large langauge models, working on both consumer GPUs and enterprise. Using XTuner is also extremely high performance with XTuner.
Evaluations and Partners.
Evaluations are developed by high quality institutions and include lots of English and Chinese data. OpenLLM is maintained by HuggingFace.
OpenCompass is another large evaluation harness that is useful and focuses on a large amount of qualities in the LLM.
OpenCompass has a lot of different models that have been benchmarked, especially open models from China but also United States models and proprietary models. Organizations choose OpenCompass. 
Deployment:
A complex part of the serving of AI models is memory usage, the LMDeploy framework is able to fix these issues with various tricks and is able to drastically decrease memory usage. LMDeploy has compatibly with OpenAI API and RESTFul and will be able to fit into your usage whey well. Very fast throughput compared to competition.
Agents:
The agent framework is able to allow an LLM to plan and execute various complex task using different call chains. Lagent has compatiblity with most major model providers. AgentLego makes it easy to assemble different models and tools to execute tasks you need to complete.
Summary:
They talked about various tools in the OpenMM family, which are all useful.
