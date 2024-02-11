Lesson 5:
LMDeploy intro:
LMDeploy has a lot of hardware support. Most models in the InternLM family are small. In larger models memory usage and GPU usage are way higher. Sometimes models will be ran multiple instances to run better in parallelism.  There is also dynamic batch size. Generating is somewhat simple in principle. 
Issues:
Running AI on a smartphone. It is a good example of hardware limitations and issues with compatibility, LMDeploy comes with an API but that’s talked about later. There is good news though! Lots of ways to optimize it. Deployment is an important implementation and should be worked on. LMDeploy brings together compatiblity with major frameworks and well-known tricks to spead up LLMs. Quantization is a top feature. 4 Bit and 8 Bit. You can Interact with the LLM through RESTFul. It is compatible with OpenCompass.
Performance:
Much higher throughput with w4a16. W stands for weights and a stands for activation. Activations are more sensitive to precision loss. KV Cache is used. Sometimes compute is memory bound or compute bound, too little memory or too little speed from the GPU. Kvcache is useful because it lets you choose your memory usage in a way. If you need less length in your samples this works especially well. GPTQ and AWQ are used to quantize. TurboMind is a special tool used which features blocked k/v cache, custom cuda kernels and more.
Batching:
Different batch slots may have persitant elements. In theory some of the techniques used can be used for infinite length.
More details on blocked K/v cache:
Pipeline is logic is modified, specifically focuses on the pipeline of the kv cache.
Other:
The cuda kernels are just good, no explaining needed. The people who wrote them know what they’re doing.
Tensor Parallelism:
Our different weights on different GPUs.
TurboMind is a way to improve the speed. They first have to convert it though.
You can use TurboMind as an api(with LM_Deploy)
LMDeploy has the same API as chatgpt. There is a built in Gradio interface. 
He talks about the various configurations for model params.
He talks about the difference between quantization levels. Int8 needs less VRAM.
W4A16 puts weights at 4 bit but still keeps activitations at fp16 precision.
