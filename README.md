uWSGI
=====

Installs or updates uWSGI. It'll also set the uWSGI emperor to run from a `@reboot` crontab entry.

Requirements
------------

The role is created for Debian-like OS's. The role will also install `build-essential` and some `-dev`
packages that it needs to compile uWSGI.

Role Variables
--------------

The role uses 4 variables, that you can also override:

* `uwsgi_version` - specifies the latest stable version of uWSGI
* `uwsgi_tyrant_mode` - if True, uWSGI will run in Tyrant mode (False by default)
* `uwsgi_lib_dir` - normally shouldn't be changed. the directory where plugins are installed.
   It's `/usr/local/lib/uwsgi` by default.
* `uwsgi_download_url` - normally shouldn't be changed. It's `https://github.com/unbit/uwsgi/archive` by default.


License
-------

BSD

Author Information
------------------

Damjan Georgievski - https://github.com/gdamjan
