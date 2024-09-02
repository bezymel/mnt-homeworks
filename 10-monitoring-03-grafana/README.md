# Домашнее задание к занятию 14 «Средство визуализации Grafana»

## Обязательные задания

### Задание 1

1. Используя директорию [help](./help) внутри этого домашнего задания, запустите связку prometheus-grafana.
1. Зайдите в веб-интерфейс grafana, используя авторизационные данные, указанные в манифесте docker-compose.
1. Подключите поднятый вами prometheus, как источник данных.
1. Решение домашнего задания — скриншот веб-интерфейса grafana со списком подключенных Datasource.

### Ответ 1

![image](https://github.com/user-attachments/assets/92c7ee1c-0af2-469b-b6c1-77b04fd67ef1)
![image](https://github.com/user-attachments/assets/26d9f180-9d2c-453d-a59d-810fa2eff7ea)
![image](https://github.com/user-attachments/assets/a83faac0-5cdb-43a0-b6c8-0246d52dca3c)

## Задание 2

Изучите самостоятельно ресурсы:

1. [PromQL tutorial for beginners and humans](https://valyala.medium.com/promql-tutorial-for-beginners-9ab455142085).
1. [Understanding Machine CPU usage](https://www.robustperception.io/understanding-machine-cpu-usage).
1. [Introduction to PromQL, the Prometheus query language](https://grafana.com/blog/2020/02/04/introduction-to-promql-the-prometheus-query-language/).

Создайте Dashboard и в ней создайте Panels:

- утилизация CPU для nodeexporter (в процентах, 100-idle);
- CPULA 1/5/15;
- количество свободной оперативной памяти;
- количество места на файловой системе.

Для решения этого задания приведите promql-запросы для выдачи этих метрик, а также скриншот получившейся Dashboard.

## Ответ 2

![image](https://github.com/user-attachments/assets/77baa3cf-fc34-4617-8bb3-e7a866cbee18)
![image](https://github.com/user-attachments/assets/91f9c7db-594a-4794-965d-e871e8d64880)
![image](https://github.com/user-attachments/assets/de20b47a-8300-46ff-95e2-5e6c6dc99150)

## Задание 3

1. Создайте для каждой Dashboard подходящее правило alert — можно обратиться к первой лекции в блоке «Мониторинг».
1. В качестве решения задания приведите скриншот вашей итоговой Dashboard.

## Ответ 3

![image](https://github.com/user-attachments/assets/bc89d7b3-894f-4035-98d6-aac171d68f8f)
![image](https://github.com/user-attachments/assets/ad5e638a-ca02-49d7-a6a6-d6a0b6af2fc9)
![image](https://github.com/user-attachments/assets/0f39ce97-615f-4ca7-bba9-05b49e9d8b8a)
![image](https://github.com/user-attachments/assets/b3e89188-fae6-438f-b028-1d4501939edc)

## Задание 4

1. Сохраните ваш Dashboard.Для этого перейдите в настройки Dashboard, выберите в боковом меню «JSON MODEL». Далее скопируйте отображаемое json-содержимое в отдельный файл и сохраните его.
1. В качестве решения задания приведите листинг этого файла.

---

### Как оформить решение задания

Выполненное домашнее задание пришлите в виде ссылки на .md-файл в вашем репозитории.

---
