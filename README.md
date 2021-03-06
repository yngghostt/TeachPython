## Идея бота
Бот, презназначенный для обучения языку Python. Возможно изменение функционала под обучение любой дисциплине. Курсы представляют из себя набор коротких сообщений с картинками или без.

## Реализация бота
Бот написан на языке Python с использованием библиотеки *PyTeleBot*. Для реализации базы данных использована библиотека *SQLAlchemy*. Для создания курса используется библиотека *pandas*, которая позволяет хранить курсы в формате таблицы.

## Хранение данных о пользователе
В базе данных хранится только id и соответствующий ему уровень прогресса.

## Хранение курса
Курс хранится в таблице excel в формате дерева - для каждого ответа записан следующий (или следующие) за ним. За это отвечает столбец next. Поддерживается отправка картинок (для этого картинка должна иметь имя, совпадающее с прогрессом по курсу). Картинка ищется, если для соответствующего сообщения в столбце picture содержатся какие-то данные. Кроме того, поддерживается система тестирования в формате "вопрос - ответ". Для этого в графе "answer" должен быть записан правильный ответ. Кроме того, необходимо задать ответы на правильный и неправильный ответ. Название i-того курса хранится в ячейке с уровнем прогресса i.0.0.
## ![image](https://user-images.githubusercontent.com/52496357/120472477-9a934280-c3ae-11eb-87f2-63e15c08771a.png)

## Команды
Бот поддерживает команды /start и /help. При первом вызове команды /start в базу даных записывается id пользователя и выдается меню. При вызове команды /help выводится сообщение с информацией о боте.

## Интерфейс бота
Интерфейс бота представлен на картинках ниже.

## ![image](https://user-images.githubusercontent.com/52496357/120659561-27adc880-c48f-11eb-9fbd-10ce6785cdc9.png)
## ![image](https://user-images.githubusercontent.com/52496357/120659593-309e9a00-c48f-11eb-82a6-f2807dbac449.png)


## Интерфейс инлайн-тестов
Бот поддерживает набор инлайн-тестов. Они хранятся в отедльной excel-таблице по тем же правилам. Интерфейс представлен на картинке.
## ![image](https://user-images.githubusercontent.com/52496357/120659463-0fd64480-c48f-11eb-9932-2ed3c831dfff.png)

## ![image](https://user-images.githubusercontent.com/52496357/120659515-1e246080-c48f-11eb-8fae-979865987ec9.png)
