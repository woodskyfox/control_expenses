# control_expenses
control_expenses.py - приложение контроль расходов.

Инструменты которые использовались при написании приложения: Python 3.9.5, mysql  Ver 8.0.26 .

Чтоб использовать приложение control_expenses.py у вас должен быть установлен Python3 последней версии и MySQL последней версии.

Скачать эти программы:
Python3 - https://www.python.org .
MySQL - https://www.mysql.com .

ЗАПУСК ПРОЛОЖЕНИЯ control_expenses.py:

1. Зарегистрируйтесь в MySQL как root пользователь. (Запомните или запишите пароль).
Пароль root пользователя базы данных MySQL будет использоваться только при регистрации нового пользователя приложения control_expenses.py .
Чтоб дать ему права доступа только к своей базе данных под совим именем user_name.
База данных пользователя user_name будет создана с таким же именем как и имя пользователя (user_name)

2. Вам нужно установить Connector/Python для соединения python с MySQl
   
   Для большинства операционных систем команда: 
   
   			pip install mysql-connector-python .

   Оригинальный документ: https://dev.mysql.com/doc/connector-python/en/connector-python-installation-binary.html

3. Запустите файл control_expenses.py с помощюь python3.
Вы увидите в консоли:


			Контроль расходов:

			Главное меню:

			0 - Выйти из программы (Exit)
			1 - Войти (Log in)
			2 - Создать пользователя (Sing up)
			
		Ваш выбор: 

В строку "Ваш выбор:" вводятся цифры с меню 
(например: если вы хотите Создать пользователь нужно ввести цифру 2 и нажать Enter).

4. При создании пользователя вам нужно будет ввести пароль root пользователя MySQL из пункта 1. 
Потом ввести имя которое вы выбрали для пользователя и пароль. 
Пароль нужно будет ввести два раза для правильности.
Пароль root пользователя базы данных MySQL будет использоваться только при регистрации нового пользователя приложения.
Чтоб дать ему права доступа только к своей базе данных под совим именем user_name.
База данных пользователя user_name будет создана с таким же именем как и имя пользователя (user_name)

Пример:

			Пароль root пользователя: password
			Введите имя пользователя: user_name
			Введите парлоль для пользователя user_name : password
			Введите для проверки пароль пользователя user_name : password

После этого будет сообщение про успех и приложение выйдет в главне меню.
Пример:

			Поздравляем: пользователь user_name создан!
			Для создание контроля расходов
			выполните вход (1 - Log in) под своим иминем и парлолем

			Контроль расходов:

			Главное меню:

			0 - Выйти из программы (Exit)
			1 - Войти (Log in)
			2 - Создать пользователя (Sing up)

		Ваш выбор: 

5. Ввойдите в приложение (введите цифру - 1) в строку "Ваш выбор: 1" и нажмите Enter.

			Вы вошли как пользователь: user_name

			Контроль расходов:

			Меню пользователя: 

			0 - Выйти (Log out)
			1 - Внести расход
			2 - Статистика расходов
			3 - Удалить данные
	
		Ваш выбор:

6. В "Меню пользователя" Если захотите ввести расход введите цифру - 1, 
просмотреть статистику расходов введите цифру - 2, 
удалить расходы введите цифру - 3 и нажмите Enter.

7. В пункте "1 - Внести расход" расходы можно вносить за сегодняшнее число 
(приложение вводит число автоматически) и за лобое число выбранное вами.
Примечание: при выборе пункта "2 - Внести расход и внести дату"
Придержуйтесь правильного форматф (формат: ГГГГ-ММ-ДД)
Например: 2021-10-11 
Сначала идет год, потом месяц, потом день. Обязательно ставте дефисы.

			Вы вошли как пользователь: user_name

			Контроль расходов:

			Меню пользователя -> Внести расход:

			0 - Выйти в меню пользователя
			1 - Внести расход за сегодня
			2 - Внести расход и внести дату

		Ваш выбор: 


8. В пункте "2 - Статистика расходов" можно просмотреть всю статистику расходов, 
Статистику по конкретной категории и статистику расходов по дате.
Примечание: при выборе пункта "3 - Статистика по дате"
Придержуйтесь правильного форматф (формат: ГГГГ-ММ-ДД)
Например: 2021-10-11

			Вы вошли как пользователь: user_name

			Контроль расходов:

			Меню пользователя -> Статистика расходов: 

			0 - Выйти в меню пользователя
			1 - Статистика по всем категориям
			2 - Статистика по названию категории
			3 - Статистика по дате

		Ваш выбор: 



			Вы вошли как пользователь: user_name

			Контроль расходов:

			Меню пользователя -> Статистика расходов ->
			-> Статистика расходов по дате: 

			0 - Выйти в статистику расходов
			1 - Статистика полная дата (формат: ГГГГ-ММ-ДД)
			2 - Статистика за день (формат: ДД)
			3 - Статистика за месяц (формат: ММ)
			4 - Статистика за год (формат: ГГГГ)
				
		Ваш выбор: 
9. В пункте "3 - Удалить данные" удаляются все внесенные вами расходы.
			
			Вы вошли как пользователь: user_name

			Контроль расходов:

			Меню пользователя -> Удалить данные:

			0 - Выйти в меню пользователя
			1 - Да (Yes)
			2 - Нет (No)
			
		Вы хотите удалить все ваши дынные?:
		
10. Что бы выйти из любого меню в предыдущее меню введите - 0 (ноль) и нажмите Enter. Выход с главного меню выходит с приложения и разлогинивает пользователя.


