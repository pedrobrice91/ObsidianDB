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







- **Variables y Tipos de Datos**
    
    - Tipos primitivos: `int`, `float`, `str`, `bool`, `None`
        
    - Conversión de tipos (`int()`, `str()`, `float()`)
        
- **Operadores**
    
    - Aritméticos, lógicos, comparación, asignación
        
    - `is` y `in` (similares a `typeof` / `instanceof` en comportamiento)
        
- **Estructuras de Control**
    
    - Condicionales: `if`, `elif`, `else`
        
    - Bucles: `for`, `while`
        
    - Control de flujo: `break`, `continue`, `pass`
        
- **Funciones**
    
    - Definición: `def`
        
    - Parámetros, retorno
        
    - Argumentos `*args`, `**kwargs`
        
    - Funciones lambda (anónimas)
        
    - Closures y funciones anidadas
        
- **Ámbito (Scope) y el uso de `global` y `nonlocal`**
    
    - Local, global, enclosing y built-in scopes (LEGB rule)
        
- **Manejo de errores**
    
    - `try`, `except`, `finally`, `else`
        
    - Tipos de excepciones (`ValueError`, `TypeError`, etc.)
        
    - Definir tus propias excepciones
        
- **Clases y Programación Orientada a Objetos**
    
    - `class`, `__init__`, atributos, métodos
        
    - Herencia, polimorfismo, encapsulamiento
        
    - Métodos mágicos (`__str__`, `__repr__`, `__len__`, etc.)
        
- **Módulos y Paquetes**
    
    - `import`, `from ... import`, `as`
        
    - Crear y organizar tus propios módulos
        
    - Uso del entorno virtual (`venv`)
        
- **Colecciones (estructuras de datos)**
    
    - `list`, `tuple`, `set`, `dict`
        
    - Métodos asociados
        
    - Iteración y comprensión de listas (`list comprehensions`)
        
- **Expresiones Regulares**
    
    - Módulo `re`
        
    - Búsqueda, sustitución, validación de patrones
        
- **Funciones avanzadas**
    
    - Decoradores
        
    - Generadores (`yield`)
        
    - Iteradores personalizados
        
- **Programación Funcional**
    
    - `map`, `filter`, `reduce`, `zip`
        
    - Uso de funciones como objetos de primera clase
        
- **Manejo de Archivos**
    
    - `open()`, lectura, escritura
        
    - Manejo con `with`
        
- **Programación Asíncrona**
    
    - `async def`, `await`, `asyncio`
        
    - Tareas concurrentes
        
- **Estructuras de Datos Avanzadas**
    
    - `collections`: `deque`, `defaultdict`, `Counter`, `namedtuple`
        
    - `heapq`, `queue`
        
- **Sets y Diccionarios (equivalentes a Sets y Maps en JS)**
    
- **Bases de datos**
    
    - Uso de SQLite con `sqlite3`
        
    - ORMs como SQLAlchemy
        
- **Testing**
    
    - `unittest`, `pytest`
        
- **Tipado estático opcional**
    
    - `type hints` (`def func(x: int) -> str:`)
        
    - Uso de `mypy` o `pyright` para análisis estático
        
- **Buenas prácticas y estilo**
    
    - `PEP8`
        
    - Linting con `flake8`, `black`
