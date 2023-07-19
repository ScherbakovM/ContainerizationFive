# ContainerizationFive
Контейнеризация семинар 5

### docker-compose

### Для того чтобы создать контейнеры через docker-compose необходимо создать инструкцию yaml

Создаём директорию для нашего проекта 

`mkdir test_compose`    
И сразу перейдём в нее  
`cd test_compose`  

### Создадим yaml фаил

`nano compose.yaml`

и заполняем его

![image](https://github.com/ScherbakovM/ContainerizationFive/assets/109952823/92bc71d7-22d5-45d4-a3fe-b3546266b29b)

### Nginx это обратный прокси сервер, он пробрасывает порты для нашего сайта, в нем указывается дирректория для рабочих файлов и тд. 
### Его будем использовать для запуска web приложения 
### mysql  используем как базу данных

### Запускаем сборку контейнеров 

### docker-compose up -d

![image](https://github.com/ScherbakovM/ContainerizationFive/assets/109952823/3bcdeaab-3d9e-4dc3-8e8b-9aff48774b47)

### проверяем контейнеры 

![image](https://github.com/ScherbakovM/ContainerizationFive/assets/109952823/fae588ad-7b47-4d8e-b6df-078f0a636bee)

### на 8087 порту работает наш nginx сервер

![image](https://github.com/ScherbakovM/ContainerizationFive/assets/109952823/6713dd85-b8b2-4b53-8a30-b92b0a02c257)


### на 3309 порту mysqlserver

### создадим для теста таблицу 

![image](https://github.com/ScherbakovM/ContainerizationFive/assets/109952823/884ef0ca-36b0-4db4-abdb-5a210e730efd)


### и попробуем подключиться к ней

![image](https://github.com/ScherbakovM/ContainerizationFive/assets/109952823/03b4709d-9de9-482d-ac5a-bd7207fb1c10)

## подключились, данные выводятся 


