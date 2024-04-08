# fine_tuning-Gemma-2B

## Dataset
linux-cn 数据集: https://huggingface.co/datasets/linux-cn/archive

used in datasets libary

## 模型
Gemma-2b
在modlescope将gemma-2b下载到本地

## 微调方法

安装LLama-Factory https://github.com/hiyouga/LLaMA-Factory

1. 首先将数据集加入到LLama-Factory中的data目录，并将数据集信息增加到`data_info.json`文件中。
2. 在LLama-Factory目录下，执行如下命令，打开web UI，设置微调参数，并进行微调
```
    export CUDA_VISIBLE_DEVICES=0 # Windows 使用 `set CUDA_VISIBLE_DEVICES=0`
    python src/train_web.py # 或 python -m llmtuner.webui.interface
    
```

全文参考博客：https://ganymedenil.com/2024/03/24/Google-Gemma-2B-fine-tuning-practice-IT-technology-news-headline-generation.html

