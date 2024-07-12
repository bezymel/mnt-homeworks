# Домашнее задание к занятию 1 «Введение в Ansible»

## Подготовка к выполнению

1. Установите Ansible версии 2.10 или выше.
2. Создайте свой публичный репозиторий на GitHub с произвольным именем.
3. Скачайте [Playbook](./playbook/) из репозитория с домашним заданием и перенесите его в свой репозиторий.

## Основная часть

1. Попробуйте запустить playbook на окружении из `test.yml`, зафиксируйте значение, которое имеет факт `some_fact` для указанного хоста при выполнении playbook.
2. Найдите файл с переменными (group_vars), в котором задаётся найденное в первом пункте значение, и поменяйте его на `all default fact`.
3. Воспользуйтесь подготовленным (используется `docker`) или создайте собственное окружение для проведения дальнейших испытаний.
4. Проведите запуск playbook на окружении из `prod.yml`. Зафиксируйте полученные значения `some_fact` для каждого из `managed host`.
5. Добавьте факты в `group_vars` каждой из групп хостов так, чтобы для `some_fact` получились значения: для `deb` — `deb default fact`, для `el` — `el default fact`.
6.  Повторите запуск playbook на окружении `prod.yml`. Убедитесь, что выдаются корректные значения для всех хостов.
7. При помощи `ansible-vault` зашифруйте факты в `group_vars/deb` и `group_vars/el` с паролем `netology`.
8. Запустите playbook на окружении `prod.yml`. При запуске `ansible` должен запросить у вас пароль. Убедитесь в работоспособности.
9. Посмотрите при помощи `ansible-doc` список плагинов для подключения. Выберите подходящий для работы на `control node`.
10. В `prod.yml` добавьте новую группу хостов с именем  `local`, в ней разместите localhost с необходимым типом подключения.
11. Запустите playbook на окружении `prod.yml`. При запуске `ansible` должен запросить у вас пароль. Убедитесь, что факты `some_fact` для каждого из хостов определены из верных `group_vars`.
12. Заполните `README.md` ответами на вопросы. Сделайте `git push` в ветку `master`. В ответе отправьте ссылку на ваш открытый репозиторий с изменённым `playbook` и заполненным `README.md`.
13. Предоставьте скриншоты результатов запуска команд.

## Ответ 

![image](https://github.com/user-attachments/assets/64c3e2c5-9922-40db-a14f-f28334eb300f)

![image](https://github.com/user-attachments/assets/94dbc4c7-1c75-453c-a4fb-fcb958c2fe35).

![image](https://github.com/user-attachments/assets/4197fa45-23bc-4825-b4c4-226e4a665eb5)

![image](https://github.com/user-attachments/assets/80b1dcd1-994e-43be-8b5a-cab00895d204)

![image](https://github.com/user-attachments/assets/4d357400-f922-4617-9203-dd5c3ff5cb83)

![image](https://github.com/user-attachments/assets/6f65fed1-6bf9-4eed-815a-43adef521300)

![image](https://github.com/user-attachments/assets/b3e4da2a-e20d-4516-8e78-d738507f32a3)

![image](https://github.com/user-attachments/assets/8c605dbc-02b4-474a-9494-1dc39c2f4a6b)

![image](https://github.com/user-attachments/assets/8099653c-cc7f-4d5c-a148-f069aa4e8de3)

![image](https://github.com/user-attachments/assets/55aaad96-b42b-4d98-89d9-1801f8653f86)

![image](https://github.com/user-attachments/assets/f177cff7-61aa-4593-816b-3e2e454d01a1)

![image](https://github.com/user-attachments/assets/21ee228c-956d-4db5-b0a5-02a8c74d3ab0)

## Необязательная часть

1. При помощи `ansible-vault` расшифруйте все зашифрованные файлы с переменными.
2. Зашифруйте отдельное значение `PaSSw0rd` для переменной `some_fact` паролем `netology`. Добавьте полученное значение в `group_vars/all/exmp.yml`.
3. Запустите `playbook`, убедитесь, что для нужных хостов применился новый `fact`.
4. Добавьте новую группу хостов `fedora`, самостоятельно придумайте для неё переменную. В качестве образа можно использовать [этот вариант](https://hub.docker.com/r/pycontribs/fedora).
5. Напишите скрипт на bash: автоматизируйте поднятие необходимых контейнеров, запуск ansible-playbook и остановку контейнеров.
6. Все изменения должны быть зафиксированы и отправлены в ваш личный репозиторий.

---

### Как оформить решение задания

Выполненное домашнее задание пришлите в виде ссылки на .md-файл в вашем репозитории.

---
