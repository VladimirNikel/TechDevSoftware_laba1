# Dracut-модуль

## Описание
Создание собственного dracut-модуля. Исходя из задания необходимо было создать модуль, в котором будет либо текст, либо рисунок и попытаться собрать это всё и чтобы это еще и всё работало.

## Что нужно сделать? Воть:
1. Необходимо выполнить команду в терминале `cd /usr/lib/dracut/modules.d`
1. Создаем папку с названием *01laba* командой `sudo mkdir 01laba>`
1. Создаем документа командой `sudo vim module-setup.sh`
1. В открытый (созданный) документ вставляем текст из файла с точно-таким же именем из репозитория
1. Необходимо также создать второй документ с именем *01laba.sh* для этого воспользуемся командой `sudo vim 01laba.sh`
1. В открытый (созданный) документ вставляем текст из файла с точно-таким же име
нем из репозитория
1. Далее переходим в папку */boot/* для этого воспользуемся командой `cd /boot`
1. Выполняем команду `sudo dracut -f`
1. Выполняем перезагрузку командой `sudo reboot`
1. При перезапуске операционной системы выбираем самое новое ядро (в списке обычно находится выше остальных)
1. Нажимаем клавишу `e` - переходим к редактированию единоразового запуска системы
1. Убираем *rhgb quiet* из строки
1. Выполняем команду нажатием `Ctrl+X`

И видим нашу надпись/рисунок в тексте лога загрузки модулей. 
