# Тестирующая система 

Разработать REST API для создания задач и тестов к ним. Реализовать возможность отправки кода под конкретную задачу и ее автоматическое тестирование.

Процесс создания задачи:
На определенный endpoint отправляется следующая информация: заголовок задачи(название), текст задачи, пример входных данных, пример выходных данных.
Далее на другой endpoint отправляются тесты для задачи в следующем формате: номер задачи, входные данные, выходные данные.

Процесс тестирования задачи:
Отправляется файл с кодом на определенный endpoint. Вместе с кодом отправляются следующие данные: язык на котором написан код, номер задачи.

В ответ на отправку решения возвращается номер этого решения, по которому можно получить результат тестирования. 

Результат тестирования должен содержать в себе информацию о пройденных и не 
пройденных тестах. Для каждого не пройденного теста должна бы быть фактические выходные данные и ожидаемые выходные данные. Если код в процессе выполнения завершился с ошибкой, то это должно быть отмечено. 

Должна быть реализована авторизация, так как каждое решение должно быть прикреплено к конкретному пользователю. Каждый пользователь может просматривать только свои решения. Каждый пользователь может просматривать все задачи. Обычный пользователь не имеет права загружать задачи и тесты к ним.


За основу идеи можно взять примеры таких сайтов как https://codeforces.com, https://codewars.com т.п.
