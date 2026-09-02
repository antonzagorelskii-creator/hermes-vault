---
title: Wiki maintenance
created: 2026-09-02
updated: 2026-09-02
type: concept
tags: [automation, workflow, context-management, reliability]
sources: [raw/articles/karpathy-llm-wiki-2026.md]
confidence: medium
---

# Wiki maintenance

## Определение

Wiki maintenance — регулярная агентная работа по обновлению summaries и ссылок, согласованию страниц, регистрации новых источников и выявлению проблем качества. В паттерне [[llm-wiki]] это основная функция LLM, снижающая ручную нагрузку на ведение базы знаний.

## Состав процесса

- при ingestion: обновлять релевантные страницы, каталог и журнал;
- при query: сохранять ценные синтезы как часть накопленной базы;
- при lint: выявлять противоречия, устаревшие утверждения, orphan pages, пробелы и недостающие cross-references;
- сохранять разделение между неизменяемыми raw-источниками и интерпретацией в wiki.

## Связь с RAG

В [[rag]] значительная часть поиска и синтеза повторяется при каждом запросе. Maintenance переносит часть этой работы в момент обработки источника и поддерживает накопленный слой знаний в актуальном состоянии.

## Related

- [[llm-wiki]]
- [[rag]]

## Sources

- [[raw/articles/karpathy-llm-wiki-2026]] — разделы «Architecture», «Operations» и «Why this works».
