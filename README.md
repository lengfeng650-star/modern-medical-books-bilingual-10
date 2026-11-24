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

## 直接下载

- [逐文件下载](https://github.com/lengfeng650-star/modern-medical-books-bilingual-10/blob/main/meta/downloads.md)

## 获取与核验

- GitHub：https://github.com/lengfeng650-star/modern-medical-books-bilingual-10；完整 PDF 以 v1.0 Release 附件发布，表中链接可直接下载。
- ModelScope：https://www.modelscope.cn/datasets/SHPDataGR/modern-medical-books-bilingual-10；目录为 `data/zh/` 和 `data/en/`，支持免登录下载。
- 两个平台共用 `metadata/books.jsonl` 书目索引，其中包含文件路径、页数、大小、ISBN（如可识别）和 SHA-256。`year` 仅在文件信息可确认时填写，否则为 `null`。
- 示例：`from modelscope.msdatasets import MsDataset; ds = MsDataset.load('modern-medical-books-bilingual-10', namespace='SHPDataGR')`，加载的是书目索引，PDF 须单独下载。

## 授权与使用边界

发布方已取得本批图书的上传与传播授权。书籍及其图表的著作权仍归各自权利人；本页面没有把书籍内容统一授权为 Apache、MIT 或其他通用许可证。下载、再分发、改编或商用的具体权利，应以适用的权利人授权为准。

联系邮箱：zhouhaoran@shujuyoupu.com
