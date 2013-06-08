Requests: Човешки HTTP
======================


.. image:: https://travis-ci.org/kennethreitz/requests.png?branch=master
        :target: https://travis-ci.org/kennethreitz/requests

.. image:: https://pypip.in/d/requests/badge.png
        :target: https://crate.io/packages/requests/

Requests е човешка HTTP библиотека под Apache2 лиценз, написана на
Python.

Повечето съществуващти Python модули за изпращане на HTTP заявки са
доста тромави и многословни. Вградената библиотека urllib2 в Python
предоставя повечето от HTTP възможностите, които Ви трябват. За
съжеление, API-то изисква нечовешки усилия и за най-лесните задачи.

Нещата не трябва да седят по този начин. Не и в Python.

.. code-block:: pycon

    >>> r = requests.get('https://api.github.com', auth=('user', 'pass'))
    >>> r.status_code
    204
    >>> r.headers['content-type']
    'application/json'
    >>> r.text
    ...

Вижте `същият код, без Requests <https://gist.github.com/973705>`_.

Requests Ви позволява да изпращате HTTP/1.1 заявки. Може да добавяте
заглавия (headers), данни за форми (form data), съставни файлове
(multipart files) и параметри чрез прости Python речници. Requests е
задвижена от httplib и `urllib3 <https://github.com/shazow/urllib3>`_, но
износва цялата работа около тях, за да не Ви се налага да я правите.

Характеристики
--------------

- Международни домейни и URL адреси
- Keep-Alive & Connection Pooling
- Сесии със Устойчивост на Бизквитките
- SSL Верификация
- Basic/Digest Аутентикация
- Елегантни Ключ/Стойност Бизквитки
- Автоматична Декомпресия
- Unicode Отговори
- Качване на Съставни Файлове
- Connection Timeouts
- Thread-safety

Инсталация
----------

За да инстаирате Requests, изпълнете:

.. code-block:: bash

    $ pip install requests

В краен случай:

.. code-block:: bash

    $ easy_install requests

Но, наистина, не бихте искали да използвате `easy_install`.

Документация
------------

Документацията е достъпна на следният адрес:
http://docs.python-requests.org/.

Допринасяне
-----------

#. Проверете за съществуващи дискусии за проблеми или създайте нова таква, ако имате проблем или идея за подобрение. Съществува Contributor Friendly бележка за съществуващи проблеми, които са подходящи за новобранци.
#. Клонирайте `хранилището`_ в GitHub и направете промените си срещу **master** клона (или създайте нов такъв, от него).
#. Напишете тестове, които показват проблема, който сте оправили или функционалността, която сте добавили.
#. Изпратате промените като Pull Request в GitHub и добавете себе си като `Автор`_.

.. _`хранилище`: http://github.com/kennethreitz/requests
.. _`Автор`: https://github.com/kennethreitz/requests/blob/master/AUTHORS.rst
