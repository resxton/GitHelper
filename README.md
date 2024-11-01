# GitHelper: Шпаргалка по Git

Набор полезных команд для работы с Git, включая базовые и продвинутые команды. 

## Основные команды

### 1. Инициализация репозитория
Создает новый локальный Git-репозиторий в текущей папке.
```bash
git init
```

### 2. Клонирование репозитория
Клонирует удаленный репозиторий в указанную папку.
```bash
git clone <url>
```

### 3. Проверка статуса
Отображает текущий статус репозитория (измененные, неотслеживаемые файлы и т.д.).
```bash
git status
```

### 4. Добавление файлов в область подготовленных
Добавляет указанный файл (или все файлы с `.`) в область подготовленных для коммита.
```bash
git add <имя_файла>
git add .
```

### 5. Создание коммита
Фиксирует изменения с сообщением о коммите.
```bash
git commit -m "Сообщение о коммите"
```

## Работа с ветками

### 6. Создание новой ветки
Создает новую ветку с указанным именем, не переключаясь на неё.
```bash
git branch <имя_ветки>
```

### 7. Переключение на другую ветку
Переключает на указанную ветку.
```bash
git checkout <имя_ветки>
```

### 8. Создание и переключение на новую ветку
Удобный способ создать новую ветку и сразу переключиться на неё.
```bash
git checkout -b <имя_ветки>
```

## Работа с удаленными репозиториями

### 9. Добавление удаленного репозитория
Добавляет удаленный репозиторий с именем `origin`.
```bash
git remote add origin <url>
```

### 10. Отправка изменений в удаленный репозиторий
Отправляет коммиты текущей ветки в удаленный репозиторий.
```bash
git push origin <имя_ветки>
```

### 11. Получение изменений из удаленного репозитория
Загружает изменения с удаленного репозитория.
```bash
git pull origin <имя_ветки>
```

## Работа с историей

### 12. Просмотр истории коммитов
Отображает список коммитов.
```bash
git log
```

### 13. Сравнение изменений
Показывает различия между текущими изменениями и последним коммитом.
```bash
git diff
```

## Откат изменений

### 14. Сброс изменений в файле
Возвращает указанный файл к состоянию последнего коммита.
```bash
git checkout -- <имя_файла>
```

### 15. Удаление последнего коммита
Удаляет последний коммит, сохраняя изменения в рабочем каталоге.
```bash
git reset --soft HEAD~1
```

### 16. Полный откат изменений
Удаляет все изменения и сбрасывает репозиторий к указанному коммиту.
```bash
git reset --hard <id_коммита>
```
---