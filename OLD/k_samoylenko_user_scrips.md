# Самойленко Кирилл - "Бот для покупок кроссовок - CopGod"
# Пользовательские сценарии
	
### Группа: 10 - МИ - 1
### Электронная почта: samoylenkk@inbox.ru
### VK: https://vk.com/owbl6ka

### [ Сценарий 1 - Регистрация пользователя ]
	
1. Пользователь вводит логин, с которым он будет заходить в систему.
2. Пользователь вводит пароль, с которым он будет заходить в систему.
3. Пользователь вводит адрес электронной почты, который будет использоваться в системе.
4. Если выбранный логин уже существует в системе, то пользователю сообщается об этом и предлагается придумать новый логин.
5. Если второй логин уже занят, система даёт рекомендации по придумыванию уникального логина.
6. Если пароль содержит менее 6 символов, система сообщает, что пароль должен быть от 6 до 30 символов и пользователь должен придумать новый пароль.
7. Если введённый адрес электронной почты не соответствует формату, то система выводит сообщение об ошибке и просит ввести адрес ещё раз.
8. Если все введённые данные соответствуют требованиям регистрации, то система отправляет на почту письмо для подтверждения почты.
9. После подтверждения имейла система приветствует пользователя и переходит в диалог выбора режима работы и тарифного плана.
10. Запускается Сценарий 2 - Создание профиля.
	
	
### [ Сценарий 2 - Создание профиля ]
	
1. Пользователь дает название новому профилю.
2. Пользователь заполняет первый пункт профиля: "Customer Information": Имя, Фамилия, Почта, Номер Телефона.
3. Далее пользователь заполняет второй пункт: "Shipping Address": Страна, Город, Область(Если есть), Улица, Дом, Корпус/ Строение(Если есть), Квартира, Почтовый индекс.
4. Теперь пользователь заполняет третий пункт: "Payment Metod": Номер карты, Имя на карте, Срок годности(месяц/год), CVV.
5. Если Адрес доставки соответствует адресу выставление счета, пользователь отмечает галочку напротив Адреса выставления.
6. Иначе Пользователь заполняет четвертый пункт: "Billing address": Имя, Фамилия, Адрес доставки, Квартира, Город, Страна, Штат/Регион, Почтовый индекс, Номер телефона. 
7. Пользователь нажимает на кнопку: "Save".
	
### [ Сценарий 3 - Мониторинг рестоков ]
	
1. Пользователь выбирает сайт, на котором будет бот будет мониторить рестоки, из доступных в списке.
2. Добавляет ключевые слова, по которому бот будет понимать, какую вещь искать.
3. Как только вещь появляется на сайте, бот автоматически информирует уведомлением пользователя, что происходит ресток, вещи которая подходит под ключевые слова.
4. Бот добавляет предмет в корзину и производит чекаут( информация о том, какое действие проходит, транслируется в статусе задачи).
5. Если для совершения покупки нужно пройти капчу, бот выводит в отдельное окошко капчу и предлагает пользователю пройти ее.
5. Бот закрывает задачу и предлагает перейти на почту(если покупка прошла успешна), чтобы посмотреть заказ.
6. Пользователь нажимает на кнопку: "Save".
	
### [ Сценарий 4 - Создание задачи ]
	
1. Пользователь нажимает на кнопку: "Add task".
2. Дальше пользователь выбирает режим задачи: отложенная покупка(запускается сценарий: Отложенная покупка) или создание задачи.
2. Пользователь выбирает сайт.
3. Затем вещь( или если таковой нет, но она будет представлена на сайте, ставит галочку и пишет ключевые слова, по которым бот, должен будет найти вещь на сайте).
4. Дальше размер(также можно выбрать random, и бот купит тот размер, который будет).
5. Затем использовать прокси или нет.
6. Пользователь нажимает кнопку: "Save". 
	
	
### [ Сценарий 5 - Отложенная покупка]
	
1. Пользователь выбирает сайт.
2. Выбирает вещь( или если таковой нет, но она будет представлена на сайте, ставит галочку и пишет ключевые слова, по которым бот, должен будет найти вещь на сайте).
3. Выбирает размер(также можно выбрать random, и бот купит тот размер, который будет).
4. Выбирает использовать прокси или нет.
5. Выбирает время, когда бот должен будет взять вещь.
6. Пользователь нажимает кнопку: "Save". 
	
### [ Сценарий 6 - Просмотр календаря релизов и уведомление о релизах]
	
1. Пользователь заходит во вкладку «Release calendar».
2. Пользователь может просматривать календарь, если ему понравился какой либо релиз, он нажимает на него.
3. В следующем окне предоставляется доступная информация о релизе: Цена, Кол-во пар, Магазины, в которых будет доступен релиз и как будет происходить продажа.
4. Пользователь может выбрать будет ли бот уведомлять о релизе или нет.
5. Пользователь выбирает за какое время он будет уведомлен о продаже.
6. Бот также предлагает создать задачу( если пользователь соглашается, то запускается сценарий: Отложенная покупка).

### [ Сценарий 7 - Запуск/Отмена всех задач сразу ]
	
1. Пользователь выбирает запусть ему все задачи или прекратить выполнение всех задач.
2. Если пользователь нажимает на кнопку: "Start All Tasks" .
3. Бот начинает выполнение всех задач.
4. Если пользоватль нажимает на кнопку: "Stop All Tasks" .
5. Бот спрашивает точно ли пользователь хочет отменить все задачи или нет.
6. Если пользователь нажимает на да, то бот прекращает выполнять все задачи.
7. Иначе бот продолжит выполнять поставленные задачи.

	
### [ Сценарий 8 - Запуск/Отмена задачи].
	
1. Если Пользователь жмет на кнопку «Start task».
2. Бот заходит на сайт.
3. Добавляет предмет в корзину и производит чекаут( информация о том, какое действие проходит, транслируется в статусе задачи).
4. Если для совершения покупки нужно пройти капчу, бот выводит в отдельное окошко капчу и предлагает пользователю пройти ее.
5. Бот закрывает задачу и предлагает перейти на почту(если покупка прошла успешна), чтобы посмотреть заказ.
6. Если пользователь нажимает на кнопку "Stop task".
7. Бот прекращает процесс покупки вещи.
8. Предлагает пользователю удалить задачу.


### [ Запрос на добавление нового сайта].

1. Пользователь жмет на кнопку «place the request».
2. Пользователь заполняет запрос на добавление нового сайта(сайт, ссылку на него, почему его нужно добавить, свои контактные данные).
3. Пользователь предлагают перепроверить заполненную информацию
4. Если пользователь нажимайт на кнопку «Send».
5. Запрос направляется на рассмотрение 
6. Если мы видим, что на этот сайт поступило достаточно большое кол-во запросов на добавление, начинается настройка бота под данный сайт
7. После разработки, делается рассылка, что бот теперь готов работать на этом сайте.


