# AskEider

**Ask your data in plain English. Get the governed number, every time.**

AskEider puts a semantic layer on your DuckDB database, files (Parquet, CSV), SQLite, Postgres or MySQL, and lets people ask it questions in plain English. The definitions live in ordinary [dbt](https://www.getdbt.com/) + [MetricFlow](https://github.com/dbt-labs/metricflow) YAML that you own. The AI model is your choice.

### For data teams

- **Start in minutes:** `init` profiles the data and drafts the semantic layer. It finds keys, joins, time axes, measures and metrics, and you refine it.
- **Shape it without YAML:** metrics, breakdowns, joins and house rules (fiscal year, default filters, questions to refuse). Each change is checked in plain words, previewed with before and after numbers, and undoable.
- **Let AI suggest, people decide:** a model proposes names, synonyms, metrics and joins from names only, and each suggestion waits for approval.
- **Reuse a setup:** export a project without its data and apply it to next month's export or another company's books. Renamed tables and columns are mapped for you.

### For everyone else

Ask "net revenue by region last quarter" or "which customers owe us the most?" and get:

- a number that comes from your team's definition of revenue, not the model's guess;
- what it counted, how it read your words, and the SQL it ran;
- "Did you mean…?" when a question is a close call, instead of a guess.

Pin answers to dashboards that open instantly, without calling the AI again.

### How we work

- **The AI never sees your database.** It gets a fixed instruction and the question, nothing else: no table or column names, no values, no rows. The SQL runs read-only on your machine.
- **The AI words the question, not the numbers.** Answers come from governed definitions, so the same question gets the same answer.
- **Built to embed.** HTTP API, Python and TypeScript clients, MCP for AI agents, Slack, Teams and a browser build share one engine.
- **An open-source stack:** DuckDB, dbt and MetricFlow, with AskEider itself under Apache 2.0. The AI model is the one part you choose: Claude, OpenAI, DeepSeek, OpenRouter, a local model through Ollama, or no AI at all.

### Links

[Request access](https://github.com/askeider/.github/issues/new?title=Access%20request)

AskEider is in private preview. It works with DuckDB, dbt and MetricFlow, and is not affiliated with the DuckDB Foundation or dbt Labs.
