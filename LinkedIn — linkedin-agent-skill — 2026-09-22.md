# LinkedIn — linkedin-agent-skill

- **Repository:** [Jakeschincariol/linkedin-agent-skill](https://github.com/Jakeschincariol/linkedin-agent-skill)
- **License:** MIT
- **Target environment:** Claude Code / Claude skills
- **Дата заметки:** 22 сентября 2026

## Что это

📘 Это open-source набор из 11 skills для подготовки LinkedIn-контента и организации работы с личным LinkedIn-аккаунтом.[1]

📘 Репозиторий рассчитан на Claude: skills копируются в `~/.claude/skills/` либо устанавливаются через Claude plugin marketplace; прямой установки в Hermes из README не предусмотрено.[1]

📘 Авторы специально не автоматизируют публикацию в LinkedIn: skills создают copy-ready drafts, а публикацию выполняет пользователь после явного одобрения.[1]

## Состав

1. `li-post` — пост из одной идеи; предлагает hooks и полный draft.[1]
2. `li-comment` — содержательные комментарии к чужим публикациям.[1]
3. `li-reply` — сортировка и подготовка ответов на комментарии под собственным постом.[1]
4. `li-profile` — аудит и переработка профиля по 12-частной rubric на 100 баллов.[1]
5. `li-plan` — недельный content plan и список людей для engagement.[1]
6. `li-human` — локальная очистка текста и heuristic review его стилистических признаков.[1]
7. `li-carousel` — сценарий document/carousel post и PDF-ready content.[1]
8. `li-repurpose` — превращение видео, newsletter или transcript в серию самостоятельных постов.[1]
9. `li-dm` — invitation note, первое сообщение и два follow-ups.[1]
10. `li-inbox` — triage входящих сообщений по категориям.[1]
11. `li-audit` — разбор уже опубликованных постов по engagement rate и reach multiple.[1]

## Что важно уточнить

📘 В `li-post` есть 21 формула hooks; в `li-human` — два Python-скрипта без внешних dependencies и настраиваемый словарь нежелательных штампов.[1]

📘 `li-human` очищает zero-width / format characters, типографику и словарь из 113 стандартных слов и фраз, а затем оценивает текст по пяти **локальным эвристикам**: burstiness, specificity, slop density, fingerprint и voice.[1]

📘 Это не прогон через пять внешних AI-detector services: README прямо указывает, что это не GPTZero, Originality, Copyleaks, Winston или Turnitin и не обещает их результат.[1]

⚠️ Использовать humanizer стоит для ясности, конкретики и соответствия собственному стилю, а не как механизм обхода AI-detection. Для профессионального LinkedIn-контента важнее фактическая точность, disclosure при необходимости и отсутствие выдуманных кейсов, метрик или клиентов.

## Применимость для вашей практики

⚠️ Наиболее ценны четыре части: `li-profile`, `li-post`, `li-repurpose` и `li-human`. Их можно адаптировать под темы valuation, disputes, damages, forensic accounting и AI in consulting: профессиональные наблюдения, разборы methodology, lessons learned и education posts.

⚠️ Перед использованием нужен свой `voice.md`: позиционирование, целевая аудитория, допустимые темы, примеры написанных вами постов, запрещённые claims и правила confidentiality. Без этого автоматические drafts будут generic и могут не соответствовать вашему профессиональному тону.

⚠️ В Hermes skills не установлены: они написаны для Claude и требуют адаптации формата/путей, прежде чем их можно будет безопасно использовать здесь. Их можно портировать выборочно, сохранив human approval перед любой публикацией.

## Sources

[1] https://github.com/Jakeschincariol/linkedin-agent-skill — Jakeschincariol/linkedin-agent-skill — README and source tree
