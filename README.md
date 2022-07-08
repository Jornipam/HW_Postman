# HW_Postman
Этот репозиторий предназначен для демонстрации навыков, полученных в процессе изучения программы Postman.

---
## HW1 by [Vadim Ksendzov]("https://ksendzov.com/")
Целью первого задания было создать запросы в Postman на различные endpoint'ы сервера и получить от каждогоо определенный ответ.

Решение: [hw_postman1_jorni_pam.json]("https://github.com/Jornipam/HW_Postman/blob/main/hw_postman_jorni_pam.json")


---
## HW2 by [Vadim Ksendzov]("https://ksendzov.com/")
Целью второго задания было изучить применение сниппетов, создание окружения, парсинг запросов и ответов, построение тестов на основе полученных данных.

Решение: [hw_postman2_jorni_pam.json]("https://github.com/Jornipam/HW_Postman/blob/main/hw_postman2_jorni_pam.json")

---
## HW2 by [Anatoly Karpovich]("https://www.linkedin.com/in/anatolykarpovich/")

Целью **первой части** этого задания было провести тестирование API данного enpoint'а на валидацию входных параметров.

Решение: [hw2_postman_Anatoly1.1_jorni_pam.json]("https://github.com/Jornipam/HW_Postman/blob/main/hw2_postman_Anatoly1.1_jorni_pam.json") + [environment hw2_postman_Anatoly2_jorni_pam.json]("https://github.com/Jornipam/HW_Postman/blob/main/environment%20hw2_postman_Anatoly2_jorni_pam.json")


Условия: 

1. Условно считаем, что негативная проверка должна возвращать любой статус НО НЕ 200.
2. На один запрос приходится только одна негативная проверка.
3. Позитивные проверки можно объединть в одну.

Требования:

1. Name: 3-40 символов включительно, запрещены префиксные и постфиксные пробелы. Поле обязательное
2. Age: только целые цифры в диапазоне 18-120 включительно. Поле обязательное
3. Salary: только целые цифры в диапазоне 1-1000000 включительно. Поле обязательное

P.S. ЗАДАНИЕ НЕ ПОДРАЗУМЕВАЕТ, ЧТО ЭНДПОИНТ РАБОТАЕТ СОГЛАСНО НАПИСАННЫМ ТРЕБОВАНИЯМ. МЫ УЧИМСЯ ПИСАТЬ ТЕСТЫ НА API!

Целью **второй части** этого задания было  преобразовать часть 1 таким образом, чтобы:
1. параметры забираись из CSV файла. 
2. в коллекции был только 1 запрос, который будет повторяться столько раз, сколько строк в CSV файле. 
3. была написана функция в тестах, которая проверяет валидность входящих данных, и в зависимости от этого проверяет на статус 200 или НЕ 200.

 Решение: [hw2_postman_Anatoly2_jorni_pam.json]("https://github.com/Jornipam/HW_Postman/blob/main/hw2_postman_Anatoly2_jorni_pam.json") + [environment hw2_postman_Anatoly2_jorni_pam.json]("https://github.com/Jornipam/HW_Postman/blob/main/environment%20hw2_postman_Anatoly2_jorni_pam.json") + [hw2_postman_anatoly2_data.csv]("https://github.com/Jornipam/HW_Postman/blob/main/hw2_postman_anatoly2_data.csv")

Так же во **второй части** было проеобразование заданий из HW2 by Vadim Ksendzov.

Задание 2* :

Проверить, что 0-й,1-й,2-й элемент параметра salary равен salary/salary*2/salary*3 из request (salary забрать из request.) Преобразовать проверку таким образом что бы она производилась циклом , в котором будет всего один тест.Имя теста должно меняться в зависимости от значения в Salary.

Задание 3* :

Проверить, что name/age/salary в ответе равно name/age/salary в запросе. Преобразовать проверку (сравнить идентичные поля в реквесте и респонсе) таким образом, чтобы это делалось ЗА ОДИН ТЕСТ (сразу все 3 поля) БЕЗ ЦИКЛОВ! (глубокое сравнение объектов).
