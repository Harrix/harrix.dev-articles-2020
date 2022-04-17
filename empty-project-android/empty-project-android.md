---
date: 2020-05-06
categories: [it, programming]
tags: [Android Studio, Android, Java]
related-id: start-java
---

# Болванка приложения на Android Studio

В статье рассказывается как создать простую болванку на Android Studio 4.0.

Так как Android Studio часто меняет внешний вид своего приложения, то, чтобы не менять всякий раз в статьях описание создания болванки приложения, то подготовил вот эту статью.

## Приготовления

В статье [Установка Android Studio в Windows](https://github.com/Harrix/harrix.dev-blog-2019/blob/main/2019-07-16-install-android-studio/2019-07-16-install-android-studio.md) узнаете, как установить и настроить Android Studio.

## Создание проекта

Когда открывается Android Studio вас будет ждать такое окно (если до этого уже создавался проект):

![Создание нового проекта](img/new-project_01.png)

Или будет такое окно, если, например, Android Studio открывается впервые:

![Создание нового проекта](img/new-project_02.png)

Выбираем шаблон пустой активности:

![Выбор шаблона активности](img/new-project_03.png)

Выбираем название проекта, его расположение, язык, на котором будет идти программирование, и минимальную версию Android для запуска приложения:

![Выбор настроек проекта](img/new-project_04.png)

После этого будет создан проект приложения:

![Готовый проект в Android Studio](img/new-project_05.png)

## Разметка внешнего вида

Перейдем вначале к файлу `activity_main.xml`, который отвечает за разметку внешнего вида приложения:

![Переход к activity_main.xml](img/new-project_06.png)

По умолчанию в Android Studio в качестве разметки используется контейнер `ConstraintLayout`. Для новичков он не совсем простой. Поменяем на обычный `LinearLayout`.

Перейдем в текстовой режим разметки XML файла:

![Переход к текстовому отображению activity_main.xml](img/new-project_07.png)

Там мы внутри контейнера `ConstraintLayout` видим элемент `TextView` с фразой `Hello, World!`:

![Текущее содержимое файла activity_main.xml](img/new-project_08.png)

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

Болванка приложения готова.
