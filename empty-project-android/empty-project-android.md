---
date: 2020-05-06
categories: [it, programming]
tags: [Android Studio, Android, Java]
related-id: start-java
author: Anton Sergienko
author-email: anton.b.sergienko@gmail.com
license: CC BY 4.0
license-url: https://github.com/Harrix/harrix.dev/blob/main/LICENSE.md
permalink-source: https://github.com/Harrix/harrix.dev-articles-2020/blob/main/empty-project-android/empty-project-android.md
permalink: https://harrix.dev/ru/articles/2020/empty-project-android/
lang: ru
attribution:
  - { author: Google Inc., author-site: "https://developer.android.com/license", license: CC
        BY 2.5, license-url: "https://creativecommons.org/licenses/by/2.5/", permalink: "https://commons.wikimedia.org/wiki/File:Android_Studio_icon.svg", permalink-date: 2019-06-07, name: Android Studio icon.svg }
---

# Болванка приложения на Android Studio

![Featured image](featured-image.svg)

В статье рассказывается как создать простую болванку на Android Studio 4.0.

Так как Android Studio часто меняет внешний вид своего приложения, то, чтобы не менять всякий раз в статьях описание создания болванки приложения, то подготовил вот эту статью.

## Приготовления

В статье [Установка Android Studio в Windows](https://github.com/Harrix/harrix.dev-articles-2019/blob/main/install-android-studio/install-android-studio.md)<!-- https://harrix.dev/ru/articles/2019/install-android-studio/ --> узнаете, как установить и настроить Android Studio.

## Создание проекта

Когда открывается Android Studio вас будет ждать такое окно (если до этого уже создавался проект):

![Создание нового проекта](img/new-project_01.png)

_Рисунок 1 — Создание нового проекта_

Или будет такое окно, если, например, Android Studio открывается впервые:

![Создание нового проекта](img/new-project_02.png)

_Рисунок 2 — Создание нового проекта_

Выбираем шаблон пустой активности:

![Выбор шаблона активности](img/new-project_03.png)

_Рисунок 3 — Выбор шаблона активности_

Выбираем название проекта, его расположение, язык, на котором будет идти программирование, и минимальную версию Android для запуска приложения:

![Выбор настроек проекта](img/new-project_04.png)

_Рисунок 4 — Выбор настроек проекта_

После этого будет создан проект приложения:

![Готовый проект в Android Studio](img/new-project_05.png)

_Рисунок 5 — Готовый проект в Android Studio_

## Разметка внешнего вида

Перейдем вначале к файлу `activity_main.xml`, который отвечает за разметку внешнего вида приложения:

![Переход к activity_main.xml](img/new-project_06.png)

_Рисунок 6 — Переход к activity_main.xml_

По умолчанию в Android Studio в качестве разметки используется контейнер `ConstraintLayout`. Для новичков он не совсем простой. Поменяем на обычный `LinearLayout`.

Перейдем в текстовой режим разметки XML файла:

![Переход к текстовому отображению activity_main.xml](img/new-project_07.png)

_Рисунок 7 — Переход к текстовому отображению activity_main.xml_

Там мы внутри контейнера `ConstraintLayout` видим элемент `TextView` с фразой `Hello, World!`:

![Текущее содержимое файла activity_main.xml](img/new-project_08.png)

_Рисунок 8 — Текущее содержимое файла activity_main.xml_

И заменим содержимое всего файла на следующий код:

```xml
<?xml version="1.0" encoding="utf-8"?>
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:paddingLeft="16dp"
    android:paddingRight="16dp"
    android:orientation="vertical" >

</LinearLayout>
```

![Новое содержимое файла activity_main.xml](img/new-project_09.png)

_Рисунок 9 — Новое содержимое файла activity_main.xml_

Болванка приложения готова.
