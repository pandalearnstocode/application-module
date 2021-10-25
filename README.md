# application-module

## sub-modules in the application

* frontend [streamlit app] : https://github.com/pandalearnstocode/frontend-submodule
* backend [fastapi app] : https://github.com/pandalearnstocode/backend-submodule

## Adding sub-modules

```
git submodule add https://github.com/pandalearnstocode/frontend-submodule
git submodule add https://github.com/pandalearnstocode/backend-submodule
git add .
git commit -m "adding sub-modules."
git push origin develop
git config submodule.recurse true
```


## Cloning this repo

```
git clone https://github.com/pandalearnstocode/application-module.git
git submodule update --init
```


## Reference:

* [Git Submodules Tutorial | For Beginners](https://www.youtube.com/watch?v=gSlXo2iLBro)