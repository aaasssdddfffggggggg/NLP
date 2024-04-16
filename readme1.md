1.模型、数据均预先下载到NLP2文件下。
2.自定义了compute_metrics函数以及用了余弦退火scheduler。
3.不使用from_pretrained API, 自己根据PPT内容搭建情感分类模型：把BERT 表示送入情感分类模型，然后进行训练情感分类模型的参数。
4.最终跑通不使用trainer训练的框架，把模型和数据均部署到gpu上进行训练，共训练50轮，并保留最优权重。
