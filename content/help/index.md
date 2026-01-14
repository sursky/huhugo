---
title: Help
description: Добро пожаловать, это тестовая страница
readingTime: false
math: true
image: cover.jpg
categories:
    # - Example Category
tags:
    # - Example Tag

sitemap:
  disable: true

# Черновик? true=в разработке, false=опубликовано
draft: false

type: "page"
---
Для получения дополнительной информации об этой теме, ознакомьтесь с документацией: https://stack.jimmycai.com/

Тема Hugo Stack поддерживает создание интерактивных галерей изображений с использованием Markdown. Она работает на основе [PhotoSwipe](https://photoswipe.com/).

Чтобы использовать эту функцию, изображение должно находиться в той же директории, что и файл Markdown, так как используется возможность Hugo использовать page bundle для чтения размеров изображений. 

**Внешние изображения не поддерживаются.**

# Галерея изображений

## Синтаксис

```markdown
![Изображение 1](1.jpg) ![Изображение 2](2.jpg)
```

## Результат

![Изображение 1](1.jpg) ![Изображение 2](2.jpg)

> Фото от [mymind](https://unsplash.com/@mymind) и [Luke Chesser](https://unsplash.com/@lukechesser) на [Unsplash](https://unsplash.com/)

# Синтаксис Markdown

## Заголовки

HTML-элементы `<h1>`—`<h6>` представляют шесть уровней заголовков секций. `<h1>` — это самый высокий уровень секции, а `<h6>` — самый низкий.

# H1
## H2
### H3
#### H4
##### H5
###### H6

## Цитаты

### Цитата без указания авторства

> Tiam, ad mint andaepu dandae nostion secatur sequo quae.
> **Примечание**, что вы можете использовать *синтаксис Markdown* внутри цитаты.

### Цитата с указанием авторства

> Не общайтесь, деля память, делите память, общаясь.<br>
> — <cite>Роб Пайк[^1]</cite>

[1]: Приведенная выше цитата взята из [выступления](https://www.youtube.com/watch?v=PAAkCSZUG1c) Роба Пайка во время Gopherfest, 18 ноября 2015 года.

## Таблицы

Таблицы не являются частью спецификации Markdown, но Hugo поддерживает их из коробки.

| Имя | Возраст |
|--------|------|
| Боб | 27 |
| Алиса | 23 |

### Встроенный Markdown в таблицах

| Курсив | Жирный | Код |
|--------|--------|-----|
| *курсив* | **жирный** | `код` |

| Italics   | Bold     | Code   |
| --------  | -------- | ------ |
| *italics* | **bold** | `code` |

| A                                                        | B                                                                                                             | C                                                                                                                                    | D                                                 | E                                                          | F                                                                    |
|----------------------------------------------------------|---------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------|------------------------------------------------------------|----------------------------------------------------------------------|
| Lorem ipsum dolor sit amet, consectetur adipiscing elit. | Phasellus ultricies, sapien non euismod aliquam, dui ligula tincidunt odio, at accumsan nulla sapien eget ex. | Proin eleifend dictum ipsum, non euismod ipsum pulvinar et. Vivamus sollicitudin, quam in pulvinar aliquam, metus elit pretium purus | Proin sit amet velit nec enim imperdiet vehicula. | Ut bibendum vestibulum quam, eu egestas turpis gravida nec | Sed scelerisque nec turpis vel viverra. Vivamus vitae pretium sapien |

## Блоки кода

### Блок кода с обратными апострофами

```html
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Example HTML5 Document</title>
</head>
<body>
  <p>Test</p>
</body>
</html>
```

### Блок кода с отступом в четыре пробела

    <!doctype html>
    <html lang="en">
    <head>
      <meta charset="utf-8">
      <title>Example HTML5 Document</title>
    </head>
    <body>
      <p>Test</p>
    </body>
    </html>

### Блок кода с разницей (diff)

```diff
[dependencies.bevy]
git = "https://github.com/bevyengine/bevy"
rev = "11f52b8c72fc3a568e8bb4a4cd1f3eb025ac2e13"
- features = ["dynamic"]
+ features = ["jpeg", "dynamic"]
```

### Однострочный блок кода

```html
<p>A paragraph</p>
```

## Типы списков

### Нумерованный список

1. Первый элемент
2. Второй элемент
3. Третий элемент

### Маркированный список

* Элемент списка
* Еще один элемент
* И еще один элемент

### Вложенный список

* Фрукты
 * Яблоко
  * Апельсин
  * Банан
* Молочные продукты
  * Молоко
  * Сыр

## Другие элементы — аббревиатуры, нижние и верхние индексы, клавиши, выделение

<abbr title="Graphics Interchange Format">GIF</abbr> — это формат растровых изображений.

H<sub>2</sub>O

X<sup>n</sup> + Y<sup>n</sup> = Z<sup>n</sup>

Нажмите <kbd>CTRL</kbd> + <kbd>ALT</kbd> + <kbd>Delete</kbd>, чтобы завершить сеанс.

Большинство <mark>salamanders</mark> ведут ночной образ жизни и охотятся за насекомыми, червями и другими мелкими существами.

# Математическая типографика

Stack имеет встроенную поддержку математической типографики с использованием [KaTeX](https://katex.org/).

## Встроенные математические выражения

Это встроенное математическое выражение: $\varphi = \dfrac{1+\sqrt5}{2}= 1.6180339887…$

```markdown
$\varphi = \dfrac{1+\sqrt5}{2}= 1.6180339887…$
```

## Блочные математические выражения

$$
    \varphi = 1+\frac{1} {1+\frac{1} {1+\frac{1} {1+\cdots} } } 
$$

```markdown
$$
    \varphi = 1+\frac{1} {1+\frac{1} {1+\frac{1} {1+\cdots} } } 
$$
```

$$
    f(x) = \int_{-\infty}^\infty\hat f(\xi)\,e^{2 \pi i \xi x}\,d\xi
$$

```markdown
$$
    f(x) = \int_{-\infty}^\infty\hat f(\xi)\,e^{2 \pi i \xi x}\,d\xi
$$
```

# Шорткоды

Для получения более подробной информации ознакомьтесь с [документацией](https://stack.jimmycai.com/writing/shortcodes).

## Видео с Rutube

{{< rutube "321d31f4787a5d8596a0996f95bd09f3" >}}

## Видео с YouTube

{{< youtube "0qwALOOvUik" >}}

## Обычный видео файл

{{< video "https://www.w3schools.com/tags/movie.mp4" >}}

## GitLab

{{< gitlab 2589724 >}}

## Цитата

{{< quote author="Знаменитый человек" source="Книга, которую они написали" url="https://en.wikipedia.org/wiki/Book">}}
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
{{< /quote >}}

-----

> Фото от [Codioful](https://unsplash.com/@codioful) на [Unsplash](https://unsplash.com/photos/WDSN62Qdxuk)