# Изменение статуса пользователя

**Акторы:**

- пользователь
- мобильное приложение
- бекенд
- администратор бекенда

**Цель:**
Пользователь(студент) хочет отредактировать текст статуса, отображаемого в его профиле

**Предусловия:**
- у пользователя установлено мобильное приложение
- пользователь зарегистрирован в приложении

**Сценарий:**

1. Пользователь открывает приложение
2. Нажимает на кнопку "Меню" (три палочки).
3. Нажимает на значок карандаша. Открывается всплывающее окно с полем для ввода статуса. В поле отображается текущий статус.
4. Пользователь редактирует текст в поле.
5. Для сохранения введенного текста пользователь нажимает кнопку "ОК".

**Результат:**

- Бекенд сохраняет текст статуса, введенного пользователем.
- На странице профиля пользователя изменяется статус.

**Исключения:**

4.1. Пользователь ввел превышенное количество символов. Мобильное приложение подсвечивает красным поле для ввода статуса. Под полем для ввода появляется сообщение об ошибке.

4.2. Пользователь ввел одно или более слов, которые администратор указал как запрещенные. Мобильное приложение подсвечивает красным поле для ввода электронного адреса. Под полем для ввода появляется сообщение об ошибке.

5.1. Отсутствие интернета на мобильном устройстве. Всплывающее окно с уведомлением пользователя об отключенном интернет-соединении.

**Альтернативный сценарий:** 

4. Пользователь передумал изменять статус. Нажимает кнопку "Назад" и попадает на главную страницу приложения. Текст статуса не изменяется.
