# Памятка: иконки в Zensical

## Иконки страниц в навигации

Устанавливаются через **front matter** в начале каждого `.md` файла:

```yaml
---
icon: lucide/rocket
---

# Заголовок страницы
```

Иконка отображается напротив страницы в левом навбаре.

---

## Иконка в названии nav-пункта (внешние ссылки)

Shortcode `:lucide-...:` **не работает** в nav-заголовках `zensical.toml`.
Для внешних ссылок используйте юникодный символ напрямую:

```toml
nav = [
  {"↗ Mediascope API" = "https://example.com"}
]
```

Полезные символы: `↗` (внешняя ссылка), `🔗`, `📡`, `📘`

---

## Логотип сайта

В `zensical.toml`:

```toml
[project.theme.icon]
logo = "lucide/monitor"
```

---

## Поиск иконок

| Набор | Сайт | Shortcode-префикс |
|---|---|---|
| Lucide | https://lucide.dev/ | `lucide/` → `:lucide-name:` |
| Material Design | https://pictogrammers.com/library/mdi/ | `material/` → `:material-name:` |
| FontAwesome | https://fontawesome.com/search?m=free | `fontawesome/brands/name` → `:fontawesome-brands-name:` |
| Octicons | https://octicons.github.com/ | `octicons/name-16` → `:octicons-name-16:` |
| Simple Icons | https://simpleicons.org/ | `simple/` → `:simple-name:` |

---

## Текущие иконки проекта

| Страница | Иконка |
|---|---|
| Введение (`index.md`) | `lucide/rocket` |
| Ночные выходы | `lucide/moon` |
| Двойные выходы | `lucide/layers` |
| Позиционирование | `lucide/target` |
| Окупаемость SuperFix | `lucide/trending-up` |
| Affinity | `lucide/git-merge` |
| Эффективные TRP | `lucide/bar-chart-3` |
| Mediascope API (nav) | `:lucide-external-link:` |
| Логотип сайта | `lucide/monitor` |
