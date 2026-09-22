---
license: other
language:
- zh
- en
tags:
- medical-books
- bilingual
- clinical-medicine
- 医学图书
configs:
- config_name: default
  data_files:
  - split: train
    path: metadata/books.jsonl
---

# 中英文现代医学图书精选 10 种｜Bilingual Medical Books Collection

从基础病理与药理，到临床内科、营养与消化，再延伸至重症医学、肺癌影像和眼肿瘤外科：本集精选中文、英文各 5 种医学图书，提供完整 PDF、逐册页数与 SHA-256 校验值，便于教学研读、专业检索和跨语言知识研究。它是图书资源集，不是临床诊疗建议，也不是经过标注的模型评测题库。

中文图书含扫描版及可检索版；英文图书均有文本层。扫描版未另行生成 OCR，文本抽取质量因原书而异。我们抽样检查了文件结构和正文页清晰度，未逐页校对原书内容。医学知识有时效性，实际诊疗请依最新规范及专业判断。

| 编号 | 书名 | 页数 | 文件形态 | MiB | GitHub 下载 |
| --- | --- | ---: | --- | ---: | --- |
| CN-01 | 病理学（本科临床配增值，第9版） | 394 | 扫描版 | 82.4 | [PDF](https://github.com/lengfeng650-star/modern-medical-books-bilingual-10/releases/download/v1.0/CN-01.pdf) |
| CN-02 | 药理学（第9版） | 1435 | 可检索版 | 29.6 | [PDF](https://github.com/lengfeng650-star/modern-medical-books-bilingual-10/releases/download/v1.0/CN-02.pdf) |
| CN-03 | 内科学（第8版，全国高等学校教材） | 986 | 扫描版 | 88.2 | [PDF](https://github.com/lengfeng650-star/modern-medical-books-bilingual-10/releases/download/v1.0/CN-03.pdf) |
| CN-04 | 中国居民膳食指南（2022） | 378 | 扫描版 | 70.8 | [PDF](https://github.com/lengfeng650-star/modern-medical-books-bilingual-10/releases/download/v1.0/CN-04.pdf) |
| CN-05 | 幽门螺杆菌及其相关疾病诊疗：成虹2020观点 | 311 | 扫描版 | 45.3 | [PDF](https://github.com/lengfeng650-star/modern-medical-books-bilingual-10/releases/download/v1.0/CN-05.pdf) |
| EN-01 | Oxford Handbook of Clinical Medicine — Mini Edition | 923 | 可检索版 | 20.9 | [PDF](https://github.com/lengfeng650-star/modern-medical-books-bilingual-10/releases/download/v1.0/EN-01.pdf) |
| EN-02 | Mayo Clinic Gastroenterology and Hepatology Board Review, 6e | 462 | 可检索版 | 44.7 | [PDF](https://github.com/lengfeng650-star/modern-medical-books-bilingual-10/releases/download/v1.0/EN-02.pdf) |
| EN-03 | Intensive Care Medicine: The Essential Guide | 802 | 可检索版 | 11.9 | [PDF](https://github.com/lengfeng650-star/modern-medical-books-bilingual-10/releases/download/v1.0/EN-03.pdf) |
| EN-04 | Diagnostic Imaging of Lung Cancers | 328 | 可检索版 | 27.7 | [PDF](https://github.com/lengfeng650-star/modern-medical-books-bilingual-10/releases/download/v1.0/EN-04.pdf) |
| EN-05 | Surgical Ophthalmic Oncology: A Collaborative Open Access Reference | 287 | 可检索版 | 25.9 | [PDF](https://github.com/lengfeng650-star/modern-medical-books-bilingual-10/releases/download/v1.0/EN-05.pdf) |

## 获取与核验

- GitHub：https://github.com/lengfeng650-star/modern-medical-books-bilingual-10；完整 PDF 以 v1.0 Release 附件发布，表中链接可直接下载。
- ModelScope：https://www.modelscope.cn/datasets/SHPDataGR/modern-medical-books-bilingual-10；目录为 `data/zh/` 和 `data/en/`，按平台设置须登录后下载。
- 两个平台共用 `metadata/books.jsonl` 书目索引，其中包含文件路径、页数、大小、ISBN（如可识别）和 SHA-256。`year` 仅在文件信息可确认时填写，否则为 `null`。
- 示例：`from modelscope.msdatasets import MsDataset; ds = MsDataset.load('modern-medical-books-bilingual-10', namespace='SHPDataGR')`，加载的是书目索引，PDF 须单独下载。

## 授权与使用边界

发布方已取得本批图书的上传与传播授权。书籍及其图表的著作权仍归各自权利人；本页面没有把书籍内容统一授权为 Apache、MIT 或其他通用许可证。下载、再分发、改编或商用的具体权利，应以适用的权利人授权为准。ModelScope 的“登录后下载”仅是访问设置，并非额外版权许可。

联系邮箱：zhouhaoran@shujuyoupu.com
