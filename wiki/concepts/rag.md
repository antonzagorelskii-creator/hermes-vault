---
title: Retrieval-Augmented Generation (RAG)
created: 2026-09-02
updated: 2026-09-02
type: concept
tags: [context-management, research, tool-use]
sources: [raw/articles/karpathy-llm-wiki-2026.md]
confidence: medium
---

# Retrieval-Augmented Generation (RAG)

## Роль в источнике

В описании [[llm-wiki]] RAG выступает как контрастная модель: LLM извлекает релевантные фрагменты raw-документов в момент запроса и строит ответ заново. По оценке автора источника, при вопросах, требующих объединить несколько документов, это повторяет поиск и синтез без накопления ранее выведенного знания.

## Соотношение с LLM Wiki

LLM Wiki не отменяет поиск по raw-источникам, но добавляет устойчивый слой с уже подготовленными summaries, entity pages, связями и отмеченными противоречиями. Это переносит часть работы из query time в ingestion и [[wiki-maintenance]].

## Open question

Утверждение о преимуществе LLM Wiki является проектной гипотезой источника; для конкретного домена его следует проверять по качеству ответов, полноте provenance и стоимости поддержки.

## Related

- [[llm-wiki]]
- [[wiki-maintenance]]

## Sources

- [[raw/articles/karpathy-llm-wiki-2026]] — раздел «The core idea».
