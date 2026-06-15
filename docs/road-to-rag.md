# RAG 转型之路
> 先搭骨架（体系框架） → 再补血肉（知识填充） → 再练肌肉（实践练习） → 最后形成能力闭环。

## 1 整体策略

转型的目标是建立一套清晰的能力闭环：
> Python 工具能力 → 大模型应用开发基础 → RAG 专项能力 → 企业级项目实践 → 作品集/面试表达

这四层各自解决不同问题：
| 层级        | 解决的问题        | 你的目标             |
| --------- | ------------ | ---------------- |
| Python 基础 | 怎么写代码        | 能写 Python RAG 服务 |
| 大模型应用基础   | 怎么调用和控制大模型   | 能做稳定的 LLM 应用     |
| RAG 技能体系  | 怎么让模型基于知识库回答 | 能做企业知识库问答系统      |
| 项目实践      | 怎么落地成真实系统    | 能形成工作能力和面试项目     |

一句话总结：
> Python 是工具，LLM 应用开发是通用底座，RAG 是专项能力，企业知识库项目是最终落地场景。

## 2 搭建 4 个技能体系
- [Python 技能体系](./01-python-skill-system.md)
- [LLM 应用开发技能体系](./02-llm-skill-system.md)
- [RAG 技能体系](./03-rag-skill-system.md)
- [企业级 RAG 项目实践](./04-rag-project-practice.md)

## 3 NotebookLM 使用策略

先搭框架，再找资料，再用 NotebookLM 填充框架，最后通过实践巩固。

### Notebook 1：Python 基础与工程

- 加入资料：
```text
  Python 官方教程--Data Structures 章节
  FastAPI 官方文档
  Pydantic 官方文档
  Pytest 官方文档
  Real Python 精选文章
  Automate the Boring Stuff with Python 相关章节
```

- 用途：
```text
  解决 Python 怎么写
  解决 Python 工程怎么组织
  解决 FastAPI 服务怎么开发
  解决 pydantic / pytest / logging 怎么用
```

- 优先级：
| 优先级  | 资料                    |
| ---- | ------------------------- |
| 主线   | Python 官方教程、FastAPI 官方文档  |
| 重点补充 | Pydantic、Pytest         |
| 查阅型  | Real Python               |
| 练习型  | Automate the Boring Stuff |

### Notebook 2：LLM 应用开发基础

- 核心资料
```text
  LLM Cookbook
  大模型应用开发极简入门
  OpenAI Cookbook
  模型厂商 API 文档
  Prompt Engineering 资料
  Function Calling / Tool Calling 资料
  结构化输出资料
  流式输出资料
  LLM 应用评估资料
```

- 用途：
```text
  解决如何调用模型
  解决如何写 Prompt
  解决如何组织 messages
  解决如何做结构化输出
  解决如何做 Tool Calling
  解决如何做日志、重试、成本控制
```

- 优先级：
| 优先级  | 资料                       |
| ---- | ------------------------ |
| 主线   | LLM Cookbook、大模型应用开发极简入门 |
| 实战参考 | OpenAI Cookbook          |
| 查阅型  | 模型厂商 API 文档              |
| 进阶补充 | Prompt、Tool Calling、评估资料 |


### Notebook 3：RAG 主线知识库

- 核心资料
```text
  大模型RAG实战
  LlamaIndex RAG 官方文档
  LangChain RAG 官方文档
  Qdrant 官方文档
  Milvus 官方文档
  pgvector / Elasticsearch Vector 资料
  RAGAS 资料
  Anthropic Contextual Retrieval 资料
  RAG 经典论文
```

- 用途：
```text
  解决 RAG 怎么设计
  解决文档怎么解析
  解决 chunk 怎么切
  解决 embedding 怎么选
  解决向量库怎么用
  解决 hybrid search / rerank 怎么优化
  解决 RAG 怎么评估
```

- 优先级：
| 优先级   | 资料                        |
| ----- | ------------------------- |
| 主线    | 大模型RAG实战                  |
| 工程参考  | LlamaIndex、LangChain      |
| 向量库参考 | Qdrant、Milvus、pgvector    |
| 评估参考  | RAGAS                     |
| 进阶优化  | Contextual Retrieval、经典论文 |


### Notebook 4：项目实践复盘

- 主要资料：
```text
  你的代码
  README
  架构图
  接口文档
  报错记录
  调参记录
  RAG评估表
  Prompt版本记录
  项目复盘文档
  面试项目讲稿
```

