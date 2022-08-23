# Домашнее задание для Netology.ru для курса Java Developer   
### Описание и инструкция к выполнению [здесь](https://github.com/netology-code/jd-homeworks/tree/master/jvm/README.md)

## Запуск программы
- После выполнение [исходного кода](/src/main/java/ru/netology/JvmExperience.java) получаем следующие графики:

![](/src/main/resources/Общий_График_куча.png)
![](/src/main/resources/Общий_График_metaspace.png)

- Сообщения в консоле IDEA: 

![](/src/main/resources/Idea.png)

## Анализ `Classes`

- Скачек после `11:23:13.629776: loaded 529 classes`:

![](/src/main/resources/1.Скачек_0.png)
![](/src/main/resources/1.Скачек_2.png)

- Скачек после выполнения `11:23:17.008224300: loaded 2117 classes`.

![](/src/main/resources/2.Скачек_2.png)

- Скачек после выполнения `11:23:20.160995200: loaded 869 classes`.

![](/src/main/resources/3.Скачек_2.png)

## Анализ `Heap(кучи)`

- После `11:23:20.008403500: loading org.springframework` и `11:23:20.160995200: loaded 869 classes` произошла чистка кучи и уменьшился максимальный размер кучи:

![](/src/main/resources/4.1Размер_кучи_после_чистки.png)

- Произошло добавление объектов `11:23:23.161676500: creating 5000000 objects` в кучу и расширение максимального размера

![](/src/main/resources/4.2Размер_кучи_после_добавления_объектов_1.png)

![](/src/main/resources/4.2Размер_кучи_после_добавления_объектов_2.png)

![](/src/main/resources/4.2Размер_кучи_после_добавления_объектов_3.png)


