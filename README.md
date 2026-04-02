# Diversion-rules

常用 AI 服务分流规则集合。

## 文件说明

- `openai.yaml`
  - OpenAI 完整版分流规则
  - 包含核心域名，以及登录、静态资源、监控、客服等常见依赖域名
- `openai-pure.yaml`
  - OpenAI 严格版分流规则
  - 仅保留 OpenAI 核心访问域名
- `gemini.yaml`
  - Gemini 完整版分流规则
  - 包含核心域名，以及登录、静态资源、Google Maps、YouTube 等常见依赖域名
- `gemini-pure.yaml`
  - Gemini 严格版分流规则
  - 仅保留 Gemini 核心访问域名和前端静态资源常见依赖

## 使用建议

- 如果希望功能尽量完整，优先使用 `openai.yaml` 或 `gemini.yaml`
- 如果希望分流范围尽量收敛，优先使用 `openai-pure.yaml` 或 `gemini-pure.yaml`

## 说明

- `pure` 版本更适合严格控制规则范围的场景
- 完整版更适合直接投入日常使用，减少因依赖域名缺失导致的访问异常
