# virt-03-docker-intro        
## Задача 1
(https://hub.docker.com/repository/docker/suntsovvv/custom-nginx/general)
## Задача 2
1. ![image](https://github.com/suntsovvv/virt-03-docker-intro/assets/154943765/8e9de5ff-452f-4271-b42b-d881ccd33aa0)
2. ![image](https://github.com/suntsovvv/virt-03-docker-intro/assets/154943765/cf6c6e42-c999-4f10-b1ec-94770e5c7758)
3. ![image](https://github.com/suntsovvv/virt-03-docker-intro/assets/154943765/65a9d67f-15ef-41dc-b7e1-316a5b513cf7)
4. ![image](https://github.com/suntsovvv/virt-03-docker-intro/assets/154943765/8f8db8cb-af61-40e1-9f14-f40a0dcc0b45)
## Задача 3
![image](https://github.com/suntsovvv/virt-03-docker-intro/assets/154943765/d87a2977-cb58-4ea4-98ad-451a8a56cadc)
Я считаю, что контейнер остановился потому, что контейнер был запущен в неинтерактивном режиме,комбинация Ctrl-C посылает выполняемому процессу (а контейнеры запускаются как процессы) сигнал SIGINT, что значит завершение процесса.
![image](https://github.com/suntsovvv/virt-03-docker-intro/assets/154943765/d5471d64-f2d9-4949-81fa-2de2670dd701)
![image](https://github.com/suntsovvv/virt-03-docker-intro/assets/154943765/98bb0bb1-2537-4104-b253-fd7bc0abf26e)
![image](https://github.com/suntsovvv/virt-03-docker-intro/assets/154943765/98447126-1c9c-4053-ab79-408c2b122341)
![image](https://github.com/suntsovvv/virt-03-docker-intro/assets/154943765/aa4fc5a3-4be2-471a-8ab7-ca2997036352)
![image](https://github.com/suntsovvv/virt-03-docker-intro/assets/154943765/c83b9714-a018-4b38-8de6-bfb177c8167a)
![image](https://github.com/suntsovvv/virt-03-docker-intro/assets/154943765/a79076e8-8edd-499c-9cd2-b48f0bcf1202)  

Суть возникшей проблемы проста. 
Когда мы запускали контейнер из образа , мы указывали перенаправление порта 80 из контейнера в порт 8080 хостовой машины.
Мы изменили конфиг сервера nginx, теперь он слушает 81 порт и на 80 порту ничего нет.

### Дополнительное задание
Останавливаем контейнер:  
![image](https://github.com/suntsovvv/virt-03-docker-intro/assets/154943765/405b63b8-f676-4699-968c-bda32743744a)

Открываем конфигурационный файл config.v2.json контейнера:  
![image](https://github.com/suntsovvv/virt-03-docker-intro/assets/154943765/93489b6e-ab86-4418-a3ba-d5d4ebe62813)

Меняем привязку к порту:  
![image](https://github.com/suntsovvv/virt-03-docker-intro/assets/154943765/3354f618-d04a-4ed2-af1f-484eaad443bd)

Открываем конфигурационный файл hostconfig.json контейнера:  
![image](https://github.com/suntsovvv/virt-03-docker-intro/assets/154943765/9e2ccf7c-9945-439e-b0a0-6c5387f9c585)

Меняем привязку к порту:  
![image](https://github.com/suntsovvv/virt-03-docker-intro/assets/154943765/5340f309-d799-408c-8324-010ff30d950f)

Перезапускаем doker:  
![image](https://github.com/suntsovvv/virt-03-docker-intro/assets/154943765/25a9faef-287e-4b69-990f-3603a543b04d)

Запускаем контейнер:  
![image](https://github.com/suntsovvv/virt-03-docker-intro/assets/154943765/0c70f89a-4ed2-4cd7-b060-72b7a68881aa)

Результат:  
![image](https://github.com/suntsovvv/virt-03-docker-intro/assets/154943765/10545a66-dbff-4f2c-8951-484a46cf8802)  

Удаление контейнера без остановки:  
![image](https://github.com/suntsovvv/virt-03-docker-intro/assets/154943765/eb59a700-4d33-4f33-947e-3f1a698c764b)  

## Задача 4
![image](https://github.com/suntsovvv/virt-03-docker-intro/assets/154943765/89dfc018-98ca-43ad-b7ce-eb16757737f8)

## Задача 5  
![image](https://github.com/suntsovvv/virt-03-docker-intro/assets/154943765/8b156824-1794-40dd-aa2d-0c1f49e22c2c)
Запустился файл compose.yaml, так как приналичии нескольких файлов yaml в одной директории
Отредактируем файл compose.yaml:  
![image](https://github.com/suntsovvv/virt-03-docker-intro/assets/154943765/8ac8b49c-1fd6-4212-899c-0d20337e63a1)  
Запускаем по новой:  
![image](https://github.com/suntsovvv/virt-03-docker-intro/assets/154943765/d3d53089-016a-4bf4-80f6-dcef8f732839)
![image](https://github.com/suntsovvv/virt-03-docker-intro/assets/154943765/db0e697b-4179-4bb8-aebd-9f78ebe9353c)
![image](https://github.com/suntsovvv/virt-03-docker-intro/assets/154943765/d57c5a98-b696-478c-bb5c-48aab1d07ffa)

![image](https://github.com/suntsovvv/virt-03-docker-intro/assets/154943765/0c5b0861-b9a6-4b0e-9ff9-052edfe04aeb)  
Cjобщение означает.......  
![image](https://github.com/suntsovvv/virt-03-docker-intro/assets/154943765/7b03db7f-3e54-4a72-8f8c-887156ae2b1b)







 





















