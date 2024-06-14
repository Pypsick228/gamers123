# Информация о геймерах
Привет! Мы создаем платформу для онлайн-игр и нам нужна помощь, чтобы хранить, обрабатывать, использовать информацию о наших геймерах. В этом году мы подкинем тебе для реализации несколько задач. И вот первая из них.  Не забывай каждый раз заглядывать в файл README.md - тут ты найдешь подробные требования и подсказки. 

## TASK 1. Доработка класса Gamer и реализация инструмента добавления данных пользователей
Мы уже создали класс Gamer. Он позволят обрабатывать следующую информацию о пользователях - имя, возраст и любимые игры. Эта информация будет выводится в качестве минипрезентации геймера и поможет завести ему новых друзей. Однако есть проблема - мы забыли добавить поля для его ника в играх и электронную почту... Сможешь помочь нашей команде с этой задачей? Тогда лови чек-лист задачи и подсказки! 

### Чек-лист TASK 1
 - [ ] Доработать класс Gamer - добавить поля **nickname** и **email**
 - [ ] Откорректировать сообщение минипрезентации так, чтобы в нем появились новые данные
 - [ ] Проверить работу кода **тестами Pytest**, которые мы подготовили, чтобы убедится, что код отвечает нашему запросу

## Про тесты

### Тесты с использованием Pytest
Мы написали тесты для автоматической проверки кода на соответствие требованиям:
-   `test_Задание_1_проверка_имени_и_возраста`: Проверяем, что в классе "Gamer" все еще есть атрибуты "name" и "age".
-   `test_Задание_2_добавить_nickname`: Проверяем, что в классе "Gamer" появился атрибут "nickname".
-   `test_Задание_3_добавить_email`: Проверяем, что в классе "Gamer" появился атрибут "email".
-   `test_Задание_4_изменить_сообщение`: Тестирует выведение информации для минипрезентации геймера.

## Подсказки

### Классы в Python

#### 1. Определение класса:
```python
class ИмяКласса:
    def __init__(self, параметры):
        # Конструктор класса
        self.поле1 = значение1
        self.поле2 = значение2
        # ...

    def метод(self, параметры):
        # Определение метода
        # ...

# Пример:
class Животное:
    def __init__(self, имя, возраст):
        self.имя = имя
        self.возраст = возраст

    def представиться(self):
        print(f"Привет, меня зовут {self.имя} и мне {self.возраст} лет.")
```
#### 2. Создание экземпляра класса:
```python
# Создание экземпляра класса
объект = ИмяКласса(аргументы)

# Пример:
кошка = Животное("Барсик", 3)
```
#### 3. Добавление полей в класс:
```python
# Добавление новых полей в класс
объект.новоеПоле = значение

# Пример:
кошка.цвет = "рыжий"
```
#### 4. Использование класса в проекте:
```python
# Использование методов и полей класса
объект.метод(аргументы)
значение = объект.поле

# Пример:
кошка.представиться()
print(кошка.цвет)
```