# llm-paraphrasing-attacks
Paraphrasing attacks are a technique where AI-generated text is perturbed by a paraphraser model to evade detection. This project explores the robustness of AI-text detection methods against such attacks.

We:
- Used a RoBERTa model trained by OpenAI to detect GPT-2 outputs as a baseline.
- Measured its effectiveness before and after paraphrasing the machine-generated text.
- Fine-tuned the RoBERTa model to detect GPT-3-generated scientific abstracts.
- Likewise evaluated the fine-tuned model’s performance before and after the paraphrasing attack.

Results:
- The GPT-2 detector’s recall dropped by ~8% under paraphrasing.
- The fine-tuned GPT-3 detector was unaffected by the attack, likely due to artifacts in the training data.

Paraphrasing was accomplished with T5 and Llama2 models. The full writeup is available in writeup.pdf.

