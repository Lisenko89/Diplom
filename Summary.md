# Отчет о проведённой автоматизации тестирования
## Что было запланировано и что было сделано
Изначально в планах нужно было выполнить больше проверок, в том числе на соответствие текста выводимых ошибок (проверка текстовой части ошибок).  

При автоматизации тестирования произошли изменения в части выполнения проверок. В частности не была включена в автоматизацию проверка заголовка страницы (имя вкладки в браузере) и проверки на соответствие текста выводимых ошибок (проверка текстовой части ошибок), оставив лишь проверки соответствия выводимых ошибок (проверки отображения).

План автоматизации тестирования был составлен с учетом этих нюансов, все сценарии прописанные в нем были выполнены.
## Причины, повлиявшие на изменения при тестировании
Отсутствие спецификации, либо оформленных требований для данного приложения. Соответственно отсутствуют четкие формулировки текста ошибок, заголовка страницы и тд.
## Сработавшие риски  
**Своеобразная настройка SUT при запуске (заявлена поддержка двух СУБД):**  
- Было затрачено дополнительное время, необходимое для осуществления корректного запуска приложения и выяснения как именно нужно передавать параметры при запуске приложения и при запуске авто-тестов.

**Отсутствие как таковой спецификации на приложение:**  
- При автоматизации тестирования возникли изменения связанные с отсутствием утвержденной спецификации и требований к приложению.

**Зависимость авто-тестов от текущей реализации веб-элементов, так как их изменение может привести к падению авто-тестов:**  
- В проекте не предусмотрены тестовые атрибуты (селекторы), что усложняет адаптацию авто-тестов и их устойчивость.

**Авто-тесты не проверяют графическую составляющую (Расположение текста, положение элементов на странице, соответствие выбранной цветой схеме оформления и тд.):**  
- В процессе ручного тестирования была обнаружена опечатка в названии города.  

## Общий итог по времени:
Подготовка к проведению тестирования (запуск SUT, подготовка плана автоматизации) - 16 часов;  
•	Написание и прогон авто-тестов - 40 часов;  
•	Написание баг-репортов - 8 часов;  
•	Оформление отчёта по итогам тестирования - 8 часов;  
•	Оформление отчёта по итогам автоматизации - 16 часов.
