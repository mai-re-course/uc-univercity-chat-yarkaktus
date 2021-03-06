# Приглашение пользователя с помощью СМС

**Акторы:**

- пользователь
- мобильное приложение
- бекенд

**Цель:**
Пользователь(студент) хочет пригласить своего друга(студента) в мобильное приложение для общения по учебе.

**Предусловия:**
- у пользователя установлено мобильное приложение
- пользователь зарегистрирован в приложении
- у пользователя в контактах его мобильного телефона добавлен контакт друга, которого он хочет пригласить в приложение

**Сценарий:**

1. Пользователь открывает приложение
2. Нажимает на кнопку "Действия" (три палочки).
3. Нажимает кнопку "Пригласить друзей". Открывается поле для ввода e-mail и список контактов пользователя.
4. В открывшемся списке контактов выбирает контакт человека, которого хочет пригласить. Появляется кнопка с зеленой галочкой.
5. Для подтверждения выбранного контакта пользователь нажимает зеленую галочку.

**Результат:**

- Бекенд обрабатывает запрос на приглашение пользователя и формирует запрос к смс-провайдеру
- Выбранному пользователем контакту отправляется смс с текстом приглашения, ссылкой и ФИО пригласившего.

**Исключения:**

3.1. У пользователя запрещен доступ к контактам. Вызов системного диалогового окна на запрос доступа к контактам пользователя.

5.1. Отсутствие интернета на мобильном устройстве. Всплывающее окно с уведомлением пользователя об отключенном интернет-соединении.