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
