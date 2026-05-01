# Suicide Risk Detection using Large Language Models

This project investigates the use of large language models (LLMs) for detecting suicide risk from conversational data.

The system focuses on analysing human–AI dialogue and classifying risk levels into clinically relevant categories, supporting early screening in mental health applications.

## Models Used

Qwen2.5 7B Instruct – primary model with consistent and reliable outputs  
Mistral 7B Instruct – strong accuracy but inconsistent formatting  
Llama 3.1 8B Instruct – baseline model with weaker classification performance  

## Experiments

Multiple experiments were conducted to evaluate model performance and reliability.

Baseline evaluation on a structured human–AI dialogue dataset  
Prompt engineering experiment comparing zero-shot, few-shot, and constrained prompts  
Secondary dataset evaluation using Reddit mental health conversations  

Qwen2.5 demonstrated the most consistent and complete predictions  
Few-shot prompting improved both accuracy and output validity  
Performance decreased on real-world Reddit data due to increased variability  

## Repository Structure

notebooks/ → experiment notebooks  
results/ → evaluation outputs and model predictions  
figures/ → confusion matrices and visualisations  
docs/ → experiment summary  

## Final Words

I implemented and evaluated multiple large language models for suicide risk detection from conversational data. I conducted structured experiments, analysed both quantitative and qualitative results, and compared model behaviour to understand trade-offs between accuracy, consistency, and real-world reliability.

## Notes

All experiments were conducted using pre-trained open-weight models without additional fine-tuning. The focus of this project was on evaluating model performance, prompt design, and practical feasibility in safety-critical applications.

## External Resources

The following resources were used to support the implementation:

Qwen2.5: https://huggingface.co/Qwen  
Mistral: https://huggingface.co/mistralai  
Llama 3.1: https://huggingface.co/meta-llama  

All models were accessed through the Hugging Face Transformers library and executed in a cloud-based environment.

All experiments were executed, modified, and analysed independently as part of this project.
