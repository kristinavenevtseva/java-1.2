# Отчёт о тестировании Credit Card Number Validator

## Краткое описание

04.05.2020 года были проведены тестирования приложения Credit Card Number Validator: функциональное, по методу граничных значений, на основе чек-листа.

На тестирование затрачено: 2 часа.

В результате тестирования выявлены следующие дефекты:
* https://github.com/kristinavenevtseva/java-1.2/issues/1

## Описание процесса тестирования

В процессе тестирования использовались следующие артефакты:
* чек-лист
* баг-репорт
* отчет о тестировании

В качестве тестовых данных использовались данные чек-листа.

Валидные номера карт:
* номер карты 5351719427810741, результат: Result is OK
* номер карты 4046975929638, результат: Result is FAIL
* номер карты 370911917788127, результат: Result is FAIL
* номер карты 63046657674035002, результат: Result is FAIL
* номер карты 503883253619185010, результат: Result is FAIL
* номер карты 6771873275175363896, результат: Result is FAIL

Невалидные номера карт:
* номер карты 0000000000000000, результат: Result is FAIL
* номер карты 1, результат: Result is FAIL
* номер карты 1111111111111111111111111, результат: Result is FAIL
* номер карты 11111111, результат: Result is FAIL
* номер карты 56784397бтмсгрдв, результат: Result is FAIL
* номер карты 6%7*5689:;№56)*8, результат: Result is FAIL
* номер карты <пустое поле>, результат: Result is FAIL
* номер карты asdfghjyrtdhokyp, результат: Result is FAIL
* номер карты 5679345698762345, результат: Result is FAIL

Тестирование производилось в следующем окружении:
* Windows 10, версия 1903, 64-разрядная
* версия Java "11.0.7" 2020-04-14
* IntelliJ IDEA 2020.1.1 (Community Edition)
