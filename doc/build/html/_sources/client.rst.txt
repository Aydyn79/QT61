Client package documentation
============================
Модуль клиентской части приложения для обмена сообщениями. 
Обеспечивает обмен сообщениями с активными пользователями,
т.е. которые находятся в сети и подключены к серверу.
Текст сообщений шифруется с помощью алгоритма шифрования RSA.

Файл client_app.py (основной файл клиентского приложения) 
поддерживает запуск с помощью коммандной строки.
Например:

``python client_app.py {имя сервера} {порт} --name {имя пользователя} и --password {пароль}``

1. {имя сервера} - ip-адрес сервера 
2. {порт} - порт сервера
3. --name - имя пользователя с которым произойдёт вход в систему.
4. --password - пароль пользователя.

Параметры командной строки являются необязательными, 
если их не ввести, программа запросит их позднее (по крайней мере имя и пароль).

Например допустимы следующие параметры коммандной строки:

* ``python client_app.py``

*Запуск приложения с ip-адресом по умолчанию "127.0.0.1" и номером порта "7777".*

* ``python client_app.py 125.87.0.15 3050``

*Запуск приложения с подключением к серверу по адресу 125.87.0.15:3050*

* ``python client_app.py --name test1 --password 123``

*Запуск приложения со значениями ip-адреса и порта сервера по умолчанию* 
*и c логином пользователя: test1 и паролем: 123*

* ``python client.py 125.87.0.15 3050 --name nexter --password qwerty``

*Запуск приложения с логином nexter и паролем qwerty и параметрами подключения к серверу по адресу 125.87.0.15:3050*
*Кроме того, необходимо учесть, что при вводе значений ip-адреса и порта сервера проверяется их валидность*
*При значениях порта менее 1024 и более 65535 будет выведено сообщение:*
*Попытка запуска клиента с неподходящим номером порта*
*Допустимы адреса с 1024 до 65535. Клиент завершается.*

Submodules
----------

client.add\_contact module
--------------------------

.. automodule:: client.add_contact
   :members:
   :undoc-members:
   :show-inheritance:

client.client\_base module
--------------------------

.. automodule:: client.client_base
   :members:
   :undoc-members:
   :show-inheritance:

client.del\_contact module
--------------------------

.. automodule:: client.del_contact
   :members:
   :undoc-members:
   :show-inheritance:

client.main\_window module
--------------------------

.. automodule:: client.main_window
   :members:
   :undoc-members:
   :show-inheritance:

client.main\_window\_conv module
--------------------------------

.. automodule:: client.main_window_conv
   :members:
   :undoc-members:
   :show-inheritance:

client.net\_client module
-------------------------

.. automodule:: client.net_client
   :members:
   :undoc-members:
   :show-inheritance:

client.start\_dialog module
---------------------------

.. automodule:: client.start_dialog
   :members:
   :undoc-members:
   :show-inheritance:

Module contents
---------------

.. automodule:: client
   :members:
   :undoc-members:
   :show-inheritance:
