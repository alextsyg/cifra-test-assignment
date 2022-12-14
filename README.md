# cifra-test-assignment
## Проект написан с использованием библиотеки React
Для запуска приложения локально необходимо:
1. Cклонировать репозиторий
2. Установить необходимые зависимости с помощью команды: `npm i`
3. Дождаться установки всех зависимостей и запустить приложение с помощью команды: `npm start`
4. Приложение должно открыться в браузере по адресу http://localhost:3000. Если этого не произошло, введите этот адрес в адресную строку браузера для просмотра проекта.
## Описание проекта/работы с приложением
В данном приложении мы можем добавлять товары в таблицу, использую интерфейс модального окна для ввода данных о товаре.
После перезагрузки страницы введённые данные в таблице сохраняются. Для реализации этого был использован local storage.
Хочется отметить, что проект в части вёрстки ***полностью реализован на чистом HTML/CSS*** без использования каких-либо CSS библиотек или библиотек с готовыми компонентами типа MUI, Bootstrap, React Bootstrap и т.д.

На главной и единственный странице нас встречает такой интерфейс:
<img width="1432" alt="image" src="https://user-images.githubusercontent.com/101048709/203712562-6ff14259-807d-4ede-841d-e716736751f7.png">

По нажатию на кнопку `New Item` открывается модальное окно с формой для вводы данных о товаре:
<img width="1432" alt="image" src="https://user-images.githubusercontent.com/101048709/203714409-44001fc2-2d77-4388-8f18-423af18c89eb.png">

Для закрытия модального окна необходимо нажать на кнопку крестик в правом верхнем углу, либо просто щелкнуть мышью за пределами модального окна.

В приложении реализована небольшая валидация вводимых данных, например, проверка на пустые поля в форме, которая выведет предупреждение под input'ом при попытке добавить данные с пустыми полями (при нажатии на кнопку `Add Item`:
<img width="1432" alt="image" src="https://user-images.githubusercontent.com/101048709/203715060-4ca2bb6b-315a-4717-b9dc-b78249e715fa.png">
Также для поля `Price` есть проверка на то, чтобы вводимые данные являлись числовыми.

После введения корректных данных в форму и нажатия на кнопку `Add Item` модальное окно закрывается, а товар добавляется в таблицу на главном экране:
<img width="1432" alt="image" src="https://user-images.githubusercontent.com/101048709/203716013-1f54cca6-9c18-49ae-882e-23ef8c8de545.png">

Как было сказано ранее, данные в таблице сохраняются после перезагрузки страницы. Чтобы принудительно очистить таблицу была реализована пасхалка: по нажатию на надпись `Items In Stock` в центре шапки сайта содержимое таблицы очищается.
<img width="1432" alt="image" src="https://user-images.githubusercontent.com/101048709/203716676-a78908ca-3feb-4fe3-9f75-7d030d067ad6.png">

В приложении была реализована адаптивность благодаря использованию относительных размеров элементов при вёрстке, а также использованию CSS медиа-запросов `@media` для вёрстки элементов под разные разрешения экрана. 
Вот так, например, приложение выглядит на экране Iphone 12 Pro:

<img width="640" alt="image" src="https://user-images.githubusercontent.com/101048709/203717611-35f9338e-9d04-4781-ac1d-df74055dfaf9.png"><img width="640" alt="image" src="https://user-images.githubusercontent.com/101048709/203717758-459320dc-4e7b-4819-97ca-9ce007cf3fc6.png">

![thats-all-folks-optical-art-ece4tkfgzlbep84s](https://user-images.githubusercontent.com/101048709/203719823-650bd6a0-b82c-4038-8a8c-26bf35984916.jpeg)







