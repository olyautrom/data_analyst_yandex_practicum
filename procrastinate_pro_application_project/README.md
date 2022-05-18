## Исследование надёжности заёмщиков

### Спринт: 
Анализ бизнес-показателей

### Цель проекта:
Задача для маркетингового аналитика развлекательного приложения Procrastinate Pro+. Несмотря на огромные вложения в рекламу, последние несколько месяцев компания терпит убытки. Задача — разобраться в причинах и помочь компании выйти в плюс.

### Навыки и инструменты:
Matplotlib, Pandas, Python, Seaborn, когортный анализ, продуктовые метрики, юнит-экономика

### Описание проекта:
Проведен анализ данных от ProcrastinatePRO+.
Рассчитаны различные метрики, использован когортный анализ: LTV, CAC, Retention rate, DAU, WAU, MAU и т.д. Использованы уже написанные ранее функции расчёта метрик. Сделаны правильные выводы по полученным данным.

### Данные:
Таблица visits (лог сервера с информацией о посещениях сайта):
- `user_id` — уникальный идентификатор пользователя
- `device` — категория устройства пользователя
- `session_start` — дата и время начала сессии
- `session_end` — дата и время окончания сессии
- `channel` — идентификатор рекламного источника, из которого пришел пользователь
- `region` - страна пользователя

Таблица orders (информация о заказах):
- `user_id` — уникальный id пользователя, который сделал заказ
- `event_dt` — дата и время покупки
- `revenue` — выручка

Таблица costs (информация о затратах на маркетинг):
- `channel` — идентификатор рекламного источника
- `dt` — дата
- `costs` — затраты на этот рекламный источник в этот день

Используемые библиотеки:
- pandas
- numpy
- matplotlib.pyplot
- datetime