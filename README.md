# Latency-Comparision-of-LLM-and-vLLM
Project is to measure and compare the response times (latency) of VLLM and LLM for the same input prompt. This can help in understanding the performance differences between these models in real-time applications.

## Workflow
- Model Initialization: Both VLLM and OpenAI's LLM are initialized.
- Prompt Definition: A sample context and a related question are defined.
- Latency Measurement: A function measures the time taken by each model to generate a response to the given prompt.
- Output Display: The latency and generated output for each model are printed.

## Need For vLLM
- Slow inference speeds on expensive hardware.
- LLMs, by their nature, are massive in scale and requires substantial computational resources, which can lead to increased latency during the inference phase. This not only affects the responsiveness but also escalates the costs associated with maintaining such systems.

## PagedAttention - The Game Changer
- vLLM utilizes PagedAttention mechanism which efficiently manages attention keys and values, significantly improving throughput without altering models architecture.

Go through this blog https://blog.vllm.ai/2023/06/20/vllm.html to know more about vLLM and its funtionality.

## Output and Latency Images of LLM and vLLM 
<img width="198" alt="image" src="https://github.com/SaikiranBSK10/Latency-Comparision-of-LLM-and-vLLM/assets/66936785/acd9fd23-4424-4a9e-a632-9b300b1bbc6d">

<img width="393" alt="image" src="https://github.com/SaikiranBSK10/Latency-Comparision-of-LLM-and-vLLM/assets/66936785/c44761a0-5629-49ed-88a3-eb9658ee11bf">

## Citation 
```
@inproceedings{kwon2023efficient,
  title={Efficient Memory Management for Large Language Model Serving with PagedAttention},
  author={Woosuk Kwon and Zhuohan Li and Siyuan Zhuang and Ying Sheng and Lianmin Zheng and Cody Hao Yu and Joseph E. Gonzalez and Hao Zhang and Ion Stoica},
  booktitle={Proceedings of the ACM SIGOPS 29th Symposium on Operating Systems Principles},
  year={2023}
}

