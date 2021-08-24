
Confluence-docker
=================


Скрипт установки и настройки сервиса Confluence.
---------------------------------------------
Во время запуска скрипта предполагается, что docker и docker-compose уже установлены.
Во время запуска скрипта будут загружены последние версии nginx и confluence с сайта https://hub.docker.com/
Далее произойдёт запуск образов nginx и confluence и будут подключены к образам конфигурационные файлы заранее заготовленные.

Запуск скрипта
--------------

.. code-block:: console

  docker-compose -f docker-compose.yaml up

Запуск отдельного сервиса в скрипте
-----------------------------------

.. code-block:: console

  docker-compose -f docker-compose.yaml up nginx &

или

.. code-block:: console

  docker-compose -f /atlassian/docker-compose.yaml stop nginx
  docker-compose -f /atlassian/docker-compose.yaml start nginx


Посмотреть выполнение сервисов
------------------------------

.. code-block:: console

  docker ps
