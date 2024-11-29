# Qwen-QwQ-32B-Preview

![FireShot Capture 028 - Qwen-QwQ-32B ipynb - Colab - colab research google com](https://github.com/user-attachments/assets/e02c94e1-09df-4464-87a0-2a6abeffb8e8)

QwQ-32B-Preview is an experimental research model developed by the Qwen Team, focused on advancing AI reasoning capabilities. As a preview release, it demonstrates promising analytical abilities while having several important limitations:

    Language Mixing and Code-Switching: The model may mix languages or switch between them unexpectedly, affecting response clarity.
    Recursive Reasoning Loops: The model may enter circular reasoning patterns, leading to lengthy responses without a conclusive answer.
    Safety and Ethical Considerations: The model requires enhanced safety measures to ensure reliable and secure performance, and users should exercise caution when deploying it.
    Performance and Benchmark Limitations: The model excels in math and coding but has room for improvement in other areas, such as common sense reasoning and nuanced language understanding.

Specification:

    Type: Causal Language Models
    Training Stage: Pretraining & Post-training
    Architecture: transformers with RoPE, SwiGLU, RMSNorm, and Attention QKV bias
    Number of Parameters: 32.5B
    Number of Paramaters (Non-Embedding): 31.0B
    Number of Layers: 64
    Number of Attention Heads (GQA): 40 for Q and 8 for KV
    Context Length: Full 32,768 tokens

For more details, please refer to our blog. You can also check Qwen2.5 GitHub, and Documentation.
Requirements

The code of Qwen2.5 has been in the latest Hugging face transformers and we advise you to use the latest version of transformers.

With transformers<4.37.0, you will encounter the following error:

KeyError: 'qwen2'
