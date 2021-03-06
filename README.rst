User messaging
==============

.. image:: https://img.shields.io/travis/eldarion/user_messages.svg
    :target: https://travis-ci.org/eldarion/user_messages

.. image:: https://img.shields.io/coveralls/eldarion/user_messages.svg
    :target: https://coveralls.io/r/eldarion/user_messages

.. image:: https://img.shields.io/pypi/dm/user-messages.svg
    :target:  https://pypi.python.org/pypi/user-messages/

.. image:: https://img.shields.io/pypi/v/user-messages.svg
    :target:  https://pypi.python.org/pypi/user-messages/

.. image:: https://img.shields.io/badge/license-BSD-blue.svg
    :target:  https://pypi.python.org/pypi/user-messages/


``user-messages`` is an application for allowing users of your Django site to
send messages to each other.


Quick Start
-----------

Include ``user-messages`` in your requirements file and add
``"user_messages"`` to your INSTALLED APPS setting.

Once you have the ``user-messages`` installed, hook up the URLs::

    urlpatterns = patterns("",
        # some cool URLs

        (r"^messages/", include("user_messages.urls")),

        # some other cool URLs
    )

Now all you need to do is wire up some templates.
