# whisper-test

Ничего не трогайте плз здесь. Описание будет позднее

Программа создает собственный p2p сервер(ноду) и запускает под-протокол whisper(v2).
+Умеет отправлять и получать сообщения с фильтрами по топикам


В репозитории используються собственные модифицированные библиотеки geth, т.к. в оригинальных библиотеках найдены
баги не позволяющие использовать whisper как подключаемый модуль.
Внесены некоторые изменения в файл библиотеки whisper.go (пакет whisperv2) что бы исправить это

Так-же добавлен вывод логов на экран (очень коряво, надо это пофиксить) и некоторые другие небольшие изменения.

Для корректной работы программы можно скачать официальный go ethereum коммандой ```go get github.com/ethereum/go-ethereum ``` и затем
заменить папку go-ethereum папкой модифицированной библиотеки (из соответствующей директории этого репозитория)

Не забывайте добавлять модифицированный go-ethereum из папки src в папку этого проекта, если вносите изменения в библиотеку
