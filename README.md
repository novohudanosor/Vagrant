1) Запустить ВМ с помощью Vagrant. -  Vagrantfile 
2) Обновить ядро ОС из репозитория  - vagrant ssh
3) Оформить отчет в README-файле в GitHub-репозитории.

Выполнил-
1. Выполняем vagrant up
2. vagrant ssh
3. uname -a  (Linux newapp 4.19.0-25-amd64 #1 SMP Debian 4.19.289-2 (2023-08-08) x86_64 GNU/Linux)
4. sudo nano -w /etc/apt/sources.list
5. deb http://deb.debian.org/debian buster-backports main    - // добавил
6. sudo apt update
7. apt search linux-image
8. sudo apt install linux-image-5.10.0-0.deb10.16-amd64
9. sudo reboot
10. uname -r   (5.10.0-0.deb10.16-amd64)   -// ядро обновлено
