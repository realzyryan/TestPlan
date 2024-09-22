# План автоматизации тестирования сценария перехода к форме записи на обучение профессии "Инженер по тестированию" и заполнения этой формы

### 1. Перечень автоматизируемых сценариев:

<details>
   <summary>1. Переход на страницу курса "Инженер по тестированию" с главной страницы сайта Нетология</summary>

##### 1.1. Переход к форме записи на курс "Инженер по тестированию" по кнопке "Каталог курсов"
1. открыть страницу сайта ["Нетология"](https://netology.ru/)
2. в верху сайта нажать на кнопку "Каталог курсов"
3. в открывшемся списке найти "Программирование"
4. нажать в появившемся списке на кнопку "Инженер по тестированию"
5. проскролить вниз до формы записи на курс

Ожидаемый результат: переход на страницу курса "Инженер по тестированию" для заполнения формы на обучение

##### 1.2. Переход к форме записи на курс "Инженер по тестированию" через раздел "Направления обучения"
1. открыть страницу сайта ["Нетология"](https://netology.ru/)
2. проскролить страницу вниз и найти раздел направления обучения
3. выбрать направление "Программирование"
4. на открывшейся странице в списке найти раздел "Инженер по тестированию"

Ожидаемый результат: переход на страницу курса "Инженер по тестированию" для заполнения формы на обучение

#### 2.1. Заполнение формы записи по кнопке "Записаться" валидными данными
1. открыть страницу курса ["Инженер по тестированию"](https://netology.ru/programs/qa)
2. ввести в поля ввода "Имя", "Телефон", "Электронная почта" валидные данные
3. нажать на кнопку "Записаться"

Ожидаемый результат: появляется сообщение "Поздравляем! Вы успешно записались на курс"

#### 3.1. Отправка пустой формы записи
1. открыть страницу курса ["Инженер по тестированию"](https://netology.ru/programs/qa)
2. проскролить всю страницу курса до формы записи
3. не вводить никакие данные в поля ввода
4. нажать на кнопку "Записаться"

Ожидаемый результат: форма записи не отправляется, поля ввода выделяются красным цветом, под ними появляются сообщения "Обязательное поле"

<details>
   <summary>- поле ввода "Имя"</summary>

#### 3.1.1. Заполнение формы записи валидными данными, имя на кириллице
1. открыть страницу курса ["Инженер по тестированию"](https://netology.ru/programs/qa)
2. проскролить всю страницу курса до формы записи
3. ввести в поля ввода "Имя" валидные данные, например, "Мария"
4. ввести в поля ввода "Телефон" валидные данные (+ и 11 цифр), например, "+79220000000"
5. ввести в поля ввода "Электронная почта" валидные данные, например, "test@gmail.com"
6. нажать на кнопку "Записаться"

Ожидаемый результат: форма записи отправляется, появляется сообщение "Поздравляем! Вы успешно записались на курс"

#### 3.1.2. Заполнение формы записи валидными данными, имя на латинице
1. открыть страницу курса ["Инженер по тестированию"](https://netology.ru/programs/qa)
2. проскролить всю страницу курса до формы записи
3. ввести в поля ввода "Имя" валидные данные, например, "Evgeniy"
4. ввести в поля ввода "Телефон" валидные данные, например, "+79220000000"
5. ввести в поля ввода "Электронная почта" валидные данные, например, "test@gmail.com"
6. нажать на кнопку "Записаться"

Ожидаемый результат: форма записи отправляется, появляется сообщение "Поздравляем! Вы успешно записались на курс"

#### 3.1.3. Заполнение формы записи, пустой ввода поля "Имя"
1. открыть страницу курса ["Инженер по тестированию"](https://netology.ru/programs/qa)
2. проскролить всю страницу курса до формы записи
3. в поле "Имя" не вводить никакие данные
4. ввести в поля ввода "Телефон" валидные данные (+ и 11 цифр), например, "+79220000000"
5. ввести в поля ввода "Электронная почта" валидные данные, например, "test@gmail.com"
6. нажать на кнопку "Записаться"

Ожидаемый результат: форма записи не отправляется, поле ввода "Имя" выделяется красным цветом, под ним появляется сообщение "Обязательное поле"

#### 3.1.4. Заполнение формы записи не валидными данными, имя включает в себя символы
1. открыть страницу курса ["Инженер по тестированию"](https://netology.ru/programs/qa)
2. проскролить всю страницу курса до формы записи
3. ввести в поля ввода "Имя" не валидные данные, например, "Катя___123;%"
4. ввести в поля ввода "Телефон" валидные данные, например, "+79220000000"
5. ввести в поля ввода "Электронная почта" валидные данные, например, "test@gmail.com"
6. нажать на кнопку "Записаться"

Ожидаемый результат: форма записи не отправляется, поле ввода "Имя" выделяется красным цветом, под ним появляется сообщение "Имя должно состоять из букв"

</details>

<details>
   <summary>- поле ввода "Телефон"</summary>

#### 3.2.1. Заполнение формы записи валидными данными, формат телефона через 8
1. открыть страницу курса ["Инженер по тестированию"](https://netology.ru/programs/qa)
2. проскролить всю страницу курса до формы записи
3. ввести в поля ввода "Имя" валидные данные, например, "Мария Иванова"
4. ввести в поля ввода "Телефон" валидные данные (11 цифр начиная с 8), например, "89220000000"
5. ввести в поля ввода "Электронная почта" валидные данные, например, "test@gmail.com"
6. нажать на кнопку "Записаться"

Ожидаемый результат: форма записи отправляется, появляется сообщение "Поздравляем! Вы успешно записались на курс"

#### 3.2.2. Заполнение формы записи, поле "Телефон" пустое
1. открыть страницу курса ["Инженер по тестированию"](https://netology.ru/programs/qa)
2. проскролить всю страницу курса до формы записи
3. ввести в поля ввода "Имя" валидные данные, например, "Иванов Иван Иванович"
4. в поле "Телефон" не вводить никакие данные 
5. ввести в поля ввода "Электронная почта" валидные данные, например, "test@gmail.com"
6. нажать на кнопку "Записаться"

Ожидаемый результат: форма записи не отправляется, поле ввода "Телефон" выделяется красным цветом, под ним появляется сообщение "Обязательное поле"

#### 3.2.3. Заполнение формы записи не валидными данными, короткий номер телефона (10 цифр)
1. открыть страницу курса ["Инженер по тестированию"](https://netology.ru/programs/qa)
2. проскролить всю страницу курса до формы записи
3. ввести в поля ввода "Имя" валидные данные, например, "Александр"
4. ввести в поля ввода "Телефон" не валидные данные (+ и 10 цифр), например, "+9 (999) 999-99-9"
5. ввести в поля ввода "Электронная почта" валидные данные, например, "test@gmail.com"
6. нажать на кнопку "Записаться"

Ожидаемый результат: Предполагаю, что форма записи не отправляется, поле ввода "Телефон" выделяется красным цветом, под ним появляется сообщение "Неверный формат номера телефона"

#### 3.2.4. Заполнение формы записи не валидными данными, длинный номер телефона (15 цифр)
1. открыть страницу курса ["Инженер по тестированию"](https://netology.ru/programs/qa)
2. проскролить всю страницу курса до формы записи
3. ввести в поля ввода "Имя" валидные данные, например, "Александр"
4. ввести в поля ввода "Телефон" не валидные данные (15 цифр), например, "891200000000111"
5. ввести в поля ввода "Электронная почта" валидные данные, например, "test@gmail.com"
6. нажать на кнопку "Записаться"

Ожидаемый результат: форма записи не отправляется, поле ввода "Телефон" выделяется красным цветом, под ним появляется сообщение "Неверный формат номера телефона"

</details>

<details>
   <summary>- поле ввода "Электронная почта"</summary>

#### 3.3.1. Заполнение формы записи не валидными данными, в поле "Электронная почта" отсутствует символ @
1. открыть страницу курса ["Инженер по тестированию"](https://netology.ru/programs/qa)
2. проскролить всю страницу курса до формы записи
3. ввести в поля ввода "Имя" валидные данные, например, "Александр"
4. ввести в поля ввода "Телефон" валидные данные (11 цифр), например, "89120000000"
5. ввести в поля ввода "Электронная почта" не валидные данные, например, "testgmail.com"
6. нажать на кнопку "Записаться"

Ожидаемый результат: форма записи не отправляется, поле ввода "Электронная почта" выделяется красным цветом, под ним появляется сообщение "Неверный email"

#### 3.3.2. Заполнение формы записи не валидными данными, пустое поле "Электронная почта"
1. открыть страницу курса ["Инженер по тестированию"](https://netology.ru/programs/qa)
2. проскролить всю страницу курса до формы записи
3. ввести в поля ввода "Имя" валидные данные, например, "Александр"
4. ввести в поля ввода "Телефон" валидные данные (11 цифр), например, "89120000000"
5. не вводить в поле "Электронная почта" никаких данных
6. нажать на кнопку "Записаться"

Ожидаемый результат: форма записи не отправляется, поле ввода "Электронная почта" выделяется красным цветом, под ним появляется сообщение "Обязательное поле"

#### 3.3.3. Заполнение формы записи не валидными данными, поле ввода "Электронная почта" состоит из символов
1. открыть страницу курса ["Инженер по тестированию"](https://netology.ru/programs/qa)
2. проскролить всю страницу курса до формы записи
3. ввести в поля ввода "Имя" валидные данные, например, "Александр"
4. ввести в поля ввода "Телефон" валидные данные (11 цифр), например, "89120000000"
5. ввести в поля ввода "Электронная почта" не валидные данные, например, "!%8%_)"
6. нажать на кнопку "Записаться"

Ожидаемый результат: форма записи не отправляется, поле ввода "Электронная почта" выделяется красным цветом, под ним появляется сообщение "Неверный email"

   </details>
   </details>
   
### 2. Перечень используемых инструментов с обоснованием выбора

- **Git** - система контроля версий (самая популярная)
- **GitHub** - веб-сервис для хостинга IT-проектов основанный на сестеме контроля версий Git (крупнейший, самый
  популярный)
- **JUnit5** - фреймворк для тестирования ПО на языке Java (наиболее удобный)
- **Java 11** - язык программирования (на ней разрабатываются большинство проектов)
- **Gradle** - система автоматической сборки, инструмент управления проектами (более гибкая и современная система сборки
  в сравнении в другими)
- **Selenide** - фреймворк для автоматизированного тестирования веб-приложений для поиска веб-элементов на странице (в
  отличие от Selenium не требует настройки окружения, установки специального драйвера)
- **JaCoCo** - плагин, использующий метрику, которая показывает насколько % код был покрыт автотестами (популярный)
- **Lombok** - библиотека для генерации кода (популярный инструмент, упрощает написание кода)
- **Faker** - библиотека, генератор данных (тестирование в широком диапазоне тестовых данных)
- **Appveyor** - веб-сервис непрерывной интеграции, предназначенный для сборки и тестирования программного обеспечения расположенного на GitHub (прост в настройке)
- **Allure** — фреймворк, предназначенный для создания визуально наглядной картины отчета о выполнении тестов. (наиболее распространен)

### 3. Перечень необходимых разрешений, данных и доступов
- разрешение на тестирование
- доступ к API сайта "Нетология"
- доступ к базе данных "Нетологии"

### 4. Перечень и описание возможных рисков при автоматизации

- отсутствие спецификации на работу приложения
- необходимость поддержки кода автотестов
- отсутствие тестов для проверки UA, кросплатформенного тестирования
- отсутствие нагрузочного тестирования, тестирования безопасности
- изменение верстки повлекут за собой неработоспособность автотестов

### 5. Перечень необходимых специалистов для автоматизации
- тестировщик ПО со знаниями языка программирования для написания автотестов
- системный администратор для обезличивания и предоставления базы данных "Нетологии"

### 6. Интервальная оценка с учётом рисков, в часах

40 часов