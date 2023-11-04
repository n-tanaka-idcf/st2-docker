```
$ python3.8 -m venv .venv

$ source .venv/bin/activate

❯ pip install st2client                                                                                                   
Collecting st2client                                                                                                      
  Using cached st2client-3.7.0.tar.gz (114 kB)                                                                            
  Preparing metadata (setup.py) ... done                                                                                  
Collecting argcomplete==1.12.2                                                                                            
  Using cached argcomplete-1.12.2-py2.py3-none-any.whl (38 kB)                                                            
Collecting cffi<1.15.0                                                                                                    
  Downloading cffi-1.14.6-cp38-cp38-manylinux1_x86_64.whl (411 kB) 
<omit>
Installing collected packages: wcwidth, sseclient-py, pytz, python-editor, ply, jsonschema, chardet, argcomplete, zipp, urllib3, typing-extensions, six, pyyaml, pysocks, pycparser, prettytable, orjson, idna, decorator, certifi, requests, python-dateutil, prompt-toolkit, jsonpath-rw, importlib-metadata, cffi, cryptography, pyOpenSSL, st2client
  Running setup.py install for jsonpath-rw ... done
  Running setup.py install for st2client ... done
Successfully installed argcomplete-1.12.2 certifi-2022.9.24 cffi-1.14.6 chardet-3.0.4 cryptography-3.4.7 decorator-5.1.1 idna-2.10 importlib-metadata-3.10.1 jsonpath-rw-1.4.0 jsonschema-2.6.0 orjson-3.5.2 ply-3.11 prettytable-2.1.0 prompt-toolkit-1.0.15 pyOpenSSL-21.0.0 pycparser-2.21 pysocks-1.7.1 python-dateutil-2.8.1 python-editor-1.0.4 pytz-2021.1 pyyaml-5.4.1 requests-2.25.1 six-1.13.0 sseclient-py-1.7 st2client-3.7.0 typing-extensions-4.1.1 urllib3-1.26.12 wcwidth-0.2.5 zipp-3.10.0
WARNING: You are using pip version 22.0.4; however, version 22.3.1 is available.
You should consider upgrading via the '/home/nbchk/work/github.com/codequokka/st2-docker/.venv/bin/python3.8 -m pip install --upgrade pip' command.

$ docker-compose down
<omit>

$ docker-compose up -d
<omit>

$ st2 login st2admin --write-password
Password:         # Ch@ngeMe
Logged in as st2admin

$ st2 whoami
Currently logged in as "st2admin".

Authentication method: authentication token
Authentication token expire time: 2022-11-19T23:49:21Z

RBAC:
 - Enabled: False
 - Roles:
```
