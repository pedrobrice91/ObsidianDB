libreriasJS: Entorno con herramientas
NODE: ejecutar js en la terminal
npm: para descargar dependencia y paquetes
Dependencia: manejador de paquetes o codigo que viene de la web
framework:herramienta
npm init -y, crea un proyecto en node o se inicializa
Librería React - librería de js para crear interfases para el usuario, bien sea librerías o framework va a generar aplicaciones ==SPA, Aplicación que no recarga la pantalla==, si le instala módulos y paquetes puedes convertirlo en framework
React se enfoca solo en la vista (UI). No impone estructura, ni herramientas, ni forma de compilar. Por eso: Puedes usar React con Webpack, Vite, Parcel, Next.js, etc.
Puedes escribir en JavaScript o TypeScript.
Puedes manejar rutas con React Router o frameworks como Next.js.
1. aplicación web monolítica(MPA)  o web spa
frameworks Angular 

src > components todos los archivos van en mayus
npm install vite@4.5.0 para error en MAC

**SÍ necesitas** importar el JavaScript si quieres usar componentes interactivos como:

- Modales
- Dropdowns
- Tooltips
- Carouseles
- Collapse/Accordion

javascript

```javascript
import 'bootstrap/dist/css/bootstrap.min.css';
import 'bootstrap/dist/js/bootstrap.min.js';
```


==JSX==

| Tipo          | ¿Devuelve valor? | ¿Permite usar en JSX? | Ejemplo                    |
| ------------- | ---------------- | --------------------- | -------------------------- |
| **Expresión** | ✅ Sí             | ✅ Sí                  | `{user.name}`, `{2 * 3}`   |
| **Sentencia** | ❌ No             | ❌ No                  | `if (...) {}`, `for (...)` |

1 + 1               // devuelve 2
usuario.nombre      // devuelve el valor de nombre
true && "Hola"      // devuelve "Hola"
lista.map(fn)       // devuelve un nuevo array
() => "Hola"        // devuelve una función

![[Captura de pantalla 2025-08-20 113438.png]]

![[Captura de pantalla 2025-08-20 113524.png]]


![[Pasted image 20250820115550.png]]

ORM ==>pieza de software o la forma de interactuar la base de datos sin saber SQL, con programación orientada objeto

  

**React**

npx create-react-app nombredelaapp

npm install bootstrap

Dependencia **Bootstraps En el archivo index.js pegar** 

npm install react-router-dom

**En el archivo app.js pegar**

import { BrowserRouter, Routes, Route } from "react-router-dom";

Hooks => ==[props](https://www.youtube.com/watch?v=TLi0jQ8TYcg&list=PL2ZWqWbnARIMwG9v8AxrMTV45FcOrIDua&index=20), [useState](https://www.youtube.com/watch?v=3Ri2zAziTR8&list=PL2ZWqWbnARIMwG9v8AxrMTV45FcOrIDua&index=21), [useEffect(cicloDeVidaComponent)](https://www.youtube.com/watch?v=vls7SZ3cjb8&list=PL2ZWqWbnARIMwG9v8AxrMTV45FcOrIDua&index=25)==  
==[enventosOn(EntradaControLadas)](https://www.youtube.com/watch?v=W1tqLxVCSb8&list=PL2ZWqWbnARIMwG9v8AxrMTV45FcOrIDua&index=22), [fetch](https://www.youtube.com/watch?v=Qj-M8H9j3tw&list=PL2ZWqWbnARIMwG9v8AxrMTV45FcOrIDua&index=24), [react-router-dom](https://www.youtube.com/watch?v=oqISHy7n6AY&list=PL2ZWqWbnARIMwG9v8AxrMTV45FcOrIDua&index=26), [EstadoGlobal(FLUX(redux)`useContext`)](https://www.youtube.com/watch?v=VZvmgX10eVI&list=PL2ZWqWbnARIMwG9v8AxrMTV45FcOrIDua&index=27)==





Mvc, arquitectura hexagonal, solid. ERP, CRM


• 17. Expresiones regulares https://www.youtube.com/watch?v=MRKpVxn5fqI



  