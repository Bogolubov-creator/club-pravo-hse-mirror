# club-pravo-hse-mirror

Публичное зеркало портала клуба выпускников факультета права НИУ ВШЭ.

- **Сайт:** [Pages-зеркало](https://bogolubov-creator.github.io/club-pravo-hse-mirror/).
- **Исходник:** [Bogolubov-creator/hse-law-alumni-club](https://github.com/Bogolubov-creator/hse-law-alumni-club) (`frontend/club_web`, экспорт Jinja2-шаблонов).
- **Инструкция:** [Статическое зеркало](https://github.com/Bogolubov-creator/hse-law-alumni-club/blob/main/docs/integrations/pages-mirror.md).
- **Опубликованная версия:** [version.json](https://bogolubov-creator.github.io/club-pravo-hse-mirror/version.json).

На Pages есть витрины, кабинет с демонстрационными достижениями и панель офиса.
Опросы и итоги показаны в [кабинете](https://bogolubov-creator.github.io/club-pravo-hse-mirror/lk/#polls)
и [офисе](https://bogolubov-creator.github.io/club-pravo-hse-mirror/admin/polls/);
вопросы и голоса вымышлены, отправка отключена. Живого API и сохранения заявок
или изменений нет; онлайн-оплата отключена. Обычная сборка берёт исходник из
`main` монорепозитория.

Ручное обновление: workflow **Deploy Pages mirror**, поле `source_ref` – коммит,
ветка или тег исходника. Для выпуска указывайте полный 40-символьный SHA
проверенного `main`. Сборка использует Python 3.14.8 и uv 0.13.4.
Перед экспортом выполняются браузерные тесты зеркала и панели офиса.
GitHub Actions закреплены по SHA коммитов.
В `version.json` записаны SHA исходника и время сборки; успешная публикация
проверяется по этому файлу и результату задания `deploy`.
