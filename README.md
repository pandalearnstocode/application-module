# application-module

## sub-modules in the application

* frontend [streamlit app] : https://github.com/pandalearnstocode/frontend-submodule
* backend [fastapi app] : https://github.com/pandalearnstocode/backend-submodule

## Project directory structure


```bash
.
├── backend-submodule # All the files related to backend lives here
│   ├── app
│   │   ├── __init__.py
│   │   └── main.py
│   ├── Dockerfile # backend docker file
│   ├── README.md
│   └── requirements.txt
├── docker-compose.yml # Docker-compose file to run all the sub-module from the app directory
├── frontend-submodule # All the frontend related sub-module lives here
│   ├── app
│   │   ├── app.py
│   │   ├── __init__.py
│   │   └── settings.py
│   ├── Dockerfile # frontend docker file
│   ├── README.md
│   └── requirements.txt
└── README.md 
```

## Adding sub-modules

```bash
git submodule add https://github.com/pandalearnstocode/frontend-submodule
git submodule add https://github.com/pandalearnstocode/backend-submodule
git add .
git commit -m "adding sub-modules."
git push origin develop
git config submodule.recurse true
```


## Cloning this repo

```bash
git clone https://github.com/pandalearnstocode/application-module.git
git submodule update --init
```


## Docker-compose

```bash
docker-compose build
docker-compose up
docker-compose down
```


## Reference:

* [Git Submodules Tutorial | For Beginners](https://www.youtube.com/watch?v=gSlXo2iLBro)