# Soufien Hajji — AI & Data Architecture

I build production systems where AI, data engineering, cloud architecture and verifiable evidence meet. Based in Luxembourg; working in English and French.

I am open to **AI Engineer** and **AI/Data Solution Architect** roles.

## Flagship work

| Project | Problem solved | Engineering evidence |
| --- | --- | --- |
| [Lex](https://law.soufien.lu) · [case study](https://sfhajji.github.io/lex/) · [source](https://github.com/SFHAJJI/lex) | Read and compare what Luxembourg and EU law said on a chosen date, article by article, with the official source and a permalink. | Formex and Akoma Ntoso parsed into relational SQLite indexes; deterministic question parsing; structure-first retrieval with no vector store; typed answers and twenty typed refusals instead of generated text; machine gates with shuffled controls; reproducible, signed releases on Azure Container Apps; a public MCP server. |
| [guide-rag: a documentary chatbot for newcomers](https://sfhajji.github.io/guide-rag/) | Answer a newcomer's question from a public guide to Luxembourg with a verbatim quote and its path (page › section › lines), or a justified absence. | Built brick by brick (document parsing into relational tables, question parsing with an expert dictionary, retrieval as filtering with anchor and context, typed generation validated against the index); no vector store, no model needed (one is optional under the same contract); 46 labelled questions at 100 % with 100 % quote fidelity; the browser runs a port of the Python pipeline, verified identical. Source: [SFHAJJI/guide-rag](https://github.com/SFHAJJI/guide-rag).
| [Energy Copilot](https://sfhajji.github.io/energy/) · [source](https://github.com/SFHAJJI/energy-copilot) | Turn public geospatial, tender, tariff and legal data into traceable solar-prospecting decisions. | Azure agentic RAG with deterministic tools, PostGIS, source citations, security controls, observability and cost controls. The public deployment is offline; the architecture page documents it. |

The emphasis is not a chatbot demo. It is the work that makes an AI product defensible: temporal data models, retrieval quality, provenance, typed failure modes, deployment safety, operational cost and honest limitations. Lex's assistant is built to a typed answer contract (the model only plans; code validates and quotes) and is switched off until its gates pass.

Try the public, read-only Lex MCP server without a key:

```bash
claude mcp add --transport http lex https://law.soufien.lu/mcp
```

## Start here

- [Portfolio](https://sfhajji.github.io/) and the [Lex case study](https://sfhajji.github.io/lex/)
- [CV](https://sfhajji.github.io/cv/) (English and French)
- [What Lex holds today](https://law.soufien.lu/en/coverage.html), class by class, with what it lacks
- [Public Luxembourg legal corpus](https://github.com/SFHAJJI/lex-corpus-lu-legilux) and [reviewed EU corpus](https://github.com/SFHAJJI/lex-corpus-eu-eurlex)
- Contact: [haji.soufien@gmail.com](mailto:haji.soufien@gmail.com)

I welcome technically serious feedback, legal-domain review and conversations about responsible AI systems in regulated environments.
