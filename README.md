
![logo](https://images.squarespace-cdn.com/content/55916c9fe4b0f356a27adc38/1436353372925-GTN274AXNY1YXT4F9IT8/nginx.png)

# Конфигурация nginx на все случаи жизни
## Предыстория
**nginx [engine x]** — это HTTP-сервер и обратный прокси-сервер, почтовый прокси-сервер, а также TCP/UDP прокси-сервер общего назначения, изначально написанный [Игорем Сысоевым](http://sysoev.ru/). Уже длительное время он обслуживает серверы многих высоконагруженных российских сайтов, таких как [Яндекс](http://www.yandex.ru/), [Mail.Ru](http://mail.ru/), [ВКонтакте](http://vk.com/) и [Рамблер](http://www.rambler.ru/). 

## Цель проекта
Каждый пользователь сталкивался с проблемой настройки веб сервера nginx. Мы решили объединить все сценарии конфигурации в одном файле, чтобы выполнялись следующие критерии:
1. Легкая адаптация под нужды пользователя
2. Хорошая документация
3. Соответствие best-practice

### Лицензионное соглашение nginx
> *Copyright (C) 2002-2021 Igor Sysoev
> Copyright (C) 2011-2023 Nginx, Inc.
> All rights reserved.*
>
> *Redistribution and use in source and binary forms, with  or without
> modification, are permitted provided that the following conditions
> are met:*
> 1. *Redistributions of source code must retain the above copyright
>    notice, this list of conditions and the following disclaimer.*
> 2. *Redistributions in binary form must reproduce the above copyright
>    notice, this list of conditions and the following disclaimer in the
>    documentation and/or other materials provided with the distribution.*
>
> *THIS SOFTWARE IS PROVIDED BY THE AUTHOR AND CONTRIBUTORS ``AS IS'' AND
> ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
>  IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
> ARE DISCLAIMED.  IN NO EVENT SHALL THE AUTHOR OR CONTRIBUTORS BE LIABLE
> FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
> DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS
> OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION)
> HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
> LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY
> OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF
> SUCH DAMAGE.*


### Использование
Склонировать репозиторий:
```
git clone https://gitlab.rebrainme.com/devops_users_repos/4756/rebrain-devops-task1.git
```
Отредактировать секцию server {}
```
    #server {
    #    listen       443 ssl;
    #    server_name  localhost;

    #    ssl_certificate      cert.pem;
    #    ssl_certificate_key  cert.key;

    #    ssl_session_cache    shared:SSL:1m;
    #    ssl_session_timeout  5m;

    #    ssl_ciphers  HIGH:!aNULL:!MD5;
    #    ssl_prefer_server_ciphers  on;

    #    location / {
    #        root   html;
    #        index  index.html index.htm;
    #    }
    #}

```

### История версий
|Номер версии|Добавленные изменения|Дата выпуска|
|:---:|:---:|:---:|
|v1.0|первая версия|11.10.2022|
|v1.0.1|багфиксы|20.10.2022|
|v2.0|добавлен функционал|15.11.2022|
|v2.0.1|исправлены баги|20.11.2022|
