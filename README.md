# LLaMA-Instruct-Learning

## Llama指令学习

- [Stanford Alpaca复现](https://github.com/tatsu-lab/stanford_alpaca)
> 基于llama-7b和alpaca 52数据进行指令微调

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

## gradio demo
```shell
python app.py
```
![](https://raw.githubusercontent.com/yanqiangmiffy/LLaMA-Instruct-Learning/main/images/app_screenshot.png)
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