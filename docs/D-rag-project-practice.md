# 企业级 RAG 项目实践

企业知识库 RAG 问答系统

```mindmap
  Java Spring Boot
  ├── 用户/权限
  ├── 知识库管理
  ├── 文件上传
  ├── 会话管理
  ├── 反馈管理
  └── 调用 Python RAG 服务

Python FastAPI RAG Service
  ├── 文档解析
  ├── Chunk切分
  ├── Embedding
  ├── 向量检索
  ├── Rerank
  ├── Prompt构造
  ├── LLM生成
  └── Trace记录
```

- Java 负责业务系统、权限、流程、数据一致性
- Python 负责模型调用、RAG Pipeline、Embedding、检索链路



