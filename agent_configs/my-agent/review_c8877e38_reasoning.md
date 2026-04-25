# Bibliographic Audit - Paper c8877e38

## Paper Details
- **Title**: DIVE: Scaling Diversity in Agentic Task Synthesis for Generalizable Tool Use
- **ID**: c8877e38

## Audit Findings

### 1. Outdated arXiv Citations
Several entries cite arXiv preprints for works that have since been published in major venues:
- `mialon2023gaia`: Published as **"GAIA: A Benchmark for General AI Assistants"** at **ICLR 2024**.
- `xie2024travelplanner`: Published as **"TravelPlanner: A Benchmark for Real-World Planning with Language Agents"** at **ICML 2024**.
- `jimenez2023swe`: Published as **"SWE-bench: Can Language Models Resolve Real-World GitHub Issues?"** at **ICLR 2024**.

### 2. Missing Capitalization Protection (Braces)
A large number of technical terms, acronyms, and model names in titles lack curly brace `{}` protection, which will lead to incorrect lowercase rendering in standard styles:
- **Technical Acronyms**: `LLM`, `LLMs`, `EHR`, `MCP`, `GAIA`, `BIOASQ`, `API-Bank`.
- **Model/Method Names**: `Qwen3`, `EnvScaler`, `DeepSeek-V3.2`, `gpt-oss-120b`, `Gemini 2.5`, `Kimi k2`, `WebSailor`, `Webdancer`, `Webwalker`, `Webresearcher`, `DeepSeek-V3.2-Exp`, `MedAgentBench`, `TheAgentCompany`, `BrowseComp`, `FinSearchComp`, `FinAgentBench`, `BixBench`, `LegalAgentBench`, `SynthTools`, `Webexplorer`, `WebSailor-v2`, `TaskBench`, `MCP-Bench`, `MCP-AgentBench`, `AgentInstruct`, `GenTool`, `AgentRefine`, `ToolLLM`, `ToolAlpaca`, `DeepSeekMath`, `SWE-Dev`, `WebArena`, `AgentBench`, `DSBench`, `Mind2Web`, `SciCode`.
- **Other Proper Nouns**: `PubMed`.

### 3. Consistency and Metadata
- Inconsistent use of sentence case vs. title case in entries (e.g., `yang2025qwen3` vs `li2025websailor`).
- Some entries are missing conference page numbers despite being published (e.g., `li2025legalagentbench`).

## Conclusion
The bibliography requires extensive cleanup to update preprints to their formal conference versions and to ensure correct capitalization of technical terms through BibTeX brace protection. This will significantly improve the professional presentation of the manuscript.
