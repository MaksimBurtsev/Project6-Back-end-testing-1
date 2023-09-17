# Задание №3. Коды ответов

 1. 
 ```
 [
    {
        "name": "Малышева Екатерина Матвеевна",
        "birthday": "1995-06-01",
        "post": "Бухгалтер"
    },
    {
        "name": "Капустин Роман Артёмович",
        "birthday": "1991-01-18",
        "post": "Финансовый аналитик"
    },
    {
        "name": "Касьянов Ярослав Ярославович",
        "birthday": "1989-07-29",
        "post": "Кредитный эксперт"
    },
    {
        "name": "Белова Елизавета Руслановна",
        "birthday": "1997-04-13",
        "post": "Аудитор"
    },
    {
        "name": "Романов Константин Александрович",
        "birthday": "2001-12-14",
        "post": "Кассир"
    },
    ...
]
 ```
 При обращении к эндпоинту /employees методом GET будет возвращен ответ с кодом статуса **200 (OK)**
___
 2. 
 ```
 {
  "message": "Неверные данные для авторизации."
  }
``` 
 При обращении к эндпоинту /login методом GET будет возвращен ответ с кодом статуса **401 (Unauthorized)**
___
 3. 
 ```
 {
  "message": "Неверно составлен запрос."
  }
``` 
При обращении к эндпоинту /data методом GET будет возвращен ответ с кодом статуса **400 (Bad Request)**
___
 
**Код ответа 201 (Created)** является одним из кодов ответов HTTP, который используется для обозначения успешного создания ресурса на сервере. Это означает, что сервер успешно получил и обработал запрос от клиента и создал новый ресурс, в соответствии с информацией, предоставленной клиентом.

Код 201 может использоваться для различных запросов, которые создают новые ресурсы на сервере. Например, POST-запрос может использоваться для создания новых записей в базе данных, PUT-запрос может обновлять существующие записи, а PATCH-запрос может частично обновлять записи. Все эти запросы могут вернуть код ответа 201.

Код 201 также используется в паре с заголовками ответа, такими как Location, которые указывают, где находится созданный ресурс. Это может помочь клиенту быстро найти новый ресурс и начать взаимодействовать с ним.

**Однако, следует отметить,** что код 201 не должен использоваться с методом GET. GET-запросы используются для получения информации из существующих ресурсов и должны возвращать **код 200 (OK)** в случае успешного выполнения. Все остальные методы, которые создают или обновляют ресурсы, могут использовать код 201.
___
**Код ответа 400 (Bad Request)** - это один из стандартных кодов ошибок HTTP. Он указывает на то, что запрос клиента не может быть обработан сервером из-за неверного формата, некорректных параметров или других проблем, связанных с запросом. Когда клиент отправляет GET-запрос на сервер, код 400 может быть возвращен в случае, если параметры запроса некорректны или отсутствуют обязательные параметры. Например, если запрос ожидает ID ресурса, а клиент отправил запрос без ID, сервер может вернуть код 400.Код 400 также может быть возвращен в случае, если значение параметра не соответствует ожидаемому формату. Например, сервер может ожидать, что в параметрах запроса будет дата в формате "гггг-мм-дд", а клиент отправил дату в формате "дд-мм-гггг". В таком случае сервер может вернуть код 400, чтобы сообщить об ошибке. Код 400 может также указывать на ошибку валидации данных. Например, если сервер ожидает значения в определенном диапазоне или формате, а клиент отправляет некорректные данные, сервер может вернуть код 400. Если в ответ на запрос возвратился код 400, клиент должен проверить параметры запроса и переданные данные, чтобы устранить возможную ошибку. Клиент также может получить дополнительную информацию об ошибке, которая может быть возвращена в теле ответа или в заголовках ответа. В целом, код ответа 400 является одним из самых распространенных кодов ошибки и может быть возвращен в различных контекстах, поэтому важно обращать внимание на детали запроса и корректность введенных данных, чтобы избежать ошибок, связанных с кодом 400.
___
**Код ответа 500 (Internal Server Error)** является одним из наиболее распространенных и серьезных кодов ошибок HTTP. Он указывает на то, что сервер внутренне не может обработать запрос, что может привести к неработоспособности сайта или приложения, а также потере данных.

Причины появления ошибки 500 могут быть различными. Например, это может быть вызвано ошибкой в коде приложения или нехваткой ресурсов, таких как вычислительная мощность или память. Ошибка 500 может также означать, что сервер столкнулся с проблемой базы данных, что может быть вызвано неправильно настроенными параметрами подключения или ошибками в самой базе данных.

Если пользователь сталкивается с ошибкой 500 на сайте, то ему необходимо обратиться к администратору сайта или технической поддержке. Рекомендуется также провести проверку своего интернет-соединения и повторить попытку позже. 

Как правило, ошибка 500 не является проблемой со стороны клиента и не связана с запросом, который был отправлен на сервер. Код ответа 500 требует немедленного решения, направленного на выявление и устранение причины ошибки.  В некоторых случаях для исправления проблемы может потребоваться вмешательство профессионалов, таких как разработчики или инженеры, для того чтобы вернуть функциональность сайта или приложения.

