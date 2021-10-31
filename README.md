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
