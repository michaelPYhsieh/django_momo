
# DOCKER DEPLOY
```
cd xxx

sudo docker-compose up

docker exec -ti CID___ bash

# create su: admin/nimda
echo "from django.contrib.auth import get_user_model; User = get_user_model(); User.objects.create_superuser('admin', '', 'nimda')" | pipenv run python manage.py shell

# run task
pipenv run python manage.py qcluster

# then open http://127.0.0.1:8000/
```

- `Pipfile.lock` is in folder-`proj_dir`.

---

# ABOUT THIS PROJECT
- Django
- Web Crawler: Selenium & bs4 
- PostgresSQL
- Async. Scrapying supported
- Scheduled job for updating data
- d3.js SVG graph with url link


---


# TODO
- [x] DB
- [x] models
- [x] json
- [x] key:val
- [x] docker: chrome
- [x] docker: createsu
- [x] docker: start qcluster
- [ ] django env
- [ ] logging

---
