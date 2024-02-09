Lesson 4: 
Intro to Finetuning:
A good framework is having a base dataset and then a dataset for instructions. Instruction tuning is needed to make the model answer the questions it is asked in a desired formats
Intro to XTuner:
InternLM used a slightly different format then LLaMA. For the pretrianing of the model, it is evaluated on how it completes the text, for instruction tuning it usually does it differently. Sometimes LoRA is used to make it less computationally intensive and use a lot less memory. LoRA is good while QLoRA is better and is able to use CPU memory as well if it runs out of VRam. 
XTuner Compatibly:
XTuner is compatible with all major model providers and Nvidia GPUs. Xtuner provides a unified interface to download models in different precisions and wit or without adapters. XTuner also comes with a helpful data format. 
What if I have no memory(8Gb)
You can also add flash attention.
InternLM Studio usage: 
Enter into your environment with SSH or other methods. To set up SSH you need your public key. Enter bash and then get started. You will then run various programs to install depencies. Make sure to create new directories to stay organized and not get confused. Download a dataset afterwards or use a built in one. There are various premade configuration modes for different models. You can change various things by directly editing the mode configuration models, the specific hyper parameters are in the GitHub documentation. Before finetuning, it will initialize and then tokenize the dataset. It loads it in a specific way.
Acceleration:
Deepspeed zero-2. After waiting you will see the loss flatter and converge. Deepspeed is very complex.
Tmux:
This guy likes Tmux. For good reason, we can leave it on while away. Tmux also means you can run other stuff.
The connection timed out. He enters make into his environmen and hopefully remembers. My guy made a mistake and tried to run the file for a long time and ran out of time. I feel somewhat bad for him. It did however save a checkpoint that was saved during training.
Maybe this was purposeful to teach how to convert pth to the huggingface format. There is also functionality to merge models. We can then have a conversation afterwards. You can also use quantization to make it faster.
Interesting Parameters:
Seed, top-p, tempature. There are other datasets we could try. For this example, let’s use MedQA.
Dataset Preparing:
First you have to sort the dataset, it is all in an excel spreadsheet which is not easy. Other programs are used to convert the excel spreadsheet into jsonl which is the proper framework. Move around some files, edit them, and at the end you can use it to train. The guy is cool cause he doesn’t like VIM, much respect. To get this to work properly, you must directly edit the applicable paremeters. 
Agents:
MSAgent is a framework supported. You can use it to enter queries into google. Lagent can also be ran. It was a good lesson.
