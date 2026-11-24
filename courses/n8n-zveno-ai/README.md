# AI-агент в n8n с ZvenoAI — материалы курса Stepik 307809

Открытые учебные материалы для курса [AI-агент в n8n на любой модели без VPN](https://stepik.org/course/307809/syllabus).

**Регистрация в ZvenoAI по реферальной ссылке автора:** https://zveno.ai/?ref=plMvItdv

## Материалы

- [Пошаговая инструкция подключения](guide/00-zveno-n8n-start.md)
- [Первый чат — готовый workflow JSON](workflows/01-first-chat.json)
- [Разбор заявки — готовый workflow JSON](workflows/02-intake-agent.json)
- [Агент с каталогом — готовый workflow JSON](workflows/03-agent-with-catalog.json)
- [Итоговый безопасный агент — готовый workflow JSON](workflows/04-final-safe-agent.json)
- [Docker Compose для запуска n8n](examples/docker-compose.yml)
- [Учебный каталог товаров](examples/catalog.csv)
- [Тестовые случаи](examples/test-cases.csv)
- [Примеры входных сообщений](examples/fixtures/)

## Использование

Чтобы импортировать workflow JSON в n8n, откройте соответствующий файл, нажмите Raw, сохраните его как JSON и импортируйте через n8n Import from File. Credential с API-ключом ZvenoAI создаётся в интерфейсе n8n и не входит в JSON.

Данные каталога демонстрационные. Workflow 03 и 04 требуют модель с поддержкой tool calling. Импорт и выполнение всех схем с реальным API ZvenoAI ещё не подтверждены интеграционным тестом; проверьте вашу версию n8n и модель.

Исходный код курса и механизмы публикации остаются в приватном репозитории; здесь размещены только материалы для учеников без секретов.
