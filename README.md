# LLaMA-Instruct-Learning

## Llama指令学习

- [Stanford Alpaca复现](https://github.com/tatsu-lab/stanford_alpaca)

> 基于llama-7b和alpaca 52数据进行指令微调

## LLaMA模型权重

| 模型名称| 基础模型     | 大小   | 模型地址 |
|-----|----------|------|----|
| LLama-7B-Alpaca | LLaMA-7B | 25GB |https://huggingface.co/quincyqiang/llama-7b-alpaca|



## Gradio Web 应用

```shell
python app.py
```

![](https://raw.githubusercontent.com/yanqiangmiffy/LLaMA-Instruct-Learning/main/images/app_screenshot.png)

## requirements

```text
datasets
loralib
sentencepiece
git+https://github.com/huggingface/transformers.git
accelerate
bitsandbytes
git+https://github.com/huggingface/peft.git
gradio
```
## Bugs

- TypeError: dispatch_model() got an unexpected keyword argument 'offload_index'

```text
!pip install --upgrade accelerate
```

- 如何上传模型到huggingface

```text
git lfs install
huggingface-cli lfs-enable-largefiles .
```

## 参考

- https://github.com/tatsu-lab/stanford_alpaca