Задача: создать обработчик POST запроса, который принимает на вход имя валюту и возвращает текущий курс к рублю(RUB).
Реализовать тест, который проверяет корректность работы.

Описать в README.md:
1. Как запускать код.
2. Как отправлять запрос и формат ответа. 

1. Установите Python на свой компьютер, если он еще не установлен. Вы можете скачать Python с официального сайта Python (https://www.python.org/downloads/) и следовать инструкциям по установке для вашей операционной системы.

Сохраните файл из репозитория и запустите его.

Код выполнит GET-запрос к указанному API и вернет значение валюты в рублях.

Для отправки запроса и получения ответа вам необходимо использовать модуль requests в Python. В коде, предоставленном выше, функция get_currency_value отправляет GET-запрос по указанному URL https://www.cbr-xml-daily.ru/daily_json.js и получает данные в формате JSON.

Ответ в формате JSON содержит информацию о курсах валют. Вы можете получить значение валюты в рублях, обратившись к соответствующему ключу в JSON-данных.

Например, чтобы получить значение доллара США в рублях, вы можете вызвать функцию get_currency_value('USD'). Она вернет текущее значение доллара США в рублях.

    Примечание: При отправке запроса в API может потребоваться использование дополнительных параметров, таких как заголовки или авторизация. В зависимости от требований API, вам может потребоваться настроить запрос соответствующим образом.