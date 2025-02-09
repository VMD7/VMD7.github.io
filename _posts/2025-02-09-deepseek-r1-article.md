---
title: 𝗗𝗲𝗲𝗽 𝗦𝗲𝗲𝗸 𝘄𝗶𝘁𝗵𝗶𝗻 𝗗𝗲𝗲𝗽𝗦𝗲𝗲𝗸-𝗥𝟭🚀
tags: [LLM, DeepSeek]
style: fill
color: info
description: DeepSeek has introduced three major innovations in their latest research on the DeepSeek-R1 model, taking AI reasoning and performance to new heights. Here's a detailed breakdown of these exciting advancements
#external_url: https://blog.usejournal.com/how-to-undo-your-git-failure-b76e31ecac74
---

DeepSeek has introduced three major innovations in their latest research on the [DeepSeek-R1 model](https://github.com/deepseek-ai/DeepSeek-R1/blob/main/DeepSeek_R1.pdf), taking AI reasoning and performance to new heights. Here's a detailed breakdown of these exciting advancements:

## 𝗗𝗲𝗲𝗽𝗦𝗲𝗲𝗸-𝗥𝟭-𝗭𝗲𝗿𝗼
* 𝗧𝗿𝗮𝗶𝗻𝗲𝗱 𝗼𝗻 𝗟𝗮𝗿𝗴𝗲-𝗦𝗰𝗮𝗹𝗲 𝗥𝗲𝗶𝗻𝗳𝗼𝗿𝗰𝗲𝗺𝗲𝗻𝘁 𝗟𝗲𝗮𝗿𝗻𝗶𝗻𝗴 (𝗥𝗟): Built on DeepSeek V3, this model leverages the GRPO (Group Relative Policy Optimization) RL framework for improved reasoning.
* 𝗚𝗥𝗣𝗢 𝗙𝗿𝗮𝗺𝗲𝘄𝗼𝗿𝗸: Focuses on relative performance within groups, setting new benchmarks in AI reasoning. First introduced in April 2024, GRPO improves performance through step-by-step refinement, much like a group of students learning together.
* 𝗥𝗟 𝗢𝘃𝗲𝗿 𝗦𝗙𝗧: DeepSeek-R1-Zero relies entirely on RL, bypassing Supervised Fine-Tuning (SFT) to avoid complications like reward hacking and additional resource needs. The model doesn’t use a reward model, simplifying the training pipeline.
* 𝗣𝗿𝗼𝗺𝗽𝘁 𝗦𝘁𝘆𝗹𝗲: Reasoning is enclosed in <𝘁𝗵𝗶𝗻𝗸></𝘁𝗵𝗶𝗻𝗸>, and the answer in <𝗮𝗻𝘀𝘄𝗲𝗿></𝗮𝗻𝘀𝘄𝗲𝗿>, ensuring clear separation of thought process and output during training.
* 𝗣𝗲𝗿𝗳𝗼𝗿𝗺𝗮𝗻𝗰𝗲 𝗚𝗮𝗶𝗻𝘀: AIME improved from 15.6% to 71% after thousands of RL steps, with majority voting boosting accuracy to 86.7%. However, challenges remain in readability and language consistency.

## 𝗗𝗲𝗲𝗽𝗦𝗲𝗲𝗸-𝗥𝟭
* 𝗥𝗟 + 𝗖𝗼𝗹𝗱-𝗦𝘁𝗮𝗿𝘁 𝗗𝗮𝘁𝗮: Combines RL with a small amount of cold-start data in a multi-stage training process, with CoT (Chain-of-Thought) examples guiding reasoning.
* 𝗥𝗲𝗮𝗱𝗮𝗯𝗹𝗲 𝗢𝘂𝘁𝗽𝘂𝘁: Uses a response pattern with each answer summarizing the reasoning process, defined as: 
|𝘀𝗽𝗲𝗰𝗶𝗮𝗹_𝘁𝗼𝗸𝗲𝗻|<𝗿𝗲𝗮𝘀𝗼𝗻𝗶𝗻𝗴_𝗽𝗿𝗼𝗰𝗲𝘀𝘀>|𝘀𝗽𝗲𝗰𝗶𝗮𝗹_𝘁𝗼𝗸𝗲𝗻|<𝘀𝘂𝗺𝗺𝗮𝗿𝘆>.
* 𝗧𝗿𝗮𝗶𝗻𝗶𝗻𝗴 𝗔𝗽𝗽𝗿𝗼𝗮𝗰𝗵: Includes a few-shot prompting technique and post-processing by human annotators for clarity. The model is trained with 600k reasoning-related and 200k non-reasoning samples, finetuning DeepSeek-V3-Base over 2 epochs.
* 𝗥𝗲𝘄𝗮𝗿𝗱𝘀 𝗳𝗼𝗿 𝗖𝗼𝗻𝘀𝗶𝘀𝘁𝗲𝗻𝗰𝘆: RL training is guided by rewards for helpfulness, harmlessness, and language consistency.

## 𝗗𝗶𝘀𝘁𝗶𝗹𝗹𝗲𝗱 𝗠𝗼𝗱𝗲𝗹𝘀
* 𝗣𝗲𝗿𝗳𝗼𝗿𝗺𝗮𝗻𝗰𝗲 𝗕𝗿𝗲𝗮𝗸𝘁𝗵𝗿𝗼𝘂𝗴𝗵𝘀: Distilled models for both 32B and 70B architectures have set new performance benchmarks.
* 𝗦𝗙𝗧-𝗕𝗮𝘀𝗲𝗱: These models are distilled using 800k samples and rely solely on Supervised Fine-Tuning (SFT), leaving the exploration of RL for the community.
* 𝗙𝘂𝘁𝘂𝗿𝗲 𝗣𝗼𝘁𝗲𝗻𝘁𝗶𝗮𝗹: The RL exploration offers opportunities for further innovation in future iterations.
