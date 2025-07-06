Pipenv  para descargar dependencia y paquetes

**Back**

Python —version
Pip —version
Pipenv —version

**Flask**

pipenv shell (ambiente virtual)
pipenv install instala dependencia
pipenv install flask flask-sqlalchemy flask-migrate flask-cors

pipenv install flask_jwt_extended flask-bcrypt

flask db init (para crear las carpetas)
flask db migrate (para crear el arechivo db)
flask db upgrade (para migrar las columnas)


### Pasos para instalar y usar `virtualenv` desde cero en Windows

#### 1. **Verifica que Python esté en el PATH**

Ejecuta esto en PowerShell o CMD:

`python --version`

`py --version`

#### 2. **Instala virtualenv**

`pip install virtualenv`

⚠️ Si el comando `pip` no funciona, prueba:

`python -m ensurepip --upgrade python -m pip install --upgrade pip python -m pip install virtualenv`

#### 3. **Crea el entorno virtual**

`python -m virtualenv env`

O si prefieres usar una versión específica de Python:

`virtualenv -p python env`

---

#### 4. **Activa el entorno virtual**

`.\env\Scripts\Activate.ps1`

En CMD:

bash

CopiarEditar

`.\env\Scripts\activate.bat`

---

#### 5. **Verifica que el entorno está activo**

Verás algo así en el prompt:

bash

CopiarEditar

`(env) PS C:\tu\proyecto>`


Back python para la web

Flask .- libreria, microframework  posee gran cantidades de dependencias para integrar a nuestros sistemas 

Django .- frameworks, gran variedad de herramienta, ya tiene un orm, paquetes, todo lo que necesitas ya lo tienen integrado
