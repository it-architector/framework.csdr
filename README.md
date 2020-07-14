# CSDR среда

<h3>Предисловие</h3>

CSDR среда предназначена для визуального построения модульного кода в согласии с <a href="https://github.com/it-architector/right.csdr">порядком CSDR</a>.

![](./Картинки/1.4.jpg)

Так как порядок CSDR не готов, нижеперечисленный текст не является актуальным.

<h3>Навигация</h3>

1. <a href="#Среда">Среда</a>

     1.1. <a href="#Развёртка">Развёртка</a>
     
     1.2. <a href="#Области">Области</a>
     
     1.3. <a href="#Аутентификация">Аутентификация</a>
     
2. <a href="#Построение">Построение</a>

    2.1. <a href="#Действия">Планирование</a>

    2.2. <a href="#Действия">Действия</a>
    
    2.3. <a href="#Компиляция">Компиляция</a>
    
![---------------------](./Картинки/hr.png)

<h2>Среда</h2>

<h3>Развёртка</h3>

Среда сборки должна разворачиваться в виде программы на операционные системы: windows, mac и *nix.

<h3>Области</h3>

Для сборки модуля заданы такие области среды:
1. Аутентификация
2. Конструкции
3. Архитектура
4. Дизайн
5. Ход сборки

![](./Картинки/program/shablon1.png)

<h3>Аутентификация</h3>

Без авторизации все области заблокированы. Здесь будет форма для идентификации и получение прав доступа к областям.
    
![---------------------](./Картинки/hr.png)

<h2>Построение</h2>

<h3>Планирование</h3>

Для взаимодействия между областями нужны такие шаги: планирование конструкции → сделать → ознакомление → запланировано → делается  →  сделано / сделать.

> Где, планирование конструкции - постановка цели.
>
> Где, сделать - перевод цели в следующую область.
>
> Где, ознакомление - сбор данных, изучение дополнительных материалов.
>
> Где, запланировано - установка даты выполнения.
>
> Где, делается - выполнение.
>
> Где, сделано - цель выполнена.

В итоге получится такое планирование:

Область конструкции

1 → планирование конструкции

2 → сделать

Область архитектуры

3 → ознакомление

4 → запланировано

5 → делается

6 → сделать

Область дизайна

7 → ознакомление

8 → запланировано

9 → делается

10 → сделано

> При этом возможен реверс с комментарием, на случай недоработки:
> 1) ознакомление → планирование конструкции
> 2) делается  →  ознакомление
> 2) сделано  →  планирование конструкции

<h3>Действия</h3>

Под действиями будем считать манипуляции в таких областях: конструкции, архитектура и дизайн.

![](./Картинки/визуализация.jpg)

Изначально области архитектуры и дизайна недоступны, их открытие начинается после того как выбрали или создали проект. Как только это совершили, в области **проект** можно будет:
1. Задать название проекта
2. Определить тип проекта
3. Управлять конструкциями

В области **архитектуры**:
1. Управлять рефлексией

В области **дизайна**:
1. Управлять местом
2. Управлять связью
3. Управлять реакцией
4. Выбирать роли

![](./Картинки/roles.png) 

Каждые произведенные действия будут записываться в файл проекта, где у каждого действия будет отмечено:

1. **Тип действия**:

     1.1. Добавить
     
     1.2. Изменить
     
     1.3. Удалить
     
     1.4. Зафиксировать // чтобы убрать возможность удаления
     
     1.5. Разафиксировать
2. **Компонент**:

     1.1. Параметр

     1.2. Конструкция

     1.3. Рефлекс
     
     1.4. Место
     
     1.5. Связь
     
     1.6. Реакция

3. **Индификатор** //номер для компонента

4. **Значение** //значение для компонента согласно <a href="https://github.com/it-architector/code.csdr">коду CSDR</a>
     
5. **Авторство** // определение программиста
     
6. **Дата** // Дата совершенного действия

<h3>Компиляция</h3>

В области **хода сборки** можно увидеть не только лог ваших действий, но и создать структурированный код проекта кнопкой компиляции. В созданный код будут автоматически добавлены функции примененных в проекте ролей.

![](./Картинки/визуализация.jpg)

