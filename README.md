Для запуска требуется docker с плагином compose. Если установлен docker desktop, то значит, что compose уже установлен.

### Загрузка

Для загрузки репозитория использовать команду

```bash
git clone --recurse https://github.com/crazyfrequency/SummerOpenCodeFullStack
```

### Запуск

сборка проекта(необходимо только после внесения изменений)

```bash
docker compose build
```

запуск

```bash
docker compose up
```

запуск в фоне

```bash
docker compose up -d
```

Порт сайта 83: `http://localhost:83/`

Также может потребоваться очистить таблицы:

Порт для подключения к бд `15432`

```sql
DROP TABLE IF EXISTS acc_rstr_list, accounts, bic_directory_entry, import_data, initial_ed, part_info, participant_info, rstr_list, swbics
```
