# new-project

Навчальний репозиторій для практики з Git.

## Інструкція для розробників

### Початок роботи

    git clone git@github.com:chumachenko-vy/new-project.git
    cd new-project
    git switch development

### Гілки

- `main` — стабільна версія, напряму в неї не комітимо.
- `development` — гілка для розробки, всі зміни робимо тут.

### Процес

1. Перейдіть у `development` і підтягніть останні зміни: `git pull`.
2. Внесіть зміни, додайте їх до коміту: `git add <файли>`.
3. Закомітьте зміни у форматі Smart Commit (див. нижче).
4. Відправте зміни: `git push`.
5. Після перевірки зміни зливаються в `main`: `git switch main && git merge development`.

### Формат коміт-повідомлень (Jira Smart Commits)

    <КЛЮЧ-ЗАДАЧІ> #comment <коментар> #time <час> #<перехід>

Приклад:

    NP-1 #comment Додано інструкцію для розробників #time 30m #done

- `#comment` — коментар до задачі в Jira;
- `#time` — облік часу (`1w 2d 4h 30m`);
- `#<перехід>` — зміна статусу задачі, наприклад `#in-progress` або `#done`.
