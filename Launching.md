Статья в процессе запиливания.

| system property | значение по умолчанию | описание |
| --------------- | --------------------- | -------- |
| org.ultramine.terminal | jline | Используемый консольный терминал. Возможные значения: `default` - удаляются все цвета и иные управляющие последовательности; `raw` - все майновские управляющие последовательности остаются как есть (\u00a7 + [0-9k-or]); `ansi` - все майновские управляющие последовательности заменяются на ANSI; `jline` - то же, что "ansi" + автокомплит по табу и поддержка windows терминала |
| org.ultramine.dirs.vanilla | storage | Имя директории, в которой создаются все ванильные файлы конфигурации (в ванилле они создаются в корне сервера). Для совместимости с ванильным расположением стоит указать `.` |
| org.ultramine.dirs.worlds | worlds | Директория, в которой создаются миры(в ванилле они создаются в корне сервера). Для совместимости с ванильным расположением стоит указать `.` |
| org.ultramine.dirs.settings | settings | Имя директории, в которой создаются все конфиги UltraMine |
| org.ultramine.dirs.storage | storage  | Имя директории, в которой хранятся различные данные UltraMine |
| org.ultramine.server.offheapchunk.memlimit | 6 | Задает лимит памяти для off-heap хранилища чанков в гигабайтах. Обратите внимание - это не выделение памяти, а **лимит**, т.е. при попытке занять больше будет брошено OutOfMemoryError, но памяти будет расходоваться столько, сколько нужно, вне зависимости от этого числа. Не изменяйте, если не поняли вышесказанного |
| ultramine.debug.chunksyncload | false | Только для разработчиков. Выводит в лог все синхронные загрузки чанков |