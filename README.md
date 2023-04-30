# chatgpt_research


1 经典论文：
1）极简综述：GPT_4，通用人工智能的火花
2）主要的几篇论文：https://hub.baai.ac.cn/view/24227

我们可以得出结论：

* 1）基础能力（gpt3）：语言生成能力 + 基础世界知识 + 上下文学习都是来自于预训练（davinci/gpt3）
* 2）指令能力和推理能力（code-davinci）
* 指令泛化：遵循指令和泛化到新任务的能力来自于扩大指令学习中指令的数量（Davinci-instruct-beta)
* 推理能力。执行复杂推理的能力很可能来自于代码训练（code-davinci-002）
* 3）人类对话提升-多轮对话和翔实的结果(chatgpt)
    * 生成中立、客观的能力、安全和翔实的答案来自与人类的对齐。具体来说：
        * 如果是监督学习版，得到的模型是text-davinci-002
        * 如果是强化学习版 (RLHF) ，得到的模型是text-davinci-003
        * 无论是有监督还是 RLHF ，模型在很多任务的性能都无法超过 code-davinci-002 ，这种因为对齐而造成性能衰退的现象叫做对齐税。
    * 对话能力也来自于 RLHF（ChatGPT），具体来说它牺牲了上下文学习的能力，来换取：
        * 建模对话历史
        * 增加对话信息量
        * 拒绝模型知识范围之外的问题

# chatgpt application

* chatgtpt vs RS (disadvantage). can chaggpt replace recommendation system? 1)in the accuracy metric, chatgpt can't beat current RS. 2)in other ereas, such as content eco-system, user increasement, chatgpt can not even understand the question or we can't give it promts. 

* chatgpt vs RS (advantage). it' s basially search. It provides so much good result so that we dont need to scan pages. but different like Search, besides relevance, it can provide quick fix to negtive feedback, interpretallity, and other  metrics. So it can have more utilities than RS had.

* from human's perspective, all that gpt cant do maybe the long term optimization and content-side eco-system.

