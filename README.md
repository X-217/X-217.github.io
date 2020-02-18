# [X-217.github.io](https://x-217.github.io/)
## Yandex Praktikum (Alexey Sidorov, project 10) 

### v0.0.1

    загружены исходные файлы проекта
    
### v0.1.0

    добавлена валидация поля Имя согласно заданию:
        - только кириллица;
        - первая буква заглавная;
        - можно ввести от 2 до 20 символов — это можно задать в атрибутах minlength и maxlength;
        - возможна запись двойных имён — например Анна-Мария.
    
    дополнительно к заданию при валидации поля Имя:
        - исключены варианты с именем, оканчивающимся на "-"
        - после "-" первая буква только заглавная, остальные только строчные
        - в двойном имени и первое и второе имя могут быть однобуквенным (на случай имени вроде Вань-Ю)

### v0.2.0 
           
    добавлена валидация поля E-mail согласно заданию:
        - только латиница
        - «собака» @ — обязательный символ
        - Точка . — тоже обязательный символ
        - Цифры, подчерк, тире — разрешённые символы
        
    дополнительно к заданию при валидации поля E-mail:
        - и первым и последним символом как в левой, так и в правой части может быть только буква или цифра
        - и в левой и в правой частях допускаются "." (имя пользователя из двух частей, разделенных точкой, 
          почта на домене третьего и выше уровня и.т.п.)
        - доменная зона - минимум два символа, только латиница    
    
### v0.3.0

    добавлена валидация поля Телефон согласно заданию:
        - допустимые форматы:
         "+7(925)900-90-90" "+7(925) 900-90-90" "+7 925-900-90-90" "+79259009090" "89259009090"   
          
    дополнительно к заданию при валидации поля Телефон:
        -последние две пары цифр в телефонном номере могут быть отделены от остальных также и пробелами
     
### v0.4.0 

    добавлена валидация поля Сайт согласно заданию:
        - начинаться с http:// или https://;
        - затем www. — это необязательная группа;
        - IP-адрес — 255.255.255.255 или доменное имя — stasbasov.ru
        - порт — необязательная группа. Порт начинается с двоеточия, за которым идут от 2 до 5 цифр. Например: :8080;
        - путь — последовательность из цифр, слешей и латинских букв, на конце которого может стоять решётка #.