# Cadmus Hedge Fund — Analysis Notes

## Source
Forked from [virattt/ai-hedge-fund](https://github.com/virattt/ai-hedge-fund) (v2026.5.9)

## Purpose
Educational reference for stock dashboard development.
Analyzing multi-agent architecture for potential adaptation.

## Security Assessment ✅
- No malware / scam code found
- All external APIs are legitimate (financialdatasets.ai, LLM providers)
- No crypto wallet addresses
- `subprocess` usage is only for local Ollama management

## Key Architecture
19 agents structured as:
- **Value investors**: Buffett, Graham, Munger, Pabrai, Jhunjhunwala
- **Growth investors**: Cathie Wood, Peter Lynch, Phil Fisher
- **Contrarian**: Michael Burry, Bill Ackman
- **Macro**: Druckenmiller, Damodaran
- **Risk**: Taleb (tail risk), Risk Manager
- **Functional**: Technical, Fundamental, Sentiment, Valuation, News

## Planned Adaptation for Stock Dashboard
- Replace `financialdatasets.ai` → **Finnhub + yfinance** (free)
- Select subset of agents suitable for personal use
- Keep DeepSeek LLM integration (already tested ✅)
- Simplify LangGraph workflow for dashboard panels

## Status
- 🔬 Analysis phase (post Fukuoka trip)
- Dependencies: Finnhub API, DeepSeek API (both available)
