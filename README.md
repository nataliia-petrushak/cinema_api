# Cinema API
API service for cinema management written on DRF

## Features
- JWT authentication
- Admin panel /admin/
- Documentation is located at /api/doc/swagger/
- Managing orders and tickets
- Creating movies with genres, actors
- Creating cinema halls
- Adding movie sessions
- Filtering movies and movie sessions

### Installing using GitHub
Install PostgresSQL and create db

```shell
git clone https://github.com/Amirammi/cinema_api.git
cd cinema_api
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
set DB_HOST=<your db hostname>
set DB_NAME=<your db name>
set DB_USER=<your db username>
set DB_PASSWORD=<your db password>
set SECRET_KEY=<your secret key>
python manage.py migrate
python manage.py runserver
```
### Run with docker
Docker should be installed

```shell
docker-compose build
docker-compose up
```

### Getting access
- create user via /api/user/register
- get access token via /api/user/token/

### Getting started
- Download [ModHeader](https://chrome.google.com/webstore/detail/modheader-modify-http-hea/idgpnmonknjnojddfkpgkljpfnnfcklj?hl=en)
- Add name and token
- Now you are authorised and can use the API
