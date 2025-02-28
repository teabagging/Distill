蒸馏
基于满血DeepSeek-R1蒸馏数据集

crypto ?OpenAI deepseekgrok 

🚀 中文开源蒸馏满血R1数据集
探索基于R1蒸馏的中文数据集，涵盖数学、考试、STEM和通用类型数据，总计110K样本。该数据集旨在帮助复现R1蒸馏模型的强大效果，特别适用于中文场景的微调训练。

下载数据集
📊 数据分布与字段说明
数据集包含：Math（36568样本）、Exam（2432样本）、STEM（12648样本）、General（58352样本）。字段包括：input（输入）、reasoning_content（思考）、content（输出）、repo_name（数据源）、score（模型打分）。

查看详情
🛠️ 数据蒸馏细节
数据蒸馏基于DeepSeek-R1官方细节：不增加额外系统提示词，temperature设置为0.6，数学数据增加推理提示词，强制输出以"\n"开头。数据生成调用无问芯穹企业版R1 API，支持64k上下文和32k输出长度。

了解更多
💡 数据打分与校验
Math和Exam数据使用Math-Verify和Qwen2.5-72B-Instruct模型打分，其他数据从无害性、有用性、正确性/完整性三个维度打分。二次校验使用8张A100 GPU部署Qwen72B模型，耗时近24小时。

查看打分细节
🔭 数据集局限性
数据由蒸馏DeepSeek-R1生成，未经严格验证，可能存在事实性不足。使用时请注意甄别，评分基于模型生成，仅供参考。

了解局限性
