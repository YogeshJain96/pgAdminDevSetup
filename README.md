# pgAdminDevSetup
How to setup pgAdmin Dev Env Setup

```git clone https://github.com/postgres/pgadmin4.git```

```cd pgadmin4/```

```virtualenv -p python3 venv3```

```source env/bin/activate```

```cd web```

```pip3 --no-cache-dir install -r requirements.txt```
```yarn install ```
```yarn bundle ```

```python pgAdmin4.py```

> Troubleshooting 

OSError: [Errno 13] Permission denied: '/var/lib/pgadmin'

```mkdir /var/lib/pgadmin```
```sudo chown <uesr>:<user> /var/lib/pgadmin```

OSError: [Errno 13] Permission denied: '/var/log/pgadmin'

```mkdir /var/log/pgadmin```
```sudo chown <uesr>:<user> /var/log/pgadmin```
