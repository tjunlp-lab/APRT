# APRT

The official implementation of our COLING-2025 paper "[Automated Progressive Red Teaming](https://arxiv.org/abs/2407.03876)"


## Abstract
Ensuring the safety of large language models (LLMs) is paramount, yet identifying potential vulnerabilities is challenging. While manual red teaming is effective, it is time-consuming, costly and lacks scalability. Automated red teaming offers a more cost-effective alternative, automatically generating adversarial prompts to expose LLM vulnerabilities. However, in current efforts, a robust framework is absent, which explicitly frames red teaming as an effectively learnable task. To address this gap, we propose Automated Progressive Red Teaming (APRT) as an effectively learnable framework. APRT leverages three core modules: an Intention Expanding LLM that generates diverse initial attack samples, an Intention Hiding LLM that crafts deceptive prompts, and an Evil Maker to manage prompt diversity and filter ineffective samples. The three modules collectively and progressively explore and exploit LLM vulnerabilities through multi-round interactions. In addition to the framework, we further propose a novel indicator, Attack Effectiveness Rate (AER) to mitigate the limitations of existing evaluation metrics. By measuring the likelihood of eliciting unsafe but seemingly helpful responses, AER aligns closely with human evaluations. Extensive experiments with both automatic and human evaluations, demonstrate the effectiveness of APRT across both open- and closed-source LLMs. Specifically, APRT effectively elicits 54\% unsafe yet useful responses from Meta's Llama-3-8B-Instruct, 50\% from GPT-4o (API access), and 39\% from Claude-3.5 (API access), showcasing its robust attack capability and transferability across LLMs (especially from open-source LLMs to closed-source LLMs).

<img src="APRT.png" width="1000">

## Updates

- (**2024/7/4**) Our paper is on arXiv! Check it out [here](https://arxiv.org/abs/2407.03876)!
- (**2024/11/30**) Our paper is accepted by COLING-2025!
- (**2024/12/18**) We have released a quick implementation of APRT, including seed data and code!

## Quick Start
