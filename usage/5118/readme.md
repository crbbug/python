# 词语分析聚合
* 对 5118 网站下载的长尾词进行分析、聚合
* 提供两种聚合的方法：**余弦相似度聚合**、**机器学习 Kmeans 聚合**

## 使用方法

### 准备工作

* 将 5118 下载的所有文件放到 zip 目录下（不需要解压）
* 安装 python3.9, [官网](https://www.python.org/downloads/release/python-390/)
* 在根目录下（5118） 下打开终端，依次执行以下命令

```shell script
python3.9 -m venv venv
source venv/bin/activate （Mac）
.\venv\Scripts\activate.bat （Windows）
pip install -r requirements.txt -i https://pypi.doubanio.com/simple
```

### 一、使用余弦相似度进行聚合
* **确保准备工作已经被执行**
* 在根目录（5118） 终端下，执行 `python cosine.py`
* 程序执行完之后将输出两个文件，`keys.csv`,`res.xlsx`
* 其中 keys.csv 是所有的关键词，res.xlsx 是分类之后的结果


### 二、使用机器学习 Kmeans 进行聚合
* **确保准备工作已经被执行**
* 在根目录（5118）终端下，执行 `python kmeans.py`
* 这个方法需要修改一个参数 `clusters_count`, 详见代码的说明
* 程序执行完之后将输出两个文件，`keys.csv`,`res.xlsx`
* 其中 keys.csv 是所有的关键词，res.xlsx 是分类之后的结果

如果有问题，欢迎微信讨论

<img src="/Wechat.jpeg" width = "220" align=center />