- 用途
```text
  把资料知识转化成你自己的项目经验
  沉淀可复用模板
  准备面试表达
  记录真实问题和解决方案
```

## 4 学习节奏

### 阶段 1：搭建学习框架
- 周期：1–2 天
- 目标：
  ```text
    建立 Python 技能树
    建立 LLM 应用基础技能树
    建立 RAG 技能树
    建立三者映射关系
    建立 4 个 NotebookLM
  ```
- 产出：
  ```text
    《Python基础编程技能体系》
    《大模型应用开发基础技能体系》
    《RAG编程技能体系》
    《Python + LLM + RAG 衔接表》
  ```

### 阶段 2：Python 最小能力
- 周期：1 周
- 目标：学 RAG 必需的 Python 能力
  ```text
    list / dict
    字符串处理
    文件读写
    JSON
    函数
    类型注解
    pydantic
    requests / httpx
    FastAPI
    logging
    pytest
  ```
- 练习：
  ```text
    读取一个 Markdown/TXT 文件
    按段落切分
    封装成 list[dict]
    保存为 JSON
    写一个 FastAPI 接口返回 chunks
  ```

### 阶段 3：LLM 应用开发基础
- 周期：1 周
- 重点掌握：
  ```text
    Chat API 调用
    Messages结构
    System Prompt
    Prompt模板
    结构化输出
    流式输出
    Function Calling
    调用日志
    token成本
    错误重试
  ```

- 练习：
  ```text
    写一个 /chat 接口
    接收 query
    构造 messages
    调用模型
    返回结构化 JSON
    记录耗时和 token
  ```

### 阶段 4：手写最小 RAG

- 周期：1–2 周
- 手写：
  ```text
    load_document()
    split_text()
    embed_chunks()
    save_vectors()
    retrieve()
    build_prompt()
    generate_answer()
  ```
先不要急着用 LangChain / LlamaIndex。手写一遍，目标是理解底层链路。

- 项目结构：
```text
  mini-rag/
    loader.py
    splitter.py
    embedding.py
    retriever.py
    generator.py
    app.py
    data/
    output/
```

### 阶段 5：框架化 RAG
- 周期：2 周
- 开始接入：
  ```text
    LlamaIndex 或 LangChain
    Chroma / Qdrant / Milvus / pgvector
    Rerank
    Hybrid Search
    引用来源
    基础评估
  ```
- 建议优先：
  ```text
    LlamaIndex：适合知识库问答
    LangChain：适合链路编排和Agent
  ```

## 5 知识体系衔接

- Python → LLM 应用开发
| Python 能力      | LLM 应用场景            |
| -------------- | ------------------- |
| dict / list    | messages、tools、模型响应 |
| JSON           | 结构化输出、接口返回          |
| requests/httpx | 调用模型 API            |
| pydantic       | 请求响应建模、输出校验         |
| FastAPI        | 封装大模型服务             |
| logging        | 记录模型调用链路            |


- LLM 应用开发 → RAG
| LLM 应用基础         | RAG 中的作用                  |
| ---------------- | ---------------------------- |
| Token            | 决定 chunk 和 prompt 长度         |
| Messages         | 构造问答请求                       |
| System Prompt    | 约束答案边界                       |
| 结构化输出            | 返回 answer/sources/confidence |
| Function Calling | 调用检索、工具、业务接口             |
| 流式输出             | 改善问答体验                    |
| Trace            | 排查检索和生成问题                  |


- RAG → 企业级项目
| RAG 能力          | 企业项目能力    |
| --------------- | --------- |
| 文档解析         | 文件上传、索引任务 |
| Chunk           | 知识单元管理    |
| Embedding       | 向量索引       |
| Metadata Filter | 权限和租户隔离  |
| Retrieval       | 知识召回      |
| Rerank          | 精准排序      |
| Prompt          | 答案生成      |
| Evaluation      | 效果优化      |
| Trace           | 线上排查      |

## 6 实践项目清单
| 项目           | 训练能力                |
| ------------- | ----------------------- |
| 1.Python 文档切分器   | Python 文件、字符串、list/dict |
| 2.FastAPI Chat 服务  | API、pydantic、HTTP          |
| 3.LLM 结构化输出服务  | Prompt、JSON、输出校验        |
| 4.Embedding 检索 Demo | 向量化、相似度、TopK          |
| 5.Mini RAG 系统      | 完整 RAG 链路                  |
| 6.LlamaIndex / LangChain RAG 系统  | 工程效率和框架能力    |
| 7.Java + Python 企业知识库 RAG 系统 | 系统设计和生产化能力  |

















