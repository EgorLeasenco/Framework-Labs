Отчет по лабораторной работе №1: Основы HTTP
Задание №1: Анализ HTTP-запросов
1. Вход с неверными данными
при вводе неверных данных сервер ответил
Request URL: http://sandbox.usm.md/login/process.php Request Method: POST Status Code: 401 Unauthorized Remote Address: 193.226.64.170:80 Referrer Policy: strict-origin-when-cross-origin

Какой метод HTTP был использован для отправки запроса? был отправлен метод Post

Какие заголовки были отправлены в запросе? accept: / (Клиент готов принять любой тип содержимого от сервера.)

accept-encoding: gzip, deflate (Указывает, что клиент поддерживает сжатые ответы с использованием методов gzip или deflate.)

accept-language: en-US,en;q=0.9,ru;q=0.8 (Предпочтительные языки ответа: американский английский и русский.)

connection: keep-alive (Соединение должно оставаться открытым для возможных последующих запросов.)

content-length: 42 (Длина содержимого тела запроса в байтах, равная сумме длины параметров username и password.)

content-type: application/x-www-form-urlencoded; charset=UTF-8 (Тип содержимого: данные формы в URL-кодировке.)

host: sandbox.usm.md (Имя хоста, к которому отправлен запрос.)

origin: http://sandbox.usm.md (Источник запроса.)

referer: http://sandbox.usm.md/login/ (Ссылка на страницу, с которой был инициирован запрос.)

user-agent: Mozilla/5.0 (Linux; Android 6.0; Nexus 5 Build/MRA58N) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/129.0.0.0 Mobile Safari/537.36 (Информация о клиенте: браузер и операционная система, с которой был отправлен запрос.)

x-requested-with: XMLHttpRequest (Указывает, что запрос был отправлен с использованием AJAX.)

Какие параметры были отправлены в запросе?
username: admin1212 password: password121212

Какой код состояния был возвращен сервером?
Status Code: 401 Unauthorized

Какие заголовки были отправлены в ответе?
Response Headers (Заголовки ответа):
connection: keep-alive content-type: text/plain;charset=UTF-8 date: Wed, 09 Oct 2024 09:45:56 GMT server: nginx/1.24.0 (Ubuntu) transfer-encoding: chunked

Повторите шаги 3-5, введя верные данные для входа (username: admin, password: password).
Request URL: http://sandbox.usm.md/login/process.php Request Method: POST Status Code: 200 OK Remote Address: 193.226.64.170:80 Referrer Policy: strict-origin-when-cross-origin connection: keep-alive content-type: text/plain;charset=UTF-8 date: Wed, 09 Oct 2024 09:56:48 GMT server: nginx/1.24.0 (Ubuntu) transfer-encoding: chunked accept: / accept-encoding: gzip, deflate accept-language: en-US,en;q=0.9,ru;q=0.8 connection: keep-alive content-length: 32 content-type: application/x-www-form-urlencoded; charset=UTF-8 host: sandbox.usm.md origin: http://sandbox.usm.md referer: http://sandbox.usm.md/login/ user-agent: Mozilla/5.0 (Linux; Android 6.0; Nexus 5 Build/MRA58N) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/129.0.0.0 Mobile Safari/537.36 x-requested-with: XMLHttpRequest

Form Data : username: admin password: password

Задание №2. Составление HTTP-запросов
Составьте GET-запрос к серверу по адресу http://sandbox.com, указав в заголовке User-Agent ваше имя и фамилию. полсе отправки get запроса с Kye : User Agent и Value : Craciun Dan серверет ответил Status: 200 OK, Date: Wed, 09 Oct 2024 10:27:10 GMT Content-Type: text/html Transfer-Encoding: chunked Connection: keep-alive Last-Modified: Fri, 05 Jan 2024 09:22:02 GMT cf-cache-status: DYNAMIC Report-To: {"endpoints":[{"url":"https://a.nel.cloudflare.com/report/v4?s=PDo02sJv45WK7sgy9bJHFhNGrJj48FfkzPhTH"}],"success_fraction":0,"report_to":"cf-nel","max_age":604800} NEL: {"success_fraction":0,"report_to":"cf-nel","max_age":604800} Speculation-Rules: "/cdn-cgi/speculation" Server: cloudflare CF-RAY: 8cfdad346ddc5b1f-VIE Content-Encoding: br

Составьте POST-запрос к серверу по адресу http://sandbox.com/cars
полсе отправки запроса raw { "make": "Toyota", "model": "Corolla", "year": "2020" }

или же через x-www-form-urlencoded:

Key: make, Value: Toyota Key: model, Value: Corolla Key: year, Value: 2020

сервер вернул 404Not Foundэ