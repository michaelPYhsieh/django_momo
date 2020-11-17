# ABOUT THIS PROJECT
- Django, 
- Web Crawler: Selenium & bs4 
- PostgresSQL
- Asynchronous Scrapying
- Scheduled job for updating data
- d3.js SVG graph with url link
- docker


>This is a shopping site web crawler. Scrapy two section of products and creditcard data asynchronously in background, then store to database and cache file. Read data from cache and show tables and svg graph with product hyperlink when visiting.





# DOCKER DEPLOY

> `Pipfile.lock` file is in the folder `proj_dir`.

```
cd __folder

sudo docker-compose up

docker exec -ti __CID bash

# create su: admin/nimda
echo "from django.contrib.auth import get_user_model; User = get_user_model(); User.objects.create_superuser('admin', '', 'nimda')" | pipenv run python manage.py shell

# run task
pipenv run python manage.py qcluster

# then open http://127.0.0.1:8000/
```



---



---


# TODO 
- [x] Async
- [x] selenium - win and linux
- [x] schedule
- [x] models
- [x] key:val
- [x] d3.js
- [x] json
- [x] pgsql
- [x] docker: chrome
- [x] docker: createsu
- [x] docker: start qcluster
- [ ] django env
- [ ] logging
- [ ] new UI

---
