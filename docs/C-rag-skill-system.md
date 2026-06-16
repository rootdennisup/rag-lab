# RAG 技能体系

### 技能体系
```mindmap
  root((RAG编程技能体系))
    基础认知
      RAG是什么
      解决什么问题
      与微调区别
      典型应用场景
    数据摄取
      文档上传
      文档解析
      文本清洗
      元数据提取
    文本切分
      chunk_size
      chunk_overlap
      按段落切分
      按标题切分
      语义切分
    向量化
      Embedding概念
      Embedding模型选择
      向量维度
      向量质量
    检索系统
      向量检索
      BM25
      Hybrid_Search
      Metadata_Filter
      TopK
    检索优化
      Query_Rewrite
      Multi_Query
      Rerank
      Contextual_Retrieval
    生成阶段
      Prompt拼接
      上下文构造
      引用来源
      拒答策略
    评估与观测
      Retrieval_Recall
      Context_Precision
      Faithfulness
      Hallucination
      Tracing
    工程化落地
      LlamaIndex
      LangChain
      Vector_DB
      FastAPI服务化
      Java集成
      权限控制
```

### 学习资料

- 主线资料

  | 资料                  | 用途                              |
  | -------------------- | --------------------------------- |
  | 《大模型RAG实战》      | 主教材，建立 RAG 系统框架          |
  | LLM Cookbook         | 快速补应用代码感                    |
  | LlamaIndex 官方文档      | 学知识库、索引、检索、query engine     |
  | LangChain 官方文档       | 学 RAG chain、retriever、agentic RAG |
  | Qdrant / Milvus 官方文档 | 学向量库工程化                        |


- 进阶资料

  | 资料                             | 用途                  |
  | ------------------------------ | ------------------- |
  | RAGAS 文档 / 论文               | 学 RAG 评估            |
  | Anthropic Contextual Retrieval | 学进阶检索优化             |
  | Haystack 官方文档               | 学 pipeline 式 RAG 架构 |
  | FlashRAG 论文 / 项目            | 了解 RAG 研究型工具与方法集合 |
  | Lewis et al. RAG 论文          | 理解 RAG 原始思想         |


### 最小验收标准

- [☑️] 能解释完整 RAG 链路
- [ ] 能完成文档解析和文本切分
- [ ] 能调用 embedding 模型
- [ ] 能把 chunk 写入向量库
- [ ] 能完成 query 检索
- [ ] 能实现 rerank 或至少理解 rerank 作用
- [ ] 能拼接 prompt 并生成答案
- [ ] 能返回引用来源
- [ ] 能设计基础评估集
- [ ] 能把 RAG 封装成 API 服务







