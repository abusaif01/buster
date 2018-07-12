A  Fork from `Buster <https://github.com/axitkhurana/buster>`__.

Buster
======

Super simple, Totally awesome, Brute force **static site generator for**
`Ghost <http://ghost.org>`__.

Start with a clean, no commits Github repository.

*Generate Static Pages. Preview. Deploy to Github Pages.*

Warning! This project is a hack. It's not official. But it works for me.

Improvement
-------------
Please read the basic from `Buster <https://github.com/axitkhurana/buster>`__. With all the basic functionality a new parameter has added with this fork. Parameter only added to **generate** command.

``generate [--domain=<local-address>] [--prod-domain=<production-address>]`` 

      Generates static pages from locally running Ghost instance.

After generating all the pages, local url/address (``--domain``) will be replaced with production/actual address/url (provided with parameter ``prod-domain``).

``prod-domain`` is optional. If not provided then URL will remain as it is.  

**No need** to change your blog URL in **Ghost configurations**.

Background
------------
With the  original version if ghost run in local address ( ex. ``http://localhost:2368``) and generate command used then all the static file will have local address as URL, which will not work in production. If we change URL  to production URL in the configuration then run ghost in local, some static page will not work. To Solve this problem this parameter is added.

The Installation
----------------

Install this fork with pip:

    $ pip install git+https://github.com/abusaif01/buster

You'll then have the wonderful ``buster`` command available.

You could also clone the source and use the ``buster.py`` file directly.

