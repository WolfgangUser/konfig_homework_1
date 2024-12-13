<h1>Задание №1</h1>

**Вариант №25**

Разработать эмулятор для языка оболочки ОС. Необходимо сделать работу эмулятора как можно более похожей на сеанс shell в UNIX-подобной ОС. Эмулятор должен запускаться из реальной командной строки, а файл с виртуальной файловой системой не нужно распаковывать у пользователя. Эмулятор принимает образ виртуальной файловой системы в виде файла формата tar. Эмулятор должен работать в режиме GUI.
Ключами командной строки задаются:

•Имя пользователя для показа в приглашении к вводу.

•Имя компьютера для показа в приглашении к вводу.

•Путь к архиву виртуальной файловой системы.

•Путь к лог-файлу.

•Путь к стартовому скрипту.

Лог-файл имеет формат xml и содержит все действия во время последнего сеанса работы с эмулятором. Для каждого действия указаны дата и время. Для каждого действия указан пользователь.
Стартовый скрипт служит для начального выполнения заданного списка команд из файла.

Необходимо поддержать в эмуляторе команды ls, cd и exit, а также следующие команды:

1.tree.

2.mkdir.

3.wc.

Все функции эмулятора должны быть покрыты тестами, а для каждой из поддерживаемых команд необходимо написать 2 теста.

<h2>Описание функций</h2>

•**__init__(self, root, username, hostname, vfs_path, log_path, startup_script)** - создание открывающегося окна

•**load_vfs(self)** - загрузка виртуальной файловой системы

•**log_action(self, action)** - логирование действий

•**process_command(self, event=None)** - выполнение введённой команды

•**ls(self)** - получение и вывод списка файлов в текущем каталоге

•**cd(self)** - изменение директории

•**exit(self)** - выход из эмулятора

•**tree(self)** - отображение структуры каталогов и файлов, а также их количество

•**mkdir(self)** - создание новых директорий

•**wc(self)** - подсчёт числа строк, слов и символов в указанном файле

•**run_startup_script(self)** - выполнение стартового скрипта

<h2>Примеры использования</h2>

Далее на рисунках представлены примеры использования команд.

Команда ls
![1](https://github.com/user-attachments/assets/aa6ddcb8-6012-490b-9b79-6ecec8b28e93)

Команда cd
![2](https://github.com/user-attachments/assets/86e43555-b63b-4711-ac10-0e556ed5abc8)

Команда tree
![3](https://github.com/user-attachments/assets/b6bcb60d-b71d-4c83-918f-35f47262aa24)

Команда mkdir
![4](https://github.com/user-attachments/assets/92bdf00b-849b-4d42-ba35-381ab556f381)


Команда wc
![5](https://github.com/user-attachments/assets/f8ca9d06-d039-41e3-a4f1-158894bf08b6)


<h2>Результаты прогона тестов</h2>

Все тесты были успешно пройдены
![t](https://github.com/user-attachments/assets/450dea09-394e-49c8-8053-c30ada8531fc)



