<img align="right" width="150" alt="logo" src="https://user-images.githubusercontent.com/5889006/190859553-5b229b4f-c476-4cbd-928f-890f5265ca4c.png">

# Шаблон-стартер Hugo с темой Hugo Stack

В комплекте настроенная структура и конфигурация темы. 

## Начало работы

1. Нажмите *Use this template* и создайте репозиторий с именем `<username>.github.io` на GitHub.
![Шаг 1](https://user-images.githubusercontent.com/5889006/156916624-20b2a784-f3a9-4718-aa5f-ce2a436b241f.png)

2. Откройте Settings -> Pages. Измените ветку сборки с `master` на `gh-pages`.
![Сборка](https://github.com/namanh11611/hugo-theme-stack-starter/assets/16586200/12c763cd-bead-4923-b610-8788f388fcb5)

3. После создания репозитория создайте связанный с ним GitHub Codespace.
![Создать codespace](https://user-images.githubusercontent.com/5889006/156916672-43b7b6e9-4ffb-4704-b4ba-d5ca40ffcae7.png)

4. Готово! Codespace настроен с последней версией Hugo Extended, просто запустите `hugo server` в терминале и посмотрите ваш новый сайт в действии.

5. Проверьте папку `config` для файлов конфигурации. Вы можете отредактировать их под свои нужды. Обязательно обновите свойство `baseurl` в файле `config/_default/config.toml` на URL вашего сайта.

# Создание контента

## Статическая страница
hugo new content/page-name/index.md

## Статья блога
hugo new content/post/post-name/index.md

# Синтаксис и примеры
https://example.com/help/