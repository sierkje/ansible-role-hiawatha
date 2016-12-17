Ansible role: Hiawatha
======================

Builds and configures Hiawatha Webserver on Debian/Ubuntu Linux servers.

Out-of-the-box, when the provided defaults are not overridden, this role will build Hiawatha from source and configure it
as a mostly 'vanilla' installation (the only thing non-standard is the default website, unless a custom definition is
provided, this role will follow the recommendation in the Hiawatha documentation).

But even though it is not required, it is useful to at least define custom values for some of the many settable
variables that are available for:

* customizing the way Hiawatha is built from source (i.e. without cache support, with Hiawatha Monitor support, etc.)
* defining whether or not Hiawatha should be upgraded to the latest version, when that one is newer than the one installed
* customizing the general server configuration (i.e. provide ban settings to deny service to clients who misbehave, control the upload speed of files, etc.)
* adding (or remove) the ports clients can connect to (i.e. adding Binding records)
* providing virtual host definitions (i.e. adding VirtualHost records )
* defining tasks for copying files to, or creating files, on the server(s)
* providing options for directories (i.e. adding Directory records)
* providing FastCGI server information (i.e. adding FastCGIserver records)
* providing rules for performing actions (based) on the URL (i.e. adding UrlToolkit records, used for URL rewriting, etc.)
* defining or overriding almost any other advanced configuration option, etc.

.. toctree::
   :maxdepth: 2
   :caption: Contents:

   index
   install/index
   config/index
   config/server
   config/bindings
   config/hosts
   config/directories
   config/fast-cgi
   config/url-toolkits
   config/advanced

Indices and tables
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`
