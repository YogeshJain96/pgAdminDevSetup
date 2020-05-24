# pgAdminDevSetup
How to setup pgAdmin Dev Env Setup

> Clone Git Repo

```git clone https://github.com/postgres/pgadmin4.git```

```cd pgadmin4/```

> Create Virtual Env (Python3)

```virtualenv -p python3 venv3```

> Activate Virtual Env

```source env/bin/activate```

> Install Python Dependency

```pip3 --no-cache-dir install -r requirements.txt```

```cd web```

> Install Node Dependency

```yarn install ```
```yarn bundle ```

> Run WebApp

```python pgAdmin4.py```

## Troubleshooting 

OSError: [Errno 13] Permission denied: '/var/lib/pgadmin'

```mkdir /var/lib/pgadmin```
```sudo chown <uesr>:<user> /var/lib/pgadmin```

OSError: [Errno 13] Permission denied: '/var/log/pgadmin'

```mkdir /var/log/pgadmin```
```sudo chown <uesr>:<user> /var/log/pgadmin```

## To Reset the Password of pgAdmin

> Remove whatever is there inside .pgadmin

FYI:In Ubuntu the path of STORAGE_DIR is **/home/yogesh/.pgadmin/**

```cd /home/yogesh/.pgadmin/```

```rm -rf *```
