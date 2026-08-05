# Commercial Presentation AI Skills

Открытый набор Agent Skills для коммерческих и маркетинговых презентаций.

Open Agent Skills for commercial and marketing presentation workflows.

## Skills

- `translate-presentation-faithfully` - перевод существующей презентации без редизайна, изменения фактов, цифр, оборудования и структуры.
- `build-commercial-presentation` - коммерческие предложения, sales decks и техническо-коммерческие презентации.
- `build-marketing-presentation` - маркетинговые, продуктовые, партнерские и launch-презентации.
- `upgrade-presentation` - управляемый апгрейд существующей презентации с пятью уровнями вмешательства.
- `audit-presentation` - независимый аудит смысла, доказательств, дизайна, локализации и целостности файла.

## Compatibility

Навыки используют открытый формат `SKILL.md` и рассчитаны на OpenAI ChatGPT/Codex, Anthropic Claude/Claude Code, Google Gemini CLI/Antigravity managed agents и другие совместимые среды.

Технический движок презентаций зависит от среды. Эти навыки задают коммерческую логику, ограничения и QA, а нативный PPTX/Slides-инструмент среды выполняет чтение и редактирование файла.

## Install

Через skills.sh:

```bash
npx skills add bea4youirk-byte/commercial-presentation-ai-skills --skill translate-presentation-faithfully --global
```

Замените имя навыка на нужное. Для установки в конкретный проект уберите `--global`.

Для managed Gemini agents поместите папки навыков в `.agents/skills/`. В ChatGPT/Codex навыки также можно загрузить или установить через интерфейс Skills. В Claude используйте импорт custom skills или совместимый installer.

## Design principles

- Один навык - одна узнаваемая задача.
- Перевод не смешивается с редизайном.
- Проверенные факты защищены от маркетингового «улучшения».
- Источники, условия, диапазоны и ограничения сохраняются.
- Каждый итоговый слайд проверяется визуально и семантически.
- Подробности загружаются прогрессивно из `references/`.

## Versioning

Текущая базовая версия: **1.0.0**. Совместимость и источники формата зафиксированы в [docs/compatibility.md](docs/compatibility.md), правила обновлений - в [docs/upgrade-policy.md](docs/upgrade-policy.md).

## License

MIT. Навыки написаны с нуля. Репозиторий не включает проприетарный код встроенных PPTX-движков OpenAI, Anthropic или Google.
