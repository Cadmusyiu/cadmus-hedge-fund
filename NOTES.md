# Integration Notes

## What Would Change for Stock Dashboard

### Data Source Layer
- `src/tools/api.py` → Replace all `financialdatasets.ai` calls with Finnhub + yfinance
- Finnhub: price data, news, company metrics
- yfinance: financial statements, fundamental data

### Agent Selection (recommended for personal use)
Keep these 8 agents as dashboard panels:
1. Buffett → Quality/value scoring
2. Munger → ROIC/moat analysis  
3. Druckenmiller → momentum/growth
4. Burry → contrarian signals
5. Technical → RSI/MACD/trend
6. Fundamentals → financial health
7. Sentiment → market mood
8. Risk Manager → position sizing

### LLM Layer
- Already tested: DeepSeek works ✅
- Replace JSON Schema models with simpler prompt templates
- Reduce API calls (each agent currently calls LLM per ticker)

### UI Layer
- React frontend can be adapted as dashboard panels
- Each agent → one dashboard card/panel
- No graph workflow needed (simpler than LangGraph)
