Домашнее задание к занятию 1 «Введение в Ansible»
Подготовка к выполнению
Установите Ansible версии 2.10 или выше.
Создайте свой публичный репозиторий на GitHub с произвольным именем.
Скачайте Playbook из репозитория с домашним заданием и перенесите его в свой репозиторий.
Основная часть
Попробуйте запустить playbook на окружении из test.yml, зафиксируйте значение, которое имеет факт some_fact для указанного хоста при выполнении playbook.
Найдите файл с переменными (group_vars), в котором задаётся найденное в первом пункте значение, и поменяйте его на all default fact.
Воспользуйтесь подготовленным (используется docker) или создайте собственное окружение для проведения дальнейших испытаний.
Проведите запуск playbook на окружении из prod.yml. Зафиксируйте полученные значения some_fact для каждого из managed host.
Добавьте факты в group_vars каждой из групп хостов так, чтобы для some_fact получились значения: для deb — deb default fact, для el — el default fact.
Повторите запуск playbook на окружении prod.yml. Убедитесь, что выдаются корректные значения для всех хостов.
При помощи ansible-vault зашифруйте факты в group_vars/deb и group_vars/el с паролем netology.
Запустите playbook на окружении prod.yml. При запуске ansible должен запросить у вас пароль. Убедитесь в работоспособности.
Посмотрите при помощи ansible-doc список плагинов для подключения. Выберите подходящий для работы на control node.
В prod.yml добавьте новую группу хостов с именем local, в ней разместите localhost с необходимым типом подключения.
Запустите playbook на окружении prod.yml. При запуске ansible должен запросить у вас пароль. Убедитесь, что факты some_fact для каждого из хостов определены из верных group_vars.
Заполните README.md ответами на вопросы. Сделайте git push в ветку master. В ответе отправьте ссылку на ваш открытый репозиторий с изменённым playbook и заполненным README.md.
Предоставьте скриншоты результатов запуска команд.

Решение:

<img width="637" alt="image" src="https://github.com/user-attachments/assets/b48a5861-64a2-4738-8433-b56a4e08c8d2">

<img width="637" alt="image" src="https://github.com/user-attachments/assets/824525b9-9008-4276-bc6a-2e5e3476bc04">

<img width="637" alt="image" src="https://github.com/user-attachments/assets/b939f131-26af-4917-978d-7db8ee76bee0">

<img width="637" alt="image" src="https://github.com/user-attachments/assets/5bfaf9b6-001a-4c32-89e1-eb4b3c6c3111">

<img width="637" alt="image" src="https://github.com/user-attachments/assets/412293c6-8cc4-4f3d-ab4e-d4854bb52d9e">



