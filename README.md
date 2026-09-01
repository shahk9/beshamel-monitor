# Бешамел — слайдове за монитора (Младост)

Всяка вечер между **21:00 и 23:40** тук се качват автоматично 4 слайда (1920×1080 PNG)
с менюто на Бешамел за **следващия ден**. Имената на файловете са постоянни — само
съдържанието се обновява.

## Постоянни линкове за сваляне

```
https://raw.githubusercontent.com/shahk9/beshamel-monitor/main/slide-1.png
https://raw.githubusercontent.com/shahk9/beshamel-monitor/main/slide-2.png
https://raw.githubusercontent.com/shahk9/beshamel-monitor/main/slide-3.png
https://raw.githubusercontent.com/shahk9/beshamel-monitor/main/slide-4.png
```

Ред на въртене на монитора: 1 → 2 → 3 → 4 (меню-табло → ястие → меню-табло → ястие).

## Проверка за свежест

`result.json` съдържа:

- `menuDate` — за коя дата е менюто (напр. `"02.09.2026"`)
- `weekday` — ден от седмицата
- `generatedAt` — кога са генерирани слайдовете (ISO 8601, UTC)
- `note` — предупреждение при нещо нестандартно (обикновено `null`)

Препоръка: сваляйте файловете веднъж дневно след 23:45 или проверявайте `generatedAt`
на `https://raw.githubusercontent.com/shahk9/beshamel-monitor/main/result.json`.
