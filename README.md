<img align="right" width="150" alt="logo" src="https://user-images.githubusercontent.com/5889006/190859553-5b229b4f-c476-4cbd-928f-890f5265ca4c.png">

# Шаблон-стартер для темы Hugo Stack

Это быстрый стартовый шаблон для [темы Hugo Stack](https://github.com/CaiJimmy/hugo-theme-stack). Он использует функцию [модулей Hugo](https://gohugo.io/hugo-modules/) для загрузки темы.

В комплекте поставляется базовая структура и конфигурация темы. Настроено действие GitHub для автоматического развертывания темы на публичной странице GitHub. Также есть задача cron для автоматического ежедневного обновления темы.

## Начало работы

1. Нажмите *Использовать этот шаблон* и создайте репозиторий с именем `<username>.github.io` на GitHub.
![Шаг 1](https://user-images.githubusercontent.com/5889006/156916624-20b2a784-f3a9-4718-aa5f-ce2a436b241f.png)

2. После создания репозитория создайте связанный с ним GitHub Codespace.
![Создать codespace](https://user-images.githubusercontent.com/5889006/156916672-43b7b6e9-4ffb-4704-b4ba-d5ca40ffcae7.png)

3. Готово! Codespace настроен с последней версией Hugo Extended, просто запустите `hugo server` в терминале и посмотрите ваш новый сайт в действии.

4. Проверьте папку `config` для файлов конфигурации. Вы можете отредактировать их под свои нужды. Обязательно обновите свойство `baseurl` в файле `config/_default/config.toml` на URL вашего сайта.

5. Откройте Settings -> Pages. Измените ветку сборки с `master` на `gh-pages`.
![Сборка](https://github.com/namanh11611/hugo-theme-stack-starter/assets/16586200/12c763cd-bead-4923-b610-8788f388fcb5)

6. После завершения редактирования сайта просто зафиксируйте изменения и отправьте их. Действие GitHub автоматически развернет сайт на связанной странице GitHub.
![Действие GitHub](https://user-images.githubusercontent.com/5889006/156916881-90b8bb9b-1925-4e60-9d7a-8026cda729bf.png)

---

Если вы не хотите использовать GitHub Codespace, вы также можете запустить этот шаблон на своем локальном компьютере. **Вам нужно установить Git, Go и Hugo Extended локально.**

## Обновление темы вручную

Выполните:

```bash
hugo mod get -u github.com/CaiJimmy/hugo-theme-stack/v3
hugo mod tidy
```

> Этот стартовый шаблон настроен с использованием версии `v3` темы. Из-за ограничений модуля Go, как только будет выпущена версия `v4` или выше, вам нужно будет обновить тему вручную. (Изменя файл `config/module.toml`)

## Развертывание на других хостингах статических страниц

Если вы хотите собрать этот сайт с использованием другого хостинга статических страниц, вы должны убедиться, что на машине установлен Go.

<details>
  <summary>Vercel</summary>
  
Вам нужно переопределить команду сборки для ручной установки Go:

```
amazon-linux-extras install golang1.11 && hugo --gc --minify
```

![](https://user-images.githubusercontent.com/5889006/156917172-01e4d418-3469-4ffb-97e4-a905d28b8424.png)

Если вы используете Node.js 20, вам нужно переопределить команду установки для ручной установки Go:

```
dnf install -y golang
```

![image](https://github.com/zhi-yi-huang/hugo-theme-stack-starter/assets/83860323/777c1109-dfc8-4893-9db7-1305ec027cf5)


Также убедитесь, что указана версия Hugo в переменной окружения `HUGO_VERSION` (используйте последнюю версию Hugo Extended):

![Переменная окружения](https://user-images.githubusercontent.com/5889006/156917212-afb7c70d-ab85-480f-8288-b15781a462c0.png)
</details>
