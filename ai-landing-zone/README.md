# AI Landing Zone: Secure GenAI Infrastructure

This module provides the blueprints for deploying **Azure OpenAI**, **AWS Bedrock**, or **GCP Vertex AI** within a strictly governed enterprise perimeter.

## 🛡️ Reference Architecture: Secure LLM

1.  **Private Endpoints**: LLM services are never exposed to the public internet.
2.  **API Management**: Centralized gateway for rate limiting, token tracking, and logging.
3.  **Enterprise RAG**: Secure connectors specifically for vector databases (Pinecone, Weaviate, AI Search).
4.  **Governance**: Guardrails to prevent data leakage and ensure PII stripping.

## 🚀 Getting Started

Deploy the core AI security stack:
```bash
terraform init
terraform apply -target=module.ai_security_perimeter
```
