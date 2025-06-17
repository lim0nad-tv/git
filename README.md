
# 🚀 Домашнее задание к занятию "`8.03. GitLab CI/CD`"  
**Автор:** _Расулов Магомед_

---



## ✅ Задание 1

**Создание репозитория и первичный коммит**

1. ✅ Аккаунт на GitHub: [lim0nad-tv](https://github.com/lim0nad-tv)
2. ✅ Репозиторий: [lim0nad-tv/git](https://github.com/lim0nad-tv/git)
3. ✅ Конфигурация Git:
   ```bash
   git config --global user.name "Расулов Магомед"
   git config --global user.email "rasulov999@yandex.ru"
   ```
4. ✅ Проверка статуса:
   ```
   On branch main
   nothing to commit, working tree clean
   ```
5. ✅ Добавил изменения:
   ```bash
   git add README.md
   git commit -m "First commit"
   git push origin main
   ```
6. ✅ Ссылка на коммит:  
   🔗 [54135c3](https://github.com/lim0nad-tv/git/commit/54135c3eaf9f4cde3c8087fab2070a93e290c139)

---

## ✅ Задание 2

**Добавление .gitignore**

1. Создание и редактирование:
   ```bash
   touch .gitignore
   echo "*.pyc cache/" > .gitignore
   ```
2. Коммит и пуш:
   ```bash
   git add .gitignore
   git commit -m "Добавлен .gitignore для игнорирования *.pyc и папки cache"
   git push origin main
   ```
3. ✅ Ссылка на коммит:  
   🔗 [c5532fa](https://github.com/lim0nad-tv/git/commit/c5532fa0fd491389f8bbdf7a6a2dc1b6b1476d51)

---

## ✅ Задание 3

**Работа с ветками и объединение**

1. Создание ветки `dev`:
   ```bash
   git checkout -b dev
   ```
2. Работа с `test.sh`:
   ```bash
   echo '#!/bin/bash' > test.sh
   echo 'echo "Привет из ветки dev!"' >> test.sh
   chmod +x test.sh
   git add test.sh
   git commit -m "Добавлен файл test.sh с начальным содержимым"
   git push -u origin dev
   ```
3. Дополнение:
   ```bash
   echo 'echo "Ветка dev развивается!"' >> test.sh
   git add test.sh
   git commit -m "Обновлено содержимое test.sh"
   git push origin dev
   ```
4. Переход в `main` и создание `main.sh`:
   ```bash
   git checkout main
   echo '#!/bin/bash' > main.sh
   echo 'echo "Привет из ветки main!"' >> main.sh
   chmod +x main.sh
   git add main.sh
   git commit -m "Добавлен файл main.sh"
   git push origin main
   ```
5. Слияние веток:
   ```bash
   git merge --no-ff dev
   git push origin main
   ```

🔗 **Граф коммитов**:  
[https://github.com/lim0nad-tv/git/network](https://github.com/lim0nad-tv/git/network)

---



