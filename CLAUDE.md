# CLAUDE.md — Margulan Personal Mentor AI · Project DNA

> Этот файл — **единый источник истины** для всех будущих сессий, работающих над этим проектом.
> Прочитай его **полностью** до того, как написать хоть одну строку кода или внести правку.
> Цель: следующий сессионный агент должен продолжить работу так, как будто это делает оригинальный автор системы.

---

## Working language

- **Общение с пользователем:** русский.
- **Код, идентификаторы, имена файлов, коммит-сообщения, имена классов, JS-переменные:** английский.
- **Контент сайта (UI-тексты, заголовки, цитаты):** русский.
- **Брендовое имя «Margulan Personal Mentor AI» и CTA-якоря «Explore the System / Start Reflection / Build Your Mission Map / Ask Personal Mentor AI»:** английский (преднамеренное смешение — executive-кодекс).

---

## Project state (snapshot)

- **Этап:** production-ready single-page site, готовый к деплою на Vercel.
- **Структура:** одна папка, один HTML-файл, без сборки.
- **Файлы в проекте:**
  - [index.html](index.html) — весь сайт (HTML + inline CSS + inline JS), ~1863 строки, ~72.5 КБ
  - [CLAUDE.md](CLAUDE.md) — этот файл
- **Связанный проект:** [../margulan-seisembai-personal-mentor-ai/](../margulan-seisembai-personal-mentor-ai/) — RAG-чат-бот (Python, отдельная кодовая база). Этот сайт — витрина того продукта.
- **Что НЕ существует:** real backend, реальный AI на сайте (только curated-демо), отдельные страницы тем, OG-image, self-hosted fonts, vercel.json, README.md, .gitignore.

---

# 1. PROJECT OVERVIEW

## Что это

**Margulan Personal Mentor AI** — premium-level статическая web-витрина цифровой системы мышления, построенной на философии Маргулана Сейсембая. Это **не блог о Маргулане** и **не landing AI-продукта**. Это **редакционная knowledge platform**, демонстрирующая систему мышления как цельную архитектуру (миссия → энергия → действие → эффективность → внутренняя свобода) и являющаяся точкой входа в Personal Mentor AI (RAG-агент в соседнем проекте).

## Цель

1. **Кратко:** показать философию Маргулана как структурированную систему, а не набор разрозненных идей.
2. **Стратегически:** служить premium-витриной для будущего AI-агента; устанавливать тон и эстетику всей экосистемы продукта.
3. **Тактически:** конвертировать читателя в пользователя AI — через единственную честную CTA «Задать вопрос наставнику».

## Целевая аудитория

- **Первичная:** executives, предприниматели, старшие специалисты, для которых наставничество — инструмент, а не контент. Возраст 30–55. Принимают решения с реальной ценой.
- **Вторичная:** интеллектуальная читающая аудитория, ищущая систему вместо «лайфхаков».
- **НЕ для:** массового потребителя «развития личности», молодёжной self-help аудитории, охотников за быстрыми советами.

## Эмоция, которую сайт должен вызывать

| Должно быть | Не должно быть |
|-------------|----------------|
| Тишина | Шум |
| Глубина | Пышность |
| Сдержанная сила | Громкая мотивация |
| Уважение к читателю | Заискивание |
| Ясность | «Загадочность» |
| Дисциплина | Хаос вкусов |
| Доверие через атрибуцию | Доверие через имена брендов |
| Достоинство | Поза |

Если открыв сайт человек первой реакцией думает «это серьёзно» — попадание. Если думает «красиво» — промах (не туда тянем).

## Позиционирование

- **«Editorial system, not SaaS landing.»**
- **«Cinema for thinking, not infotainment.»**
- **«A book on a screen — with one AI port at the back.»**

## UX-философия

1. **Одна мысль на экран** на мобильном.
2. **Одно primary-действие на секцию.** Никаких выбора-из-четырёх.
3. **Атрибуция важнее эффектности.** Любая идея — со ссылкой на источник или на логику системы.
4. **Show, don't tell.** Пример диалога важнее десяти буллитов «возможностей AI».
5. **Прогрессивное раскрытие.** Каждая секция отвечает на вопрос предыдущей.

## Interaction-философия

- Никаких hover-only состояний (мобильный — primary surface).
- Никаких pop-up, никаких модалок кроме mobile-menu.
- Никаких auto-play видео, никаких трекинговых баннеров.
- Любая навигация ведёт либо в якорь, либо в внешний ресурс. Нет «декоративных» ссылок.
- Главное действие — **«Спросить»** — постоянно доступно: в hero, в каждой ситуации, в footer-навигации, в sticky-bar.

## Эстетическая директива

- **Tasteful executive dark.** Тёмный по умолчанию, тёплый off-white текст, единственный акцент — латунь (brass).
- **Editorial typography first.** Типографика — главный визуал, не иллюстрации, не иконки.
- **Calm motion.** Всё движется как будто думает; ничего не «прыгает».
- **Analog warmth via grain.** Едва различимая зернистая текстура поверх всего убирает «цифровую плоскость».
- **AI-product breath.** Тонкие сигналы AI-присутствия (pulse dots, teal-edge, typewriter) — но не агрессивно.

---

# 2. CORE PROJECT RULES

## 2.1 Foundational rules (НЕ менять без согласования)

Эти 13 правил установил пользователь в первой сессии. Они **константы продукта**, не рекомендации.

1. **Анализ перед изменениями.** Перед любыми правками сначала разбирай существующий код. Никогда не правь вслепую.
2. **Не искажай смысл исходного материала.** Цитаты Маргулана — точно. Перефразировки — с сохранением смыслового ядра.
3. **Не выдумывай.** Идеи, формулировки, цитаты, концепции, которых нет в материале, — запрещены. Сейчас источник — список 10 идей, переданных пользователем (см. секцию 7.6 «Канон контента»). Когда появятся транскрипты — расширим.
4. **План перед кодом.** Перед каждой итерацией — короткий план (3–7 пунктов).
5. **Self-review после каждого этапа.** По завершении этапа сам проверь соответствие правилам.
6. **Mobile-first.** Все макеты сначала под мобильный, потом расширение.
7. **Premium knowledge platform / executive personal mentor AI.** Эстетика executive-инструмента, не блога.
8. **Без бэкенда.** Только статика. Никаких API-роутов. Внешние API — только из браузера, и только если без них нельзя (на данный момент: только Google Fonts CSS-CDN).
9. **Без тяжёлых либ без необходимости.** Никаких Three.js, GSAP, Framer Motion, Tailwind, Bootstrap, jQuery. Vanilla только.
10. **Production-ready код.** Семантический HTML, a11y, нет `console.log`/`TODO`/закомментированного кода.
11. **Глубокие, ясные, уважительные тексты.** Никаких маркетинговых клише («измени жизнь», «секреты успеха», «trusted by 10,000+»).
12. **Visual style:** премиальный, философский, интеллектуальный, современный.
13. **Отчёт после этапа:** что сделано, что улучшено, как проверить.

## 2.2 Continuity rules (введены этим документом)

14. **Maintain continuity over novelty.** Если делаешь новое — делай как существующее. Никакого «давайте теперь попробуем другой подход».
15. **Prefer extending existing systems over introducing new paradigms.** Если задача похожа на уже решённую — расширяй, не создавай вторую систему.
16. **Avoid unnecessary redesigns.** Любое визуальное изменение требует обоснования через продуктовую цель, а не через «свежий взгляд».
17. **Preserve established interaction patterns.** Hover-стрелки, reveal-on-scroll, typewriter, pulse-dot, sticky-bar — это **product language**, не декор.
18. **Reuse existing abstractions whenever possible.** Если нужен компонент похожий на `.cluster` — используй `.cluster`, не создавай `.section-card`.

## 2.3 Visual identity preservation rules

Эти элементы **визуально определяют продукт**. Менять их можно только с явным согласованием:

- **Палитра:** Ink (#0E0E0F) + Paper (#F2EFEA) + Brass (#C8A368) + Teal-edge (rgba 120,180,195,*).
- **Шрифты:** Fraunces + Inter. Никакого третьего семейства. Никаких системных fallback-как-default.
- **Грейн-overlay** на body — это часть identity, не «эффект».
- **Римские цифры I–VIII** в meta-линиях секций — chapter-структура.
- **«Глава 0 · Введение» eyebrow** в hero.
- **Pulse-точка возле «О.» в диалоге.**
- **Эпистолярный формат AI-блока** (В. / О., не bubble-chat).
- **Editorial-типографика** клусеров (нет card-grid эстетики).

## 2.4 Architecture preservation rules

- **Single-file architecture.** Не разбивать на модули без явного перехода на сборку (Astro/Vite). Если переход — только после согласования.
- **Inline CSS/JS.** Не выносить во внешние файлы пока сайт остаётся single-file.
- **Vanilla only.** Не вводить React/Vue/Svelte без переучреждения проекта.
- **No build step.** Сайт открывается двойным кликом. Это часть продукта.
- **Static hosting.** Vercel/Cloudflare Pages/Netlify — да. Серверный рендер — нет.

## 2.5 UX consistency rules

- **Якорная навигация.** Все внутренние ссылки — якоря к секциям. Не открывать новые «страницы» (их нет).
- **One primary CTA на секцию.** Если их две — пересмотри иерархию.
- **Hover-стрелки** (`→`) появляются с translateX-сдвигом и brass-цветом — везде одинаково.
- **Reveal-on-scroll** через `[data-reveal]` атрибут с opacity + translateY 16px. Никаких rotate, scale, blur.
- **Sticky bottom-bar** только на мобильном (`< 900px`), исчезает при scroll-down, появляется при scroll-up.
- **Mobile menu** — full-screen overlay с staggered reveal.

---

# 3. DESIGN SYSTEM

Все токены живут в `:root` в [index.html](index.html). При любых изменениях — **трогаем токены, не hex-значения в местах использования**.

## 3.1 Colors

### Полная палитра (CSS custom properties)

| Токен | HEX/RGBA | Семантика |
|-------|----------|-----------|
| `--color-ink` | `#0E0E0F` | Главный фон, тёплый near-black |
| `--color-ink-2` | `#111114` | Финал градиента в hero (чуть холоднее) |
| `--color-ink-alt` | `#0B0B0D` | Фон альтернативных секций (чуть темнее) |
| `--color-surface` | `#16161A` | Резервный для глубоких поверхностей (сейчас почти не используется) |
| `--color-stroke` | `#2A2A2C` | Видимые разделители, обводки кнопок |
| `--color-stroke-2` | `rgba(255,255,255,0.07)` | Тонкие разделители (списки, между секциями) |
| `--color-paper` | `#F2EFEA` | Основной текст, тёплый off-white |
| `--color-mute` | `#A8A29A` | Вторичный текст (`.lead`, описания) |
| `--color-soft` | `#7E7770` | Третичный текст (cluster count, ai-demo hint) |
| `--color-quiet` | `#5A574F` | Резервный (контраст ниже AA — использовать осторожно) |
| `--color-brass` | `#C8A368` | **Единственный акцент** — meta-метки, номера, CTA-underlines, focus-кольца |
| `--color-brass-mute` | `rgba(200,163,104,0.6)` | Brass для второстепенных элементов (chapter index, scroll progress fade) |
| `--color-ai-glow` | `rgba(120,180,195,0.16)` | Teal radial-glow в Mentor секции |
| `--color-ai-edge` | `rgba(120,180,195,0.32)` | Teal обводки и edge-линии в AI-блоке |
| `--color-ai-pulse` | `rgba(200,163,104,0.85)` | Pulse-точка у «О.» и в sticky-bar |

### Семантические алиасы

```
--bg          → ink
--text        → paper
--text-muted  → mute
--text-soft   → soft
--text-quiet  → quiet
--accent      → brass
```

### Правила использования

- **Brass — экономно.** Допустимые места: meta-метки, номера принципов/опор/шагов, focus-кольца, CTA-underlines, attribution-выделения, AI-pulse, scroll-progress, hover-стрелки. **Если на странице brass появляется > 12 раз без видимой иерархии — это перебор.**
- **Teal — только в AI-зоне.** Mentor section glow + ai-edge + ai-pulse + Demo-badge border. Нигде больше teal не должен появиться.
- **Никаких градиентов кроме**: hero вертикаль (ink→ink-2), hero radial-overlays (brass + teal sub-1%), section-mark (transparent → brass-mute → transparent), scroll-progress (brass → brass-mute), dialogue top-edge (transparent → ai-edge → transparent).
- **Никаких ярких цветов.** Всё, что не из палитры — запрещено. Если кажется, что нужен «зелёный success» или «красный error» — пересмотри необходимость.
- **Контраст:** body Paper-on-Ink ~14:1 (AAA). Mute-on-Ink ~7.5:1 (AA). Soft-on-Ink ~5:1 (AA для большого текста). **Quiet НЕ использовать для текста — только для marks/lines.**

## 3.2 Typography

### Шрифтовая пара

- **Display:** **Fraunces** (variable serif). Используется для всех заголовков, цитат, hero, italic-выделений, theme-name. Variable axes: `opsz` 9–144, `wght` 400–500 normal, `wght` 380–460 italic.
- **Body:** **Inter** (variable sans). Используется для UI-текста, body, meta, CTAs, footer, описаний. Weights: 400, 500.
- **Третьего семейства нет.** Если возникает соблазн добавить mono для технических элементов — сначала спроси «зачем». Сейчас mono не используется.

### Подключение

Через Google Fonts CDN (subset под фактически используемые axes — НЕ менять без причины, иначе вернётся 300+ КБ):

```html
<link href="https://fonts.googleapis.com/css2?family=Fraunces:ital,opsz,wght@0,9..144,400..500;1,9..144,380..460&family=Inter:wght@400;500&display=swap" rel="stylesheet">
```

### Type scale (fluid через clamp)

| Токен | clamp() | Min/Max px | Использование |
|-------|---------|------------|---------------|
| `--fs-display` | `clamp(2.625rem, 8.5vw, 5.75rem)` | 42 → 92 | Hero `<h1>` |
| `--fs-h1` | `clamp(2rem, 5vw, 3.5rem)` | 32 → 56 | Резерв (сейчас не используется напрямую) |
| `--fs-h2` | `clamp(1.625rem, 3.5vw, 2.5rem)` | 26 → 40 | `.section-title` (h2) |
| `--fs-h3` | `clamp(1.25rem, 2vw, 1.5rem)` | 20 → 24 | h3 в Inter (footer, шаги) |
| `--fs-lead` | `clamp(1.0625rem, 1.6vw, 1.3125rem)` | 17 → 21 | `.lead` |
| `--fs-body` | `clamp(1rem, 1.2vw, 1.125rem)` | 16 → 18 | body |
| `--fs-meta` | `0.8125rem` (фикс) | 13 | Meta-метки, footer-h4, nav |

### Веса и font-variation

- Fraunces: `wght 400` базовый, `420` в hero/CTA, `440–460` в принципах/path-узлах, `380` в italic для use-cases. Изменения через `font-variation-settings: 'wght' X, 'opsz' Y;`.
- Inter: 400 для body, 500 для UI/meta.
- **Никаких bold (700+).** Editorial-сила — в воздухе и italic, не в жирности.

### Line-height

| Контекст | Значение |
|----------|---------|
| Display (hero h1) | 1.02–1.05 |
| h2/h3 | 1.2 |
| Body | 1.6 |
| Lead | 1.55 |
| Quote/italic | 1.4 |

### Letter-spacing

- Display: `-0.02em` (`--track-tight`)
- Meta: `+0.14em` (`--track-meta`) uppercase
- Body: 0
- Brand mark: `+0.06em`

### Font features (micro-typography)

```
--feat-display: 'liga' on, 'kern' on, 'salt' on, 'ss01' on;
--feat-body:    'kern' on, 'liga' on, 'cv11' on, 'ss01' on;
```

- `font-variant-numeric: lining-nums proportional-nums` на body (общее).
- `lining-nums tabular-nums` на номерах (01, 02, и римские цифры).
- `hanging-punctuation: first last allow-end` на body — для editorial-кавычек.

### Italic

- Используется ОСМЫСЛЕННО, не декоративно:
  - Hero accent line («Система мышления.»)
  - Use cases («Я выгорел.» и т.д.) — голос пользователя
  - AI question (`<p>` в `.dialogue__q`)
  - Disclaimer-strip (тон автора)
  - Chapter index в `.meta__index` (мелкая римская цифра)
- `<em>` использовать только для эмфазы (семантика). Декоративный italic — через `<span>` + класс.

## 3.3 Spacing System

### База: 8px grid

```
--space-2:  0.5rem  (8 px)
--space-3:  1rem    (16 px)
--space-4:  1.5rem  (24 px)
--space-5:  2rem    (32 px)
--space-6:  3rem    (48 px)
--space-7:  4rem    (64 px)
--space-8:  6rem    (96 px)
--space-9:  8rem    (128 px)
--space-10: 12rem   (192 px)
```

`--space-1` (4px) удалён за неиспользуемостью. Если потребуется 4px — пересмотри композицию.

### Секционный ритм

```
--section-py:    clamp(96px, 12vw, 192px)   /* вертикальный отступ секции */
--container-px:  clamp(24px, 5vw, 32px)     /* горизонтальный отступ контейнера */
--container-max: 1280px
--prose-max:     66ch
```

### Правила вертикального ритма

- Между секциями: `--section-py` (всегда через токен).
- Между `section-head` и контентом: `--space-7` (64px).
- Между meta и заголовком: `--space-3` (16px).
- Между заголовком и lead: `--space-4` (24px).
- Между блоками внутри секции (карточки/строки): `--space-5`–`--space-6`.
- Между micro-элементами (мета и заголовок карточки): `--space-2`.

### Правила горизонтального ритма

- Контейнер всегда `var(--container-px)` слева/справа.
- Содержимое внутри контейнера — макс `--container-max` (1280px).
- Длинные тексты (body) — макс `--prose-max` (66ch).

## 3.4 Component Style Language

### Borders

- **Толщина:** 1px только. 2px только для focus-outline.
- **Стиль:** solid по умолчанию. **dashed** только в `.ai-demo` (явный сигнал «прототип»).
- **Цвет:** `--color-stroke` (видимые), `--color-stroke-2` (еле различимые). Brass-borders только в hover-состояниях и в принципах.
- **Border-radius:** **0 везде.** Editorial эстетика. Исключения — кружочки `.node::before` (border-radius: 50%) и pulse-dots.

### Shadows

- **Только один значимый shadow** в проекте: на `.dialogue` карточке `0 30px 60px -30px rgba(0,0,0,0.45)` + inset highlight.
- **Никаких drop-shadow на кнопках, карточках, иконках.** Editorial flat.
- **`box-shadow` для outer-glow:** только на `.node.is-visible::before` (4px brass aura).

### Transparency и blur

- **`backdrop-filter: blur(...)`** используется на 3 элементах: `.nav`, `.dialogue`, `.sticky-bar`. **Не добавлять на 4-й** — performance бьёт по mobile.
- Полупрозрачные фоны: только `rgba(14,14,15,0.78–0.88)` для navigation surfaces, `rgba(255,255,255,0.012–0.025)` для AI-card subtle gradient.

### Hover behavior

| Элемент | Hover-эффект |
|---------|--------------|
| Inline-link | color → brass, underline остаётся |
| Pillar/Cluster | border → stroke (subtle) |
| Theme row | none (намеренно — non-interactive) |
| Case-link | padding-left +12px, brass-arrow появляется |
| Principle | none |
| CTA item | padding-left +8px, border → brass, arrow translateX +8px brass |
| Primary button | border → brass, brass background-tint, top-edge accent появляется, bottom underline появляется |
| Secondary button | color → brass, arrow translateX +6px |
| Footer link | color mute → paper |
| Nav menu link | color mute → paper, underline scaleX 0→1 |

**Правило:** все hover работают только под `@media (hover: hover) and (pointer: fine)`. На touch — нет hover-эффектов.

### Transitions

```
--ease-out:     cubic-bezier(0.22, 1, 0.36, 1)
--ease-content: cubic-bezier(0.16, 1, 0.3, 1)
--dur-fast:     280 ms
--dur-base:     420 ms
--dur-slow:     640 ms
```

- **Никогда быстрее 200ms** — теряется ощущение преднамеренности.
- **Никогда медленнее 1s** — теряется отзывчивость.
- **Никаких spring/bounce/elastic.** Только ease-out семейство.

### Animation philosophy

- **«Всё движется так, будто думает.»**
- Keyframe-анимации, существующие в проекте:
  - `breathe` — variable wght в hero h1 (9s loop)
  - `cuePulse` — opacity hero scroll-cue (3s loop)
  - `cursorBlink` — typewriter курсор (1s step-end)
  - `aiPulse` — pulse-точка возле «О.» и в sticky-bar (2.4s ease-in-out)
- **Интерсекшн-анимации** (через JS):
  - `[data-reveal]` — fade-in + translateY 16px → 0, 720ms ease-content
  - `[data-node]` — sequential reveal с stagger 150ms
  - typewriter — char-by-char, 22ms/char
- **`prefers-reduced-motion: reduce`** — обязательно отключает все keyframes, reveal становится instant, typewriter моментальный.

---

# 4. UI/UX PHILOSOPHY

## 4.1 Как должны ощущаться интерфейсы

- **Тихие.** Никаких ярких подсветок при загрузке, никаких «hello, look at this».
- **Дисциплинированные.** Каждый элемент имеет место и причину.
- **Дышащие.** Между элементами — воздух, не теснота. На мобильном тоже.
- **Уважительные.** Не пытаются угадать, что хочет пользователь. Дают ему пространство.

## 4.2 Density

- **Один смысловой блок на скролл-экран** на мобильном, два-три на десктопе.
- **Длина строки body** не превышает 66ch (через `--prose-max` или явный `max-width`).
- **Пустота — это контент.** Большие отступы между секциями (96–192px) — фича, не баг.

## 4.3 Сложность → ясность

- **Перечисления нумерованы** (01, 02, ...) — это даёт ощущение системы, не списка.
- **Кластеры** (Knowledge Map) группируют 23 темы в 6 смысловых блоков.
- **Roman numerals** (I–VIII) на section-meta задают порядок чтения «как в книге».
- **Шесть шагов «Как работает»** объясняют продукт через процесс, не через features.

## 4.4 Управление вниманием

- **One primary action на экран.** Sticky-bar мобильная — единственное постоянное «Спросить».
- **Brass — навигатор внимания.** Глаз идёт по brass-меткам: meta → номер → линия → стрелка.
- **Reveal-on-scroll** мягко привлекает внимание к новому контенту, не дёргает.
- **AI pulse-точка** — единственный «активный» элемент на странице. Сигнал: «здесь живой AI».

## 4.5 Animation behavior

- **Reveal:** мягкое opacity + translateY. Никогда не должно «вылетать сбоку», «крутиться», «масштабироваться».
- **Typewriter** для AI-ответа — единственный сильный motion-момент. Уважает reduced-motion.
- **Pulse-dots** — 2.4s loop, scale 1 → 1.4 + opacity 0.4 → 1. Тонко.
- **Hero breathing** — variable wght oscillates ±50 за 9 секунд. Eye почти не замечает, но чувство «живой» сохраняется.

## 4.6 Responsive scaling

- **Layout** скейлится через `clamp()` для типографики и spacing — никаких jump-cuts на breakpoints.
- **Структура** меняется на breakpoints: 720px (двухколоночные сетки начинают), 900px (десктоп: десктоп-меню, sticky-bar исчезает), 1100px (Knowledge Map в 3 колонки).
- **Mobile menu** — fullscreen overlay с staggered reveal.
- **Sticky bottom-bar** — только мобильный.

## 4.7 Perceived qualities

| Качество | Как достигается |
|----------|-----------------|
| **Premium** | Сдержанность палитры, voice-серифа, дисциплина в брасс-точках, аналоговый грейн |
| **Intelligent** | Editorial chapter-numbers, цитата с атрибуцией, AI с честным dis-claimer, нелинейная мысль (миссия → энергия → действие) |
| **Modern (2026)** | Variable fonts, fluid typography, font-feature-settings, `dvh`, `inert`, `:focus-visible`, `text-wrap: balance/pretty` |
| **Fast** | One file, inline CSS/JS, subset fonts, no JS frameworks, `requestAnimationFrame` для scroll handlers, `will-change` управляется |
| **Trustworthy** | Видимый дисклеймер о симуляции, атрибуция логики AI, четкая источниковая ссылка на проект Маргулана |

---

# 5. FRONTEND ARCHITECTURE

## 5.1 Topology

```
margulan-knowledge-platform/
├── CLAUDE.md       ← этот файл
└── index.html      ← весь сайт (HTML + <style> + <script>)
```

**Single-file by design.** Это не «временное» — это сознательный выбор:
- Open by double-click.
- Deploy by drag-drop.
- Edit без сборки.
- Read без прыжков по 50 файлам.
- Transparent: автор сайта может прочитать его за 20 минут целиком.

При переходе на масштабную фазу (несколько страниц, сложные компоненты) — переезд на Astro. До тех пор — один файл.

## 5.2 HTML structure (top-down)

```
<!DOCTYPE html>
<html lang="ru">
  <head>
    [meta, title, OG, favicon (inline SVG), preconnect, fonts, <style>]
  </head>
  <body>
    <a class="skip-link">                    ← a11y skip
    <div class="scroll-progress">            ← top brass progress bar
    <header class="nav">                     ← sticky top nav (60px)
    <div class="mobile-menu" role="dialog">  ← fullscreen overlay
    <main id="main" tabindex="-1">
      <section class="hero">                 ← chapter 0
      <section class="philosophy">           ← I — пять опор
      <span class="section-mark">            ← chapter break
      <section class="knowledge section--alt"> ← II — карта знаний
      <section class="how">                  ← III — как работает
      <span class="section-mark">
      <section class="cases section--alt">   ← IV — реальные ситуации
      <section class="principles">           ← V — восемь аксиом
      <span class="section-mark">
      <section class="mentor">               ← VI — AI mentor preview
      <section class="path">                 ← VII — путь
      <span class="section-mark">
      <section class="cta-final section--alt"> ← VIII — четыре входа
      <p class="disclaimer-strip">           ← italic disclaimer
    </main>
    <footer class="footer">                  ← 4 колонки
    <nav class="sticky-bar">                 ← mobile-only bottom CTA
    <script>                                 ← IIFE
  </body>
</html>
```

## 5.3 CSS organization

CSS разделён на пронумерованные блоки **в порядке cascade-логики** (база → токены → утилиты → компоненты → секции → анимации):

1. `TOKENS` — все CSS custom properties в `:root`
2. `RESET` — современный мини-reset + `body::before` грейн
3. `UTILITIES` — `.container`, `.sr-only`, `.skip-link`, `:focus-visible`, `.scroll-progress`
4. `TYPOGRAPHY` — h1–h4, p, `.meta`, `.lead`, `.section-title`, `.section-mark`
5. `BUTTONS` — `.btn`, `.btn--primary`, `.btn--secondary`
6. `NAV` — header.nav + .nav__brand + .nav__menu + .burger
7. `MOBILE MENU` — `.mobile-menu` + staggered links
8. `SECTION BASE` — общий `section` styles, `.section-head`, `.section--alt`
9. **Section-specific** (по одному блоку):
   - HERO
   - PHILOSOPHY CORE
   - KNOWLEDGE MAP
   - HOW IT WORKS
   - USE CASES
   - PRINCIPLES
   - AI MENTOR PREVIEW (включая `.dialogue` и `.ai-demo`)
   - TRANSFORMATION PATH
   - CTA FINAL
   - DISCLAIMER STRIP
   - FOOTER
   - STICKY ASK BAR
10. `REVEAL ANIMATIONS` — `[data-reveal]`
11. `REDUCED MOTION` — глобальный override

**Правило:** новые компоненты добавляются **в конец секционного блока, к которому они относятся**, или выделяются в новый блок с пронумерованным комментарием-разделителем.

## 5.4 JS architecture

JS — единственный IIFE:

```js
(function () {
  'use strict';
  const reduceMotion = window.matchMedia('(prefers-reduced-motion: reduce)').matches;
  /* ... */
})();
```

### Modules (логические блоки внутри IIFE, в порядке)

1. **Constants pickup** — DOM-ссылки и state (lastY, ticking, isDesktop, docHeight)
2. **`onScroll()`** — nav border, sticky-bar visibility, scroll-progress (rAF-throttled)
3. **`onResize()`** — пересчёт isDesktop, docHeight, сброс sticky-bar
4. **Mobile menu** — `setSiblingsInert`, `openMenu`, `closeMenu`, focus-trap, Esc-handler
5. **Reveal observer** — IntersectionObserver, добавляет `.is-visible`, потом `.is-revealed` для cleanup
6. **Path nodes observer** — отдельный IO, sequential reveal с stagger
7. **AI typewriter** — IO triggers `startTypewriter()`, char-by-char через `setTimeout`

### JS-конвенции

- Vanilla только. Никакого jQuery, axios, lodash.
- `const` для всего; `let` только когда мутируется.
- Стрелочные функции для callback'ов; named functions для loaders/handlers.
- Нет async/await (нет async-операций).
- Нет try/catch (нет вещей, которые могут бросить ожидаемо).
- Нет error logging (нет места для логирования на статике).

## 5.5 State management

- **Нет state-management библиотеки.** Состояние — DOM-классы и атрибуты:
  - `.is-open`, `.is-scrolled`, `.is-hidden`, `.is-visible`, `.is-revealed`, `.is-typing`, `.is-shown`, `.is-done`, `.menu-open`
  - `aria-expanded`, `aria-hidden`, `aria-disabled`, `inert`
- Local state в JS — простые переменные (`lastY`, `ticking`, `lastFocused`, `started`).
- Никакого `window.state`, никакого custom EventBus.

## 5.6 Rendering strategy

- **Static rendering.** Файл = output. Нет server, нет hydration, нет SPA-routing.
- **Progressive enhancement:** контент полностью читается без JS. JS добавляет анимации, focus-trap, typewriter — улучшения, не блокеры.
- **CSS-driven layout.** Никакой JS не правит layout. JS только переключает классы.

## 5.7 Responsiveness architecture

- **Mobile-first.** Базовые стили = мобильный. Media queries только увеличивают (min-width).
- **Breakpoints:**
  - `720px` — мелкие сетки (pillars 2-кол на промежутке 720–899px, clusters 2-кол)
  - `900px` — десктопный nav, sticky-bar исчезает, pillars 5-кол, steps 2-кол, principles asymmetric grid, timeline горизонтальный
  - `1100px` — clusters 3-кол
- **Container queries** не используются (пока нет необходимости).

## 5.8 Why this architecture exists

- **Single file** — потому что сайт мал (≤ 100KB), деплой должен быть instant, чтение для нового контрибьютора — без cognitive overhead.
- **No framework** — потому что framework решает state/data-flow/SPA проблемы, которых у нас нет. Vanilla даёт полный контроль над байтами.
- **No build step** — потому что product = file. Сборка добавляет шаг, ничего не упрощая.
- **Inline styles/scripts** — потому что один HTTP-запрос быстрее трёх, и потому что параллельный edit upgrade проще атомарного.
- **CSS custom properties** — потому что они дают design tokens без препроцессоров.
- **IntersectionObserver** — потому что это нативный, performant, и не требует scroll-libraries.

---

# 6. CODING STANDARDS

## 6.1 Naming conventions

### CSS

**BEM-light, без модификаторов через `--`.** Обычно: `.block__element`, иногда `.block--variant`.

| Pattern | Пример |
|---------|--------|
| Block | `.pillar`, `.cluster`, `.dialogue`, `.cta-item`, `.step` |
| Element | `.pillar__num`, `.cluster__head`, `.dialogue__label`, `.cta-item__title`, `.step__num` |
| Variant | `.btn--primary`, `.btn--secondary`, `.section--alt` |
| State | `.is-open`, `.is-scrolled`, `.is-visible`, `.is-typing` |
| Data attr | `[data-reveal]`, `[data-node]`, `[data-text]` (data-text — для typewriter content) |

### JS

- camelCase для переменных и функций (`isDesktop`, `setSiblingsInert`, `startTypewriter`).
- Constants — обычные const camelCase, не SCREAMING (`focusableSel`, не `FOCUSABLE_SEL`).
- DOM-references по id: `nav`, `burger`, `menu`, `aiAnswer`, `progress`.

### HTML

- IDs только когда нужны (anchor-targets, JS-hooks, aria-references). Не для стилизации.
- `id` в kebab-case или camelCase — оба используются (по контексту: anchor-targets — kebab, JS hooks — camel). Это исторически устаканилось, не менять.

### Files

- Сейчас один файл: `index.html`. При расширении — `kebab-case.html`.

## 6.2 Component creation rules

**Прежде чем создавать новый компонент:**

1. Посмотри в [index.html](index.html), есть ли похожий.
2. Если похожий — расширь его (`.cluster--variant`, новый элемент `.cluster__footer`), не создавай `.cluster-v2`.
3. Если действительно новый — добавь в подходящий пронумерованный CSS-блок (Section base / Components / etc.).
4. Используй существующие токены. Не вводи новые `--color-*` без обсуждения.
5. Документируй в этом CLAUDE.md, если паттерн повторяется.

## 6.3 File organization rules

- Один файл, пока возможно.
- Если файл превысит 3000 строк — обсудить переезд на Astro (но не Vite-only — Astro даёт лучшее DX для статики с компонентами).
- Никогда не дробить раньше необходимости.

## 6.4 HTML conventions

- **Semantic HTML** обязательно. `<header>`, `<main>`, `<section>`, `<article>`, `<nav>`, `<footer>`, `<aside>` — по назначению, не для стилизации.
- **Каждая `<section>` имеет `aria-labelledby`** к своему `<h2>` (или `<h1>` для hero).
- **Один `<h1>` на страницу** — всегда в hero.
- **Иерархия заголовков** не пропускает уровни внутри одной landmark зоны.
- **`role="list"`** добавлять на любой `<ul>`/`<ol>` со снятым `list-style` (Safari/VoiceOver fix).
- **`tabindex="-1"`** только на `<main>` (для skip-link target). Никогда не использовать `tabindex="0"+` для не-интерактивных элементов.
- **Focus-trap** в overlay (mobile-menu) — обязательно.
- **`inert`** на siblings overlay — обязательно при открытии.

## 6.5 CSS conventions

- **CSS custom properties** для всего, что повторяется или может меняться.
- **`clamp()`** для всех fluid размеров (типографика, секционные отступы, container padding).
- **Никаких `!important`** кроме как в `@media (prefers-reduced-motion: reduce)` блоке.
- **`@media (hover: hover)`** обязательно для hover-эффектов.
- **`@supports`** не используется (target — современные браузеры, fallback — деградация без поломки).
- **Никакого `position: absolute` без `position: relative` на родителе.**
- **`transform`** для анимаций (GPU-accelerated). Не анимировать `width/height/top/left`.
- **`transition` — только нужные свойства**, не `transition: all`.
- **Никаких CSS-фреймворков** (Tailwind, Bootstrap, Bulma — нет).
- **Никаких CSS-in-JS.**

## 6.6 JS conventions

- **`'use strict'`** обязательно.
- **IIFE-wrapper** обязателен для всего файлового JS.
- **`const` everywhere**, `let` только если мутируется.
- **No globals.** Всё внутри IIFE.
- **`{ passive: true }`** для всех scroll/touch listeners.
- **`requestAnimationFrame`** для scroll handlers.
- **`IntersectionObserver`** для появлений на скролле (НЕ scroll listener).
- **Reduced-motion check** на старте: `window.matchMedia('(prefers-reduced-motion: reduce)').matches`.
- **No async/await, no Promises** (нет async-операций).
- **No `console.*`, no `debugger`, no `alert`** в production коде.

## 6.7 Comments policy

- **По умолчанию — без комментариев.**
- **Sectional dividers** в CSS — допустимы (помогают навигации в большом single-file):
  ```
  /* =========================================================
     SECTION NAME
     ========================================================= */
  ```
- **Inline JS-комментарии** — только для не-очевидных решений (например, «rAF для performance»).
- **Никаких TODO без даты и автора.** Лучше — issue в трекере.
- **Никакого закомментированного кода.** Удалять.

## 6.8 Abstraction rules

- **Prefer consistency over cleverness.** Если есть простой способ — используй простой.
- **Avoid overengineering.** Не создавай factory для одного компонента.
- **Keep components composable.** Каждый блок CSS — independently usable.
- **Preserve readability.** Чёткие имена > умные сокращения.
- **Avoid introducing conflicting paradigms.** Если в проекте всё через DOM-классы — не вводи Web Components.

---

# 7. REUSABLE PATTERNS

## 7.1 Section pattern

Каждая section следует одному template'у:

```html
<section class="[name] [section--alt?]" id="[anchor]" aria-labelledby="[id]Title">
  <div class="container">
    <div class="section-head" data-reveal>
      <p class="meta"><span class="meta__index">[ROMAN]</span>[ВАРИАНТ]</p>
      <h2 class="section-title" id="[name]Title">[ЗАГОЛОВОК]</h2>
      <p class="lead">[1–2 предложения lead-абзаца]</p>
    </div>
    [content]
  </div>
</section>
```

**Правила:**
- Roman numeral (I–VIII) в `.meta__index` обязателен для контентных секций.
- Hero — единственное исключение: использует `.hero__chapter` («Глава 0 · Введение»).
- `data-reveal` на `.section-head` — fade-in при появлении.
- `.section--alt` применяется на чередующиеся секции для тональной альтернации (knowledge, cases, cta-final).

## 7.2 Numbered item pattern (pillar / step / principle / cluster cluster)

```html
<article class="[block]" data-reveal style="--reveal-delay: [N]ms">
  <span class="[block]__num">[01]</span>
  <h3>[Название]</h3>
  <p>[Описание]</p>
</article>
```

**Stagger delay:** 80ms между соседними элементами (`--reveal-delay: 0, 80, 160, 240, 320, 400ms`).

## 7.3 Editorial expandable list (Knowledge Map clusters)

Без card-styling. Header с подчёркивающей линией, list с тонкими разделителями. Каждая тема — раскрывающийся `<details>` с реальным контентом из транскриптов.

```html
<article class="cluster" data-reveal>
  <header class="cluster__head">
    <p class="meta">[Название кластера]</p>
    <span class="cluster__count">[N тем]</span>
  </header>
  <p class="cluster__lead">[1-2 строки о смысле кластера]</p>
  <ul role="list">
    <li class="theme">
      <details class="theme__expand">
        <summary class="theme__head">
          <span class="theme__title">
            <span class="theme__name">[Тема]</span>
            <span class="theme__desc">[Краткое описание]</span>
          </span>
          <span class="theme__chevron" aria-hidden="true">+</span>
        </summary>
        <div class="theme__body">
          <p>[Параграф-разворот, парафраз из транскриптов или платформенный copy]</p>
          <blockquote class="theme__quote">
            «[Прямая цитата Маргулана]»
            <cite>Маргулан Сейсембай · [Название выступления]</cite>
          </blockquote>
          <a class="theme__cta" href="#mentor">Спросить про эту тему →</a>
        </div>
      </details>
    </li>
    [...]
  </ul>
</article>
```

**Правила раскрытия:**
- `<details>`/`<summary>` — нативный disclosure, без JS.
- `+` шеврон поворачивается на 45° при `[open]`, превращаясь в `×`-знак.
- Body имеет slide-fade-in animation (`themeSlide`), гарантировано отключается при reduced-motion.
- При раскрытии — параграф (обязательно), цитата (опционально, только если есть в транскриптах), CTA `<a href="#mentor">` (обязательно).
- Темы без прямой цитаты Маргулана получают только параграф + CTA. Цитату не выдумывать.

**Каждая тема обязана быть кликабельной** и раскрывать реальный контент. Visual-cue (chevron) и semantic (`<details>`) синхронизированы — affordance соответствует поведению.

## 7.4 Interactive entry pattern (Use Cases, CTA Final)

Когда строка должна быть кликабельной:

```html
<li>
  <a class="case-link" href="#mentor" data-reveal>
    <span class="case__text">[Текст]</span>
    <span class="case__arrow" aria-hidden="true">→</span>
  </a>
</li>
```

**Hover:** padding-left +12px, brass-arrow появляется (opacity 0→1, translateX -6px → 0).

## 7.5 Section break pattern

Между визуально связанными парами секций — `.section-mark`:

```html
<span class="section-mark" aria-hidden="true"></span>
```

1px × 32px вертикальный gradient (transparent → brass-mute → transparent), opacity 0.5. Используется между Philosophy↔Knowledge, How↔Cases, Principles↔Mentor, Path↔CTA Final. **Не использовать между всеми парами** — теряется смысл chapter-break.

## 7.6 Канон контента

**Канонический источник** — объединённый файл транскриптов выступлений Маргулана:

```
C:\Users\ildmu\OneDrive\Desktop\Margulan Seisembay\all_transcripts_merged.txt
```

Это **24 смысловых группы** транскриптов (миссия, счастье, эффективность, энергия, привычки, целеполагание, страхи, обучение, адаптивность, бизнес, лидерство, успех, возможности, внутренняя свобода, дети, деньги, инвестиции, переговоры, отношения, религия/наука/философия, рефлексия, биография, экономика/технологии, фрагменты на казахском). Каждый фрагмент атрибутирован к конкретному выступлению (имя `.txt` файла).

**Принцип использования:**

1. **Прямая цитата** — берётся из транскрипта дословно, в `<blockquote class="principle__quote">` или `.pullquote__text` с `<cite>` атрибуцией к названию выступления.
2. **Парафраз** — допустим для UI-копи (descriptions, leads), при условии сохранения смыслового ядра. Парафраз НЕ маркируется как цитата, не получает `<cite>`.
3. **Платформенный copy** (hero h1, section title, CTA labels) — формулируется как голос платформы, без претензии на цитирование. Никаких `«»` кавычек.
4. **Атрибуция** обязательна для любого `<blockquote>` — формат: `Маргулан Сейсембай · {название выступления}`.

**Источники цитат, уже использованных на сайте (по состоянию на v2):**

| Где на сайте | Цитата (короткое содержание) | Источник-транскрипт |
|--------------|------------------------------|---------------------|
| Hero epigraph | «Стремитесь к счастью. Успех — побочный продукт.» | О мотивации |
| Pull-quote 1 (после Philosophy) | «Главный ресурс — энергия. Деньги, власть, слава, связи — её формы.» | 1070371306 (1) — Об энергии |
| Pull-quote 2 (после Principles) | «Стремиться надо к счастью, не к успеху.» | О мотивации |
| Principle 01 | «Если не определили цель — все цели разрозненны.» | Определите свою миссию |
| Principle 02 | «Наличие всех факторов не гарантирует счастья. Отсутствие любого — гарантирует несчастье.» | О 5 компонентах счастья |
| Principle 03 | «Главный ресурс — энергия. Мир — энергетическое поле.» | 1070371306 (1) |
| Principle 04 | «Главный закон — закон эффективности.» | Об эффективности |
| Principle 05 | «Кайдзен — бочка по стаканам. В единицу времени — одно дело.» | 4 инструмента продуктивного дня |
| Principle 06 | «Радость и счастье — это выбор.» | Об обидах и разочарованиях |
| Principle 07 | «Успех приходит после 10 попыток.» | Совет молодым |
| Principle 08 | «Не видел счастливого, который считал себя неуспешным.» | Успех — это счастье |

**Что ещё доступно для будущего расширения** (из 24 групп транскриптов, ещё не цитированное):
- Метафора парашюта в пустыне (миссия / распаковка талантов)
- Концепция Кансуги (принятие черного и белого мира)
- Притча о строителе и дворнике (смысл работы)
- Концепция Эриха Фромма про любовь как заинтересованность
- Энергодефицит / энергопрофицит классификация людей
- Эффективное несовершенство (анти-перфекционизм)
- Кайдзен-час (одна привычка, которую оставил бы Маргулан)
- Три уровня целей (задачи / жизненные цели / миссия)
- Менеджмент ожиданий и обиды как неоправданные ожидания
- Природа конкуренции (любовь к делу как преимущество)

**Разрешено:** добавлять новые блоки контента из этого корпуса с атрибуцией.
**Запрещено:** придумывать формулировки «в стиле Маргулана» — это нарушение правила 3.

## 7.7 AI presence pattern

Когда нужно показать AI-присутствие:
- **Pulse-точка** через `aiPulse` keyframe (2.4s loop, scale 1→1.4, opacity 0.4→1).
- **Teal edges** через `var(--color-ai-edge)` (только в зоне Mentor / Demo / sticky-bar AI signals).
- **Typewriter-эффект** для генеративного текста (22ms/char).
- **`aria-disabled`** для не-работающих элементов (Demo button) — честно.

---

# 8. RESPONSIVENESS RULES

## 8.1 Breakpoint philosophy

- **Mobile-first.** Базовые правила = мобильные.
- **3 явных breakpoint'а:** 720px, 900px, 1100px.
- **Все media queries — `min-width` only.** Никаких `max-width` кроме промежуточного `(min-width: 720px) and (max-width: 899px)` для intermediate-сеток.
- **Никаких `orientation`-queries** (вертикаль/горизонталь — мобильный поток одинаков).

## 8.2 Mobile (< 720px)

- Один column во всех секциях.
- Sticky bottom-bar с «Спросить» виден.
- Bürger-меню (две линии) → fullscreen overlay.
- Hero на 100dvh.
- Type через clamp на минимальных значениях.
- Container padding 24px.

## 8.3 Tablet (720–899px)

- Pillars: 2-кол.
- Clusters: 2-кол.
- Steps: 2-кол.
- Principles: 2-кол (без offset).
- Footer: 4-кол (через 2fr 1fr 1fr 1fr).
- Sticky-bar остаётся.

## 8.4 Desktop (≥ 900px)

- Pillars: 5-кол.
- Steps: 2-кол.
- Principles: 2-кол с asymmetric offset (even items translateY 32px, except last).
- Timeline (path): горизонтальный, 7-кол.
- Bürger исчезает, navigation visible.
- Sticky bar исчезает.
- Container padding до 32px.

## 8.5 Wide desktop (≥ 1100px)

- Clusters: 3-кол.
- Container max остаётся 1280px (не растягивается).

## 8.6 Spacing adaptation

- `--section-py` — clamp(96px, 12vw, 192px). На 320px ≈ 96px, на 1280px ≈ 153px, на 1920px ≈ 192px.
- `--container-px` — clamp(24px, 5vw, 32px).
- Между элементами spacing — фиксированные токены (--space-*), не fluid.

## 8.7 Typography adaptation

- Все display/heading/lead/body размеры — fluid через clamp.
- Meta — фиксированный 13px (читается одинаково на всех экранах).
- Тап-таргеты — минимум 44×44px (через padding на ссылках/кнопках).

## 8.8 Interaction adaptation

- Hover-эффекты — только под `@media (hover: hover) and (pointer: fine)`.
- Touch — никаких hover-only состояний; все важные действия доступны тапом.
- Reduced-motion respected всюду.

---

# 9. PERFORMANCE PHILOSOPHY

## 9.1 Optimization priorities

1. **Time to first render** — единственный HTML файл, inline CSS, нет рендер-блокирующих JS.
2. **Perceived speed** — fast first paint важнее total load time.
3. **Smoothness** — все scroll-handlers через rAF, все анимации через transform/opacity.
4. **Stability** — нет CLS благодаря fixed dimensions + `min-height: 100dvh` для hero.

## 9.2 Rendering philosophy

- **CSS-first.** Layout определяется CSS, JS только переключает классы.
- **`will-change`** не использовать постоянно. Только перед анимацией, снять после (через `.is-revealed` класс с `will-change: auto`).
- **`backdrop-filter`** только на 3 элементах (nav, dialogue, sticky-bar). Не больше.
- **Анимация только** `transform` и `opacity` (плюс `font-variation-settings` в hero — приемлемо).

## 9.3 Lazy loading rules

- **Текст:** не нужен (всё inline).
- **Изображения:** в проекте нет. Если появятся — `loading="lazy"`, `decoding="async"`, явные `width`/`height`, AVIF/WebP.
- **AI typewriter:** запускается только когда `.dialogue__answer` входит в viewport (IO с threshold 0.3).
- **Reveal-анимации:** через IntersectionObserver, после reveal — unobserve (одноразово).

## 9.4 Animation performance rules

- `transform`, `opacity` only.
- 60fps target.
- `step-end` для cursor-blink (не ease — экономнее).
- `requestAnimationFrame` для scroll-progress update.
- `transform: scaleX(N)` для progress bar (GPU layer).

## 9.5 Bundle discipline

- **One file.** Single HTTP-request для всего сайта.
- **Subset Google Fonts** — Fraunces 400–500 normal + 380–460 italic; Inter 400, 500. **Не расширять без причины.**
- **Без icon-libraries.** SVG inline (favicon как data-URI). Стрелки — символы (`→`).
- **Без analytics-скриптов** в default-сборке. Если добавится — Plausible/Cloudflare Web Analytics (без cookies).

## 9.6 Image handling

- В проекте нет изображений (по дизайн-выбору).
- Если когда-либо появится hero-image — оптимизировать через `<picture>` с AVIF/WebP source-set, явные dimensions, lazy кроме hero.

## 9.7 State efficiency

- Нет state-store, нет re-render циклов.
- DOM-классы — единственный механизм state.
- IntersectionObserver — один observer на reveal-class, не один на элемент.

## 9.8 Lighthouse цели

- Performance ≥ 92 (mobile)
- Accessibility = 100
- Best Practices ≥ 95
- SEO = 100

При деплое — прогнать DevTools Lighthouse, при результате ниже — выяснить причину перед мержем.

---

# 10. FUTURE DEVELOPMENT RULES

## 10.1 При добавлении новой секции

1. **Использовать template** из 7.1.
2. **Добавить Roman numeral** (продолжая последовательность, на сегодня — IX).
3. **Если визуально связана с соседями** — между ними `.section-mark`.
4. **Решить, нужен ли `.section--alt`** для альтернации (паттерн ink → ink-alt → ink → ink-alt).
5. **`aria-labelledby`** обязательно.
6. **`data-reveal`** на `.section-head`.
7. **`role="list"`** на любой `<ul>`/`<ol>`.

## 10.2 При добавлении нового компонента

1. **Существует похожий?** Расширь его. Если нет — создавай.
2. **Использует ли существующие токены?** Должен. Цвета/spacing/font-size — через `var(--...)`.
3. **Имеет ли hover-state?** Под `@media (hover: hover)`.
4. **Имеет ли focus-state?** Должен. `:focus-visible` outline brass.
5. **Анимируется?** Только transform/opacity, через тайминги `--dur-*` и `--ease-*`.
6. **Уважает ли reduced-motion?** Если анимация — добавь override.

## 10.3 При добавлении нового интерактива

1. **Mobile-first.** Тестируй на 375px ширине первой.
2. **Тап-таргет ≥ 44px.**
3. **Keyboard-accessible.** Если новое interactive — Tab должен попадать.
4. **`aria-*`** атрибуты по семантике.
5. **Не добавляй click outside листенеры на overlay.** (Они не нужны для fullscreen menu — выходить через X.)

## 10.4 При добавлении нового контента

1. **Из канона** (см. 7.6) или из реальных транскриптов Маргулана.
2. **Не выдумывай цитаты.** Если нет источника — формулируй как платформенный copy, не маскируй под цитату.
3. **Атрибуция** обязательна для всего, что может быть прочитано как цитата Маргулана.
4. **Тон сдержанный.** Без маркетинга. Без хайповых формулировок.
5. **На русском.** Английский — только для брендовых элементов (имя продукта, CTA-titles).

## 10.5 При добавлении нового цвета

**По умолчанию — НЕ добавлять.** Палитра завершена.

Если действительно нужен (например, success-state для будущей формы) — обсудить с пользователем. Если решено — добавить как `--color-*` в `:root`, документировать в этом файле в секции 3.1.

## 10.6 При добавлении нового шрифта

**По умолчанию — НЕ добавлять.** Пара Fraunces+Inter завершена. Третий шрифт нарушает дисциплину.

Если действительно нужен mono для технического раздела — обсудить. Если решено — JetBrains Mono или IBM Plex Mono, через тот же Google Fonts CSS, subset под ASCII.

## 10.7 При добавлении новой анимации

1. Только transform/opacity (или font-variation-settings).
2. Тайминги через `--dur-*` токены.
3. Easing через `--ease-*` токены.
4. Если keyframe — добавить override в `prefers-reduced-motion`.
5. Если scroll-driven — IntersectionObserver, не scroll listener.

## 10.8 Что **НИКОГДА** не делать

- Не добавляй framework (React/Vue/Svelte).
- Не добавляй Tailwind.
- Не добавляй jQuery/lodash/axios.
- Не добавляй analytics-скрипты без согласования.
- Не добавляй чат-виджеты (Intercom, Drift).
- Не добавляй pop-up подписки на рассылку.
- Не добавляй cookie-баннер пока не используешь cookies.
- Не добавляй маркетинговые блоки «trusted by», «testimonials with avatars», «as seen in».
- Не добавляй stock-фото людей.
- Не используй emoji-иконки.
- Не используй цветные пиктограммы (ни одной — линейные SVG inline brass-only если действительно нужны).
- Не вводи новые цвета без обсуждения.
- Не вводи новый шрифт.
- Не вводи новую анимацию timing-вне токенов.

---

# 11. AI SESSION CONTINUATION PROTOCOL

## 11.1 Перед началом работы

**Обязательные шаги:**

1. Прочитай этот CLAUDE.md **полностью**. Не пропускай разделы.
2. Открой [index.html](index.html) и просмотри структуру (хотя бы Read с большим limit).
3. Найди секцию, которую тебя просят менять, и **прочитай весь её CSS-блок** в `<style>`.
4. Найди соответствующий HTML-блок и прочитай его.
5. Если задача затрагивает JS — прочитай весь IIFE.

## 11.2 Принципы работы

1. **Reuse > Recreate.** Прежде чем создавать новое — проверь, нет ли существующего паттерна.
2. **Tokens > Hardcoded.** Никаких hex-цветов, px-значений напрямую — всегда через `var(--*)`.
3. **Match the voice.** Тексты — сдержанные, философские, на русском. Без маркетинга.
4. **Match the motion.** Все новые анимации — в семействе ease-out, тайминги через токены, обязательная reduced-motion guard.
5. **Match the markup.** Семантический HTML, BEM-имена классов, role/aria по необходимости.
6. **Plan before code.** Короткий план (3–7 пунктов) до правок (правило 4 проекта).
7. **Self-review after.** Проверь по 13 правилам после правки (правило 5 проекта).

## 11.3 Workflow

```
[задача от пользователя]
    ↓
[прочитай CLAUDE.md]
    ↓
[прочитай относящиеся секции index.html]
    ↓
[короткий план — 3-7 пунктов]
    ↓
[Edit или Write]
    ↓
[self-review по 13 правилам + checks (см. 11.4)]
    ↓
[отчёт: что сделано / что улучшено / как проверить]
```

## 11.4 Checks после правок

- `grep "console\.|debugger|TODO"` → должно быть 0.
- `grep "href=\"#\""` → должно быть 0 (нет мёртвых ссылок).
- `grep "cursor: pointer"` → только в `.btn` и в `button` reset, нигде больше.
- Все `aria-labelledby` ссылки имеют существующие `id`.
- Все `href="#anchor"` имеют существующие `id="anchor"`.
- `role="list"` есть на всех `<ul>`/`<ol>` со снятым list-style.
- `[data-reveal]` имеет связь с JS observer.
- Новые анимации имеют `prefers-reduced-motion` override.
- Lighthouse не упал ниже 90/100/95/100.

## 11.5 Что НЕ делать в новой сессии

- **НЕ переписывай весь файл, если задача — точечная.** Используй Edit.
- **НЕ изобретай новые компоненты, когда есть существующие.**
- **НЕ меняй визуальный язык** (палитру, шрифты, тайминги) без явного запроса.
- **НЕ добавляй фреймворки/либы.**
- **НЕ выдумывай контент.** Если не знаешь — спроси у пользователя.
- **НЕ удаляй секции без разрешения.**
- **НЕ переименовывай классы массово** (поломает связи).

## 11.6 Когда сомневаешься

- Спроси пользователя.
- Перечитай этот CLAUDE.md.
- Сверься с index.html — что-то похожее уже наверняка есть.
- Прочитай [memory file project_council_of_advisors.md](../../.claude/projects/c--Users-ildmu-git-practice/memory/project_council_of_advisors.md) для контекста большой картины (multi-agent система).

## 11.7 Известный roadmap (открытые задачи)

В порядке приоритета:

1. **GitHub + Vercel deploy** — готов к запуску.
2. **`vercel.json`** для cache-headers + security-headers (если запросят).
3. **`README.md`** с deploy-кнопкой и скриншотами (если запросят).
4. **`.gitignore`** минимальный для статики.
5. **OG-image** (1200×630, тёмный фон с brass-accent).
6. **Self-hosted fonts** вместо Google Fonts CDN.
7. **`favicon.ico` + `apple-touch-icon`** (сейчас только inline SVG).
8. **`sitemap.xml` + `robots.txt`**.
9. **Контентная глубина** — раскрыть пилары и принципы до 3-4 строк с цитатами и атрибуциями (требует материала Маргулана).
10. **Реальный AI** — связать сайт с RAG-агентом из соседней папки.
11. **Отдельные страницы тем** — `/принципы/[slug]/` для каждой из 23 тем (потребует Astro).
12. **2-3 разных AI-диалога** через табы (демонстрация на разные ситуации).

---

# 12. DESIGN DNA SUMMARY

## Soul of the project

> Это **тихий редакционный кабинет executive-наставника**, временно расположенный в браузере. Не landing AI-продукта. Не блог. Не collection-of-quotes. **Система мышления**, поданная как структурированная книга, с одним living AI-портом в её середине.

## Core visual traits

- **Tasteful executive dark**: ink (#0E0E0F) + paper (#F2EFEA) + brass (#C8A368), плюс teal-edge (rgba 120,180,195) только в AI-зоне.
- **Editorial typography first**: Fraunces (variable serif) для всей экспрессии, Inter (variable sans) для UI/body. Никакого третьего семейства. Никаких bold-весов.
- **Roman chapter numerals (I–VIII)** на каждой контентной секции — сайт читается как нон-фикшн книга.
- **Аналоговый грейн** через SVG turbulence overlay (opacity 0.5 + mix-blend overlay) убирает «цифровую плоскость».
- **Минимум декора**: 0 border-radius (кроме точек), 0 box-shadow (кроме одного на AI-card), 0 цветных иконок, 0 эмодзи, 0 stock-фото.
- **Brass-точки** как единственный акцент: meta-метки, номера, focus, AI-pulse, scroll-progress, attribution.

## Core engineering traits

- **Single-file static**: один `index.html`, inline CSS+JS, без сборки, deploy by drag-drop.
- **Vanilla**: нет фреймворков, нет либ кроме Google Fonts CSS-CDN.
- **CSS custom properties** для всех токенов; **`clamp()`** для всего fluid; **container-as-grid**, не flex-cosplay.
- **Modern web 2026**: variable fonts, fluid type, `dvh`, `inert`, `:focus-visible`, `text-wrap: balance/pretty`, `hanging-punctuation`, `font-feature-settings`, `font-variant-numeric`.
- **A11y baseline**: WCAG AA+, `inert` для overlay-isolation, focus-trap в menu, skip-link, semantic HTML, role/aria-* по семантике.
- **Performance**: один HTTP-запрос на HTML, subset fonts, IntersectionObserver не scroll-listeners, `requestAnimationFrame` для scroll-handlers, `will-change` управляется.
- **Reduced motion** уважается на каждой keyframe и каждом transitionна.

## Core UX traits

- **Mobile-first** буквально: базовые стили = мобильные, media-queries только увеличивают.
- **Один primary CTA на секцию + sticky-bar внизу мобильного**: «Спросить» доступен с любой точки.
- **Editorial reveal**: opacity + translateY 16px, 720ms ease-content, stagger 80ms между сиблингами.
- **Calm motion**: всё движется как будто думает (280–640ms ease-out), никакого spring/bounce/elastic.
- **Living AI presence**: pulse-точка возле «О.», typewriter, teal-edge в AI-блоке, sticky-bar pulse — но **только в AI-зоне**.
- **Эпистолярный AI-формат**: В./О., не chat-bubble. AI читается как письмо, не как мессенджер.
- **Honest demo**: disabled textarea + Demo-badge — не врёт о том, чего нет.
- **Атрибуция**: каждое заявление о Маргулане либо со ссылкой, либо явно как платформенный copy (никогда не маскируется под цитату).

---

## Окончание

Если ты — будущая сессия, которая дочитала до этого места: **продолжай в этом духе.** Каждое решение в этом проекте было сделано осознанно. Tasteful executive dark, editorial typography, roman chapter numerals, brass-only accents, calm motion, honest AI presence — это не «текущий вариант». Это **продукт**.

Меняй — да. Но в этом языке.

— Маргулан Personal Mentor AI · Project DNA · 2026
