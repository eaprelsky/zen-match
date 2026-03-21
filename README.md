# Zen Match

Casual match-3 mobile game. PWA, works offline.

[🇬🇧 English](#english) | [🇷🇺 Русский](#русский)

---

## English

### Play

Open `www/index.html` in browser or install as PWA on your phone.

### Mechanics

**Basic:**
- Swipe to swap adjacent pieces
- Three or more in a row — removed
- Cascades with score multiplier

**Special blocks:**

| Combination | Block | Effect |
|-------------|-------|--------|
| 4 in a row | Line | Clears row or column |
| L or T (5 cells) | Bomb | Explodes 3×3 |
| Large L/T (6+ cells) | Rainbow | Clears all pieces of one color |
| 5 in a line | Rainbow | Same |
| 2×2 square | Plane | Flies to random target, explodes 3×3 |

**Special combos:**

| Combo | Effect |
|-------|--------|
| Line + Line | Cross |
| Line + Bomb | 3-wide cross |
| Bomb + Bomb | 5×5 explosion |
| Plane + Plane | 3 planes |
| Rainbow + piece | All pieces of that color |
| Rainbow + special | All pieces of random color become that special and activate |
| Rainbow + Rainbow | Entire board |

**Ice:**
- Appears from level 2
- Light ice (1 layer) — one hit to thaw
- Heavy ice (2 layers) — two hits needed
- Frozen pieces participate in matches

**Balance:**
- Moves and goal grow by √level
- Difficulty stabilizes, game gets longer

### Tech

- Vanilla JS, Canvas 2D
- PWA with Service Worker for offline
- localStorage for progress
- Auto ru/en localization
- No dependencies, single HTML file

---

## Русский

### Играть

Открыть `www/index.html` в браузере или установить как PWA на телефон.

### Механики

**Базовые:**
- Свайп для обмена соседних фигур
- Три и более в ряд — удаляются
- Каскады с множителем очков

**Специальные блоки:**

| Комбинация | Блок | Эффект |
|------------|------|--------|
| 4 в ряд | Линия | Уничтожает ряд или столбец |
| L или T (5 клеток) | Бомба | Взрывает 3×3 |
| Большой L/T (6+ клеток) | Радуга | Уничтожает все фигуры одного цвета |
| 5 в линию | Радуга | То же |
| 2×2 квадрат | Самолёт | Летит к случайной цели, взрывает 3×3 |

**Комбинации спецблоков:**

| Комбо | Эффект |
|-------|--------|
| Линия + Линия | Крест |
| Линия + Бомба | Крест 3 в ширину |
| Бомба + Бомба | Взрыв 5×5 |
| Самолёт + Самолёт | 3 самолёта |
| Радуга + фигура | Все фигуры этого цвета |
| Радуга + спецблок | Все фигуры случайного цвета становятся этим спецблоком и срабатывают |
| Радуга + Радуга | Всё поле |

**Лёд:**
- Появляется с уровня 2
- Лёгкий лёд (1 слой) — один удар размораживает
- Тяжёлый лёд (2 слоя) — нужно два удара
- Замороженные фигуры участвуют в матчах

**Баланс:**
- Ходы и цель растут по √level
- Сложность стабилизируется, игра становится длиннее

### Технологии

- Vanilla JS, Canvas 2D
- PWA с Service Worker для офлайна
- localStorage для сохранения прогресса
- Автолокализация ru/en
- Без зависимостей, один HTML-файл

---

## Structure / Структура

```
www/
  index.html    — game / игра
  sw.js         — Service Worker
  manifest.json — PWA manifest
  icon-192.png  — icon
  icon-512.png  — icon
```

## History / История

Created in one evening chatting with Claude after Yandex Plus casual game shutdown. 22 iterations from prototype to balanced game.

Создано за один вечер в диалоге с Claude после закрытия казуалки в Яндекс Плюсе. 22 итерации от прототипа до сбалансированной игры.

## License / Лицензия

MIT
