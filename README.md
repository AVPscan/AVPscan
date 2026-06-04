# Alexey Vasilievich Pozdnyakov (AVPscan)

## 🧬 Programs do not depend on:

- **Operating system** `terminal/sys_*.c` for demonstration on current OSes
- **Graphics card** `Fps` is just a constant
- **Processor** `32/64/128...Cell` auto-adaptation
- **Monitor** `8k/16k/32k...CellPow` auto-adaptation
- **Geo-adaptive system** `Hz` mains frequency, `UTF8` full support without libraries, auto-adaptation
- **Color depth** mathematically decomposed spectrum based on depth, auto-adaptation
- **"Ecosystems"** `Libc` is essentially unnecessary

One binary (16–57 KB) works **identically** on Linux, Windows, macOS, in Docker, over SSH, and on embedded systems. No modifications. No runtimes. No virtualization.

### [Fresh](https://github.com/AVPscan/Fresh) — Runtime Environment

**19 KB.MuslStatic** Completely independent development environment.

## 🌟 What's inside v8.0

- **16K Graphics** via Braille `change constant → 32K, 64K`
- **Window System** Z-order, hierarchy, overlapping, `512 windows`
- **Event Model** `256` handlers, key binding to functions
- **Context Dispatching** handlers know which window they were called for
- **RT Input** buffered keyboard `255/510 keys`, any mouse with horizontal scroll `+Shift`
- **Viewport** free movement or inside windows
- **Frame Function** automatic data update
- **No data movement on the canvas**
- **FPS** regulated by a single constant `20 ms → 50 Hz`
- **Works even over SSH, without GPU**
- **Example application** see `main.c` — 11 lines of code create windows, menus, RealTime events, and works everywhere.

### [Products](https://github.com/AVPscan/Products) — Smart Shopping & Analytics

**57 KB.** A full-featured application for purchase tracking, price analytics, and report sending.

- Fast entry of three fields (quantity, price, name)
- Auto-completion from dictionary
- Weighted average price analytics
- **HWID binding and encryption** (email/password not stored in plain text)
- Automatic email report sending
- Cross-platform (Linux/Windows/macOS)

> *Both projects — GPLv3. One person. No management, no grants, no "ecosystems". Only code that works.*

---

## 📜 Brief History

- **January 2026** — wrote **Products** for my wife (so she could make shopping lists and estimate budgets)
- **February 2026** — started extracting common mechanisms into a separate engine → **Fresh** was born
- **April 2026** — both projects published, documented, working

**Ideas from these projects** appear daily on open.net (3 out of 6 news items). People see the power. They use it. According to GPLv3, authorship is preserved.

---

## 🔧 My Approach

- **Pure C11** — as a reliable layer, but I write as if in assembly or Forth
- **No libraries** — only system calls and my own memory
- **RDTSC** — timing calibration, microsecond delays
- **UTF-8 without libicu** — my own parser, support for all languages and RTL
- **Bitness auto-adaptation** — code automatically adapts to 32/64/128 bit
- **Cross-platform** — 5 functions for the system layer, and it's done

---

## 🌀 My Credo

> *"The terminal is not static, it's a window into the world of data. If the code is written correctly, it will work everywhere as if it were native, without requiring graphics cards."*
>
> *"You no longer need to know GTK, Qt, and other OS layers. And if you haven't programmed before — read a book on Forth and save years at university."*

---

## 📡 Contact

