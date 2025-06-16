 Завдання: “Git Rescue: Відновлення марсіанського проєкту”
 📘 Сюжет:
Твій марсіанський науковий центр втратив дані про важливі експерименти. Лише ти маєш локальну копію репозиторію. Твоя місія — відновити структуру проєкту, відредагувати файли, створити нові гілки, і без помилок виконати злиття.
 Крок 1: Створення репозиторію
Відкрий GitHub Desktop.

Натисни "File → New repository".

Назва: mars-project

Додай опис: Проєкт для відновлення марсіанської бази

Створи README.md (галочка при створенні).

Натисни "Publish repository" — обери свій GitHub акаунт.

 Крок 2: Робота з файлами
У файловій системі відкрий папку репозиторію.

Створи файл base.txt з текстом:
Стан бази: аварійний. Потрібна діагностика.
Повернись у GitHub Desktop:

Побачиш зміни (Uncommitted changes)

Введи коментар: Add base status file

Зроби коміт ("Commit to main")

Натисни "Push origin"
 Крок 3: Створення гілки
У GitHub Desktop натисни "Current Branch" → New Branch"

Назви гілку: diagnostics

У файловій системі створи файл diagnostics.txt:
Проведено первинне сканування. Стан: нестабільний.
Зроби коміт з назвою Add diagnostics report

Натисни "Push origin"
Крок 4: Редагування в main
Перемкнись назад на main (Current Branch → main)

Відредагуй файл base.txt, змінивши його на:
Стан бази: стабільний. Робота систем відновлена.
Зроби коміт: Update base status after recovery

Push

 Крок 5: Злиття гілок
Перемкнись знову на main

У меню "Branch" → "Merge into current branch"

Обери гілку diagnostics

Якщо буде конфлікт (GitHub Desktop покаже це), обери "Resolve Conflicts" → "Open in editor", виправ конфлікт самостійно.

Натисни "Mark as resolved", потім — "Commit merge"

 Крок 6: Перевірка структури
У підсумку у тебе має бути:

Гілка main з файлами:

README.md

base.txt (оновлений)

diagnostics.txt

В історії: принаймні 4 коміти (init, base, diagnostics, merge)

