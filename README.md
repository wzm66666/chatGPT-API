# 《ChatGPT AI 问答助手》

### 1. 项目介绍

**《ChatGPT AI 问答助手》** 涵盖爬虫接口、ChatGPT API对接、DDD架构设计、镜像打包、Docker容器部署。

**注意**：
1. 技术栈：Java、SpringBoot、爬虫、ChatGPT、job、Docker
2. OpenAi Keys 申请：[https://beta.openai.com/account/api-keys](https://beta.openai.com/account/api-keys) 。


### 2. 模型训练

#### 2.1 环境安装

- 下载 Python：[https://www.python.org/downloads/macos/](https://www.python.org/downloads/macos/) 3.6版本以上
- 配置 Python：
    1. 搜索地址 `which python3`
    2. 环境配置 `alias python="/Library/Frameworks/Python.framework/Versions/3.10/bin/python3"`
    3. 生效配置 `source .bash_profile`
    
- 安装 pip：以下需要用到 pip 指令，如果没有需要安装 'curl https://bootstrap.pypa.io/get-pip.py | python3'

#### 2.3 tensorflow

地址：[https://www.tensorflow.org/install?hl=zh-cn](https://www.tensorflow.org/install?hl=zh-cn)

脚本：

```python
# Requires the latest pip
pip install --upgrade pip

# Current stable release for CPU and GPU
pip install tensorflow

# Or try the preview build (unstable)
pip install tf-nightly
```

mac m1：`python3 -m pip install tensorflow-macos`

测试：

```python
python3 -c "import tensorflow as tf; print(tf.reduce_sum(tf.random.normal([1000, 1000])))"

# 结果；tf.Tensor(228.22836, shape=(), dtype=float32)
```
