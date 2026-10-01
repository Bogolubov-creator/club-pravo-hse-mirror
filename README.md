# club-pravo-hse-mirror

Публичное зеркало портала клуба выпускников факультета права НИУ ВШЭ.

- **Сайт:** [Pages-зеркало](https://bogolubov-creator.github.io/club-pravo-hse-mirror/).
- **Исходник:** [Bogolubov-creator/hse-law-alumni-club](https://github.com/Bogolubov-creator/hse-law-alumni-club) (`frontend/club_web`, экспорт Jinja2-шаблонов).
- **Инструкция:** [Статическое зеркало](https://github.com/Bogolubov-creator/hse-law-alumni-club/blob/main/docs/integrations/pages-mirror.md).
- **Опубликованная версия:** [version.json](https://bogolubov-creator.github.io/club-pravo-hse-mirror/version.json).

На Pages есть витрины, демо-кабинет и демо-админка. Живого API и сохранения
заявок или изменений нет; онлайн-оплата отключена. Обычная сборка берёт исходник
из `main` монорепозитория.

Ручное обновление: workflow **Deploy Pages mirror**, поле `source_ref` – коммит,
ветка или тег исходника. Сборка использует Python 3.14.7 и uv 0.12.21.
В `version.json` записаны SHA исходника и время сборки; успешная публикация
проверяется по этому файлу и результату задания `deploy`.
