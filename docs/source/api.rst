API
===
.. Weather API:

Weather API
------------
To start, first install requests using pip. This allows us to call the API:

.. code-block:: console

   pip install requests

We will also need to access the API key from our .env file:

.. code-block:: console

   pip install python-dotenv

Before writing any code, all libraries need to be installed:

.. code-block:: python

   import requests
   import json
   from datetime import datetime

   import os
   from dotenv import load_dotenv

The first thing we need when using an API is the API key. As it is stored as an environmental variable in .env, we need to retrieve it. In this case, our API key is stored as "WEATHER_KEY" in the .env file:

.. code-block:: python

   load_dotenv()
   api_key = os.getenv("WEATHER_KEY")
