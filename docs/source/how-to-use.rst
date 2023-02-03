如何使用
=====

.. _installation:

下载
------------

请通过下列方式下载模组，除此之外皆为非法分发

1. 官网：https://www.serpzacek.com/addons/serp-pok%C3%A9drock
2. MCPEDL：https://mcpedl.com/user/zacek-estrada/
3. MineBBS（汉化）：https://www.minebbs.com/pokedrock/

.. code-block:: console

   (.venv) $ pip install lumache

安装
----------------

To retrieve a list of random ingredients,
you can use the ``lumache.get_random_ingredients()`` function:

.. autofunction:: lumache.get_random_ingredients

The ``kind`` parameter should be either ``"meat"``, ``"fish"``,
or ``"veggies"``. Otherwise, :py:func:`lumache.get_random_ingredients`
will raise an exception.

.. autoexception:: lumache.InvalidKindError

For example:

>>> import lumache
>>> lumache.get_random_ingredients()
['shells', 'gorgonzola', 'parsley']

