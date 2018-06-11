### How did you install WebODM? (Docker, natively, ...)?

[Natively, with installing file (.sh).

### What's your browser and operating system? (Copy/paste the output of https://www.whatismybrowser.com/)

Kubuntu 18.04lts - Firefox

### What is the problem?

WODM did not start, report this problem:
Checking for docker...   OK
Checking for git...   OK
Checking for python...   OK
Checking for pip...   OK
Checking for docker-compose...   OK
Starting WebODM...

Using the following environment:
================================
Host: localhost
Port: 8000
Media directory: appmedia
SSL: NO
SSL key: 
SSL certificate: 
SSL insecure port redirect: 80
Celery Broker: redis://broker
================================
Make sure to issue a ./webodm.sh down if you decide to change the environment.

docker-compose -f docker-compose.yml -f docker-compose.nodeodm.yml start || docker-compose -f docker-compose.yml -f docker-compose.nodeodm.yml up
Traceback (most recent call last):
  File "/usr/local/bin/docker-compose", line 7, in <module>
    from compose.cli.main import main
  File "/usr/local/lib/python2.7/dist-packages/compose/cli/main.py", line 17, in <module>
    import docker
  File "/usr/local/lib/python2.7/dist-packages/docker/__init__.py", line 6, in <module>
    from .client import Client, AutoVersionClient, from_env # flake8: noqa
  File "/usr/local/lib/python2.7/dist-packages/docker/client.py", line 11, in <module>
    from . import api
  File "/usr/local/lib/python2.7/dist-packages/docker/api/__init__.py", line 2, in <module>
    from .build import BuildApiMixin
  File "/usr/local/lib/python2.7/dist-packages/docker/api/build.py", line 9, in <module>
    from .. import utils
  File "/usr/local/lib/python2.7/dist-packages/docker/utils/__init__.py", line 2, in <module>
    from .utils import (
  File "/usr/local/lib/python2.7/dist-packages/docker/utils/utils.py", line 19, in <module>
    from .. import tls
  File "/usr/local/lib/python2.7/dist-packages/docker/tls.py", line 5, in <module>
    from .ssladapter import ssladapter
  File "/usr/local/lib/python2.7/dist-packages/docker/ssladapter/__init__.py", line 1, in <module>
    from .ssladapter import SSLAdapter # flake8: noqa
  File "/usr/local/lib/python2.7/dist-packages/docker/ssladapter/ssladapter.py", line 21, in <module>
    from backports.ssl_match_hostname import match_hostname
ImportError: No module named ssl_match_hostname

### What should be the expected behavior?

workin as appened in Kubuntu 17.10, same procedure.

### How can we reproduce this? (What steps did you do to trigger the problem? What parameters are you using for processing? If possible please include a copy of your dataset uploaded on Google Drive or Dropbox. Be detailed)

i would know
