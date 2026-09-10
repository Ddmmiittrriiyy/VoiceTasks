# Update: navigation / focus

- При открытии активного списка приложение автоматически позиционируется на сегодняшнем дне и текущем времени.
- В сегодняшнем блоке добавлена ненавязчивая линия «Сейчас HH-MM» в правильной позиции между задачами.
- Если на сегодня задач нет, визуальный блок сегодняшней даты создаётся только для ориентации; данные задач не изменяются.
- После создания новой задачи сортировка остаётся прежней, но экран автоматически прокручивается к новой карточке.
- Новая карточка располагается ниже середины экрана и кратко подсвечивается для быстрой проверки.
- Уведомления не добавлялись.

# VoiceTasksPlanner — theme update

This version keeps the existing task logic and adds only visual theme support plus overdue-date highlighting.

- Light theme is the default for a new installation/browser profile.
- Moon/sun theme switch is placed beside the three-dot import/export menu.
- Theme choice is stored locally and restored on the next launch.
- Existing dark theme is preserved.
- Overdue active task cards retain a dashed underline and danger-color time.
- Date headers containing overdue tasks are highlighted in the danger color.
- A task on a past date is overdue even if no exact time was entered; for today, time is used when present.

## Parser expansion
- RU/UA/EN: hour words expanded from 1–4 to 1–12.
- Explicit parts of day supported both after and before time: «в шесть вечера», «вечером в шесть», «в 6 утра», «утром в шесть».
- Added time prepositions such as «на 18:30», «к 18:30» (RU) and matching UA/EN forms.
- Added speech-recognition form «в 18 30» for cases where dictation drops the colon.
- Added named-month dates with year: «10 сентября 2026», and ordinal form «10-го сентября».
- Added relative dates «через 2 дня / через два дня», UA and EN equivalents.
- Existing task ordering, themes, overdue highlighting, current-time line, and focus/highlight behavior are unchanged.


## v3.2 — parser fix
- Fixed the actual runtime config: ambiguousAfternoonMax changed from 4 to 7 for RU/UA/EN.
- Verified: «в 6» → 18:00, «в 7» → 19:00, «в 8» → 08:00, «в 10» → 10:00.


## v3.3 — original proven parser
- Parser section restored verbatim from the tested main version.
- Date/weekday/time parsing is unchanged from that version.
- Light/dark theme, overdue styling, current-time marker, auto-focus and new-task highlight remain from the current UI.


## v3.5 — natural date/time phrases
- Added RU forms: утро/утром/утра/с утра; день/днём/дня/после обеда; вечер/вечером/вечера; ночь/ночью/ночи.
- Daypart can appear before or after the hour.
- Added "на следующей неделе + weekday" parsing.
- Existing today/tomorrow/day-after-tomorrow and nearest-weekday logic retained.
