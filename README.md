###### Простой веб-сервер для отдачи статики
_____________________________________
Сервер принимает и обрабатывате только GET и HEAD запросы.

Чтобы поднять сервер локально необходимо собрать образ:<br>
`docker build . --tag go_server_image`<br>

Запустить можно с такими параметрами:<br>
`docker run -p 8080:80 go_server_image`<br>

Чтобы проверить результат работы сервера нужно открыть браузер
на странице http://127.0.0.1:8080/wikipedia_russia.html

Вся статика для этой страницы находится внутри проекта и отдается
сервером.
