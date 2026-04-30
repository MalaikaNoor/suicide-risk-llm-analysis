# Experiment Summary

This project evaluates the use of large language models (LLMs) for detecting suicide risk from conversational data, focusing on classification across five clinically relevant categories: safe, indicator, ideation, behaviour, and attempt. The experiments aim to assess model performance, reliability, and practical suitability for use in safety-critical mental health applications.

## Baseline Model Evaluation

The first experiment involved evaluating three open-weight instruction-tuned models, Qwen2.5 7B Instruct, Mistral 7B Instruct, and Llama 3.1 8B Instruct, using a prompt-based classification approach on a structured dataset of human–AI dialogues. The results showed that all models were capable of identifying patterns related to suicide risk, but their performance varied significantly.

Qwen2.5 produced the most consistent and complete outputs across all cases, making it the most reliable model overall. Mistral achieved higher accuracy in some cases but generated inconsistent output formats, which reduced its evaluation coverage. Llama 3.1 demonstrated weaker performance and had difficulty distinguishing between risk levels, particularly in more nuanced cases.

## Prompt Engineering Experiment

The second experiment focused on evaluating the impact of prompt design on model performance. Different prompting strategies, including zero-shot, few-shot, and strict output formatting constraints, were tested to observe how they influence classification accuracy and output reliability.

The results showed that few-shot prompting consistently improved both prediction accuracy and output validity across all models. In contrast, strict formatting constraints reduced output errors but negatively impacted classification performance. This highlights the importance of balancing structure and flexibility in prompt design, as overly restrictive prompts may limit the model’s reasoning capability.

## Secondary Dataset Evaluation

The third experiment evaluated model performance on a secondary dataset derived from Reddit conversations. This dataset introduced more informal language, variability in expression, and less structured inputs compared to the primary dataset.

Performance across all models decreased on this dataset, reflecting the challenges of applying LLMs to real-world conversational data. Qwen2.5 remained the most consistent model, while Mistral and Llama showed increased variability in predictions. These results highlight the gap between controlled experimental settings and real-world deployment scenarios.

## Combined Insights

The experiments demonstrate that model performance in this task is influenced not only by model architecture but also by prompt design and data characteristics. While LLMs are capable of capturing contextual and linguistic signals associated with suicide risk, their reliability varies depending on input complexity and output constraints.

A key observation is the trade-off between accuracy and consistency. Models that achieve higher accuracy do not always produce usable outputs, particularly in structured classification tasks. This is especially important in safety-critical applications, where incomplete or inconsistent predictions can reduce the effectiveness of the system.

## Conclusion

Overall, the experiments show that large language models have strong potential for supporting early suicide risk detection from conversational data. Among the models evaluated, Qwen2.5 7B Instruct provides the most practical balance between performance and reliability. The results also emphasise the importance of prompt design, dataset quality, and human oversight in developing safe and effective AI systems for mental health applications.
