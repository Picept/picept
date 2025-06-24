# Picept - AI Agent Reliability Platform

[![PyPI version](https://badge.fury.io/py/picept.svg)](https://badge.fury.io/py/picept)
[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)

Simulate, test, and optimize AI agents — catch failures before users do and deploy with confidence.

## 🎯 What is Picept?

Picept is an AI tracing and observability toolkit that powers **PiMax** - the first failure diagnosis and optimization engine for AI agents. Built from analyzing thousands of real production agent failures, PiMax helps you catch issues before they impact your users.

## 🚀 Meet PiMax

**PiMax** is trained on real agentic failures from production systems, enabling it to:

- 🔍 **Catch issues before users hit them** - Proactive failure detection
- 🧠 **Recognize 20+ failure patterns** - From hallucinations to tool misuse  
- ⚡ **Understand real-world breakdowns** - Not just theoretical scenarios
- 🎯 **Optimize agent performance** - Actionable insights for improvement

### Watch PiMax in Action
[![PiMax Demo](https://img.youtube.com/vi/MO_C0ftq964/0.jpg)](https://youtu.be/MO_C0ftq964?si=MppBq1x8tXuqSy0a)

## 📦 Installation

```bash
pip install picept
```

## 🏗️ Platform Support

Picept works seamlessly with all major AI agent frameworks:

- **OpenAI Agent SDK** - Full integration support
- **LangChain** - Complete trace capture for LangGraph workflows  
- **Custom OpenAI clients** - Any OpenAI-compatible implementation
- **Custom Anthropic clients** - Claude-based agent implementations
- **Multi-agent systems** - Complex workflow orchestration

## ⚡ Quick Start

```python
import picept
from openinference.instrumentation.langchain import LangChainInstrumentor

# Initialize Picept with auto-instrumentation
picept.init(
    project_id="your-project",
    api_key="your-api-key",
    integrations=[
        LangChainInstrumentor(),  # Auto-capture LangChain operations
    ]
)

# Your agent code runs normally - traces captured automatically
# PiMax analyzes execution patterns for failure detection
```

## 🔍 Failure Detection Capabilities

PiMax detects 20+ distinct failure modes including:

**Core Agent Issues:**
- Hallucinations (content & tool-based)
- Tool response misreading  
- Task misunderstanding
- Objective drift

**Operational Problems:**
- Wrong tool usage
- Output format issues
- Instruction violations
- Context loss

**System-Level Failures:**
- HTTP errors & timeouts
- Resource limit issues
- Environment problems
- Performance bottlenecks

## 📚 Documentation & Examples

- **[Getting Started Guide](https://docs.picept.ai/pimax/getting-started)** - Complete setup and usage examples
- **[PiMax Documentation](https://docs.picept.ai)** - Full platform documentation
- **[Picept Platform](https://picept.ai)** - Try PiMax free

## 🛠️ Why Picept?

Building reliable AI agents is challenging. They fail in unexpected ways - objective drift, tool misreading, context loss that cascades into wrong outputs. Traditional debugging approaches miss the subtle failure modes that emerge in production.

Picept solves this by bringing battle-tested failure detection directly to your development process. Instead of learning the hard way through production incidents, leverage PiMax's knowledge to prevent issues before they impact users.

## 🤝 Contributing

We welcome contributions! Please see our [GitHub repository](https://github.com/Picept/picept) for guidelines.

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

---

**Ready to maximize your agent's reliability?** [Get started with PiMax](https://docs.picept.ai/pimax/getting-started) and catch failures before your users do.