Server package documentation
============================
Модуль серверной части приложения для обмена сообщениями. 
Обеспечивает прием, обработку и последующую отправку сообщений пользователей,
Обеспечивает регистрацию новых пользователей и авторизацию
Текст сообщений шифруется с помощью алгоритма шифрования RSA.

Файл cerver_app.py (основной файл серверного приложения) 
поддерживает запуск с помощью коммандной строки.
Например:

``python server_app.py {имя сервера} {порт}``

1. {имя сервера} - ip-адрес сервера (по умолчанию: "" - поддержка соединений с любых ip-адресов)
2. {порт} - порт сервера (по умолчанию: 7777)


Параметры командной строки являются необязательными, 
если их не ввести, программа будет использовать значения по умолчанию.

Например допустимы следующие параметры коммандной строки:

* ``python server_app.py``

*Запуск приложения с ip-адресом по умолчанию "" и номером порта "7777".*


*Необходимо учесть, что при вводе значения порта сервера проверяется его валидность*
*При значениях порта менее 1024 и более 65535 будет выведено сообщение:*
*Попытка запуска клиента с неподходящим номером порта*
*Допустимы адреса с 1024 до 65535. Клиент завершается.*





Submodules
----------

server.add\_user module
-----------------------

.. automodule:: server.add_user
   :members:
   :undoc-members:
   :show-inheritance:

server.config\_window module
----------------------------

.. automodule:: server.config_window
   :members:
   :undoc-members:
   :show-inheritance:

server.main\_window module
--------------------------

.. automodule:: server.main_window
   :members:
   :undoc-members:
   :show-inheritance:

server.msg\_processor module
----------------------------

.. automodule:: server.msg_processor
   :members:
   :undoc-members:
   :show-inheritance:

server.remove\_user module
--------------------------

.. automodule:: server.remove_user
   :members:
   :undoc-members:
   :show-inheritance:

server.server\_base module
--------------------------

.. automodule:: server.server_base
   :members:
   :undoc-members:
   :show-inheritance:

server.server\_gui module
-------------------------

.. automodule:: server.server_gui
   :members:
   :undoc-members:
   :show-inheritance:

server.stat\_window module
--------------------------

.. automodule:: server.stat_window
   :members:
   :undoc-members:
   :show-inheritance:

Module contents
---------------

.. automodule:: server
   :members:
   :undoc-members:
   :show-inheritance:
