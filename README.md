# club-pravo-hse-mirror

Публичное зеркало портала клуба выпускников факультета права НИУ ВШЭ.

- **Сайт:** [Pages-зеркало](https://bogolubov-creator.github.io/club-pravo-hse-mirror/).
- **Исходник:** [Bogolubov-creator/hse-law-alumni-club](https://github.com/Bogolubov-creator/hse-law-alumni-club) (`frontend`, режим `VITE_MIRROR`).
- **Инструкция:** [Статическое зеркало](https://github.com/Bogolubov-creator/hse-law-alumni-club/blob/main/docs/integrations/pages-mirror.md).
- **Опубликованная версия:** [version.json](https://bogolubov-creator.github.io/club-pravo-hse-mirror/version.json).

На Pages есть витрины, демо-кабинет и демо-админка. Живого API и сохранения
заявок или изменений нет; онлайн-оплата отключена. Обычная сборка берёт исходник
из `main` монорепозитория.

Ручное обновление: workflow **Deploy Pages mirror**, поле `source_ref` – коммит,
ветка или тег исходника. Сборка использует Node.js 24.21.0 и pnpm 12.8.1.
В `version.json` записаны SHA исходника и время сборки; успешная публикация
проверяется по этому файлу и результату задания `deploy`.