- **Email:** avp70ru@mail.ru
- **GitHub:** [AVPscan](https://github.com/AVPscan)

**Open for complex system programming and optimization tasks.** But most importantly — I create things that won't become obsolete in a year.

---

*P.S. Yes, it all works even over SSH. Yes, on a Raspberry Pi. Yes, on a 32-bit processor. Yes, without a graphics card. No, it's not magic. It's just C and 35 years of the right experience, which once turned into a gift for my wife, and then — into a tool for the whole world.*

---

# Алексей Васильевич Поздняков (AVPscan)
## 🧬 Программы не зависят от:
- операционной системы `terminal/sys_*.c` для демонстрации на текущих осях
- видеокарты `Fps` просто константа
- процессора `32/64/128...Cell` автоадаптация
- монитора `8k/16k/32k...CellPow` автоадаптация
- гео-адаптивная система `Hz` частоте питающей сети `UTF8` полная поддержка без библиотек автоадаптация
- цветность математически разложен спектр исходя из глубины автоадаптация
- «экосистем» `Libc` по сути лишнее
Один бинарник (16–57 КБ) работает **одинаково** на Linux, Windows, macOS, в Docker, по SSH и на встраиваемых системах. Без доработок. Без рантаймов. Без виртуализации.
### [Fresh](https://github.com/AVPscan/Fresh) — среда исполнения
**19 КБ.MuslStatic** Полностью независимая среда разработки.
## 🌟 Что внутри v8.0
- **Графика 16K** через браэль `меняем константу → 32K, 64K`
- **Оконная система** Z-порядок, иерархия, перекрытия, `512 окон`
- **Событийная модель** `256` обработчиков, привязка клавиш к функциям
- **Контекстная диспетчеризация** обработчики знают, для какого окна вызваны
- **RT-ввод** буферизированная клавиатура `255/510 клавиш`, любая мышь с горизонтальным скроллом `+Shift`
- **Вьюпорт** свободное перемещение или внутри окон
- **Кадровая функция** автоматическое обновление данных
- **Нет перемещений данных на холсте**
- **FPS** регулируется одной константой `20 мс → 50 Гц`
- **Работает даже по SSH, без GPU**
- **Пример приложения** смотрите в `main.c` 11 строк кода создают окна, меню, события RealTime и работает везде.

### [Products](https://github.com/AVPscan/Products) — умные покупки и аналитика
**57 КБ.** Полноценное приложение для учёта покупок, аналитики цен и отправки отчётов.
- Быстрый ввод трёх полей (количество, цена, название)
- Автодополнение из словаря
- Аналитика средневзвешенных цен
- **HWID-привязка и шифрование** данных (почта/пароль не хранятся в открытом виде)
- Автоматическая отправка отчётов на email
- Кроссплатформа (Linux/Windows/macOS)

> *Оба проекта — GPLv3. Один человек. Без начальства, без грантов, без «экосистем». Только код, который работает.*
---
## 📜 Краткая история
- **Январь 2026** — написал **Products** для жены (чтобы составляла список покупок и прикидывала бюджет)
- **Февраль 2026** — начал выносить общие механизмы в отдельный движок → родился **Fresh**
- **Апрель 2026** — оба проекта опубликованы, документированы, работают
**Идеи из этих проектов** ежедневно появляются на open.net (3 из 6 новостей). Люди видят мощь. Используют. Согласно GPLv3, авторство сохраняется.
---
## 🔧 Мой подход
- **Чистый C11** — как надёжная прокладка, но пишу как на ассемблере или Forth'е
- **Никаких библиотек** — только системные вызовы и своя память
- **RDTSC** — калибровка таймингов, микросекундные задержки
- **UTF-8 без libicu** — своя парсер, поддержка всех языков и RTL
- **Автоадаптация под разрядность** — код сам подстраивается под 32/64/128 бит
- **Кроссплатформа** — 5 функций для системного слоя, и готово
---
## 🌀 Моё кредо
> *«Терминал — это не статика, это окно в мир данных. Если код написан правильно, он будет работать во всём мире как родной, не требуя видеокарт.»*
> *«Вам больше не нужно знать GTK, Qt и прочие слои в ОС. А если вы не программировали — прочитайте книгу по Forth'у и сэкономите годы в вузе.»*
---
## 📡 Связь
- **Email:** avp70ru@mail.ru
- **GitHub:** [AVPscan](https://github.com/AVPscan)
**Открыт для сложных задач по системному программированию и оптимизации.** Но главное — я создаю вещи, которые не устареют через год.
---
*P.S. Да, это всё работает даже по SSH. Да, на Raspberry Pi. Да, на 32-битном процессоре. Да, без видеокарты. Нет, это не магия. Это просто C и 35 лет правильного опыта, который однажды превратился в подарок для жены, а потом — в инструмент для всего мира.*

[![Linux musl static +(Cross-Platform)](https://github.com/AVPscan/Fresh/actions/workflows/release.yml/badge.svg)](https://github.com/AVPscan/Fresh/actions/workflows/release.yml)
