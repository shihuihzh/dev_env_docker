# My develop environment

## How to use
1. Install docker and docker-componse
2. Change the source of the volumes. For exapmle
``` yaml
    volumes:
      - "/your/source/msyql/data:/var/lib/mysql"
      - "/your/source/mysql/conf.d:/etc/mysql/conf.d"
```
3. Use `docker-compose up -d` to run in background


## Services
1. MySQL - SQL Database. Bind to local `3306` and use `root` as password of `root` account by default.
2. Adminer - Simple SQL client. Bind to local `3300`. Use for MySQL management. Its network has linked to mysql. So it can use `mysql` as hostname to access MySQL
3. Redis - In memory data grid. Bind to local `6379`. No password by default
