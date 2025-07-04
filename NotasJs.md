libreriasJS:Entorno con herramientas
NODE: ejecutar js en la terminal
npm: Instalar paquetes
Dependencia: manejador de paquetes o codigo que viene de la web
framework:herramienta
npm init -y, crea un proyecto en node o se inicializa
React crear interfaz de usuario

React se enfoca solo en la vista (UI). No impone estructura, ni herramientas, ni forma de compilar. Por eso:
Puedes usar React con Webpack, Vite, Parcel, Next.js, etc.
Puedes escribir en JavaScript o TypeScript.
Puedes manejar rutas con React Router o frameworks como Next.js.

src > components todos los archivos van en mayus
npm install vite@4.5.0


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

| Tipo          | ¿Devuelve valor? | ¿Permite usar en JSX? | Ejemplo                    |
| ------------- | ---------------- | --------------------- | -------------------------- |
| **Expresión** | ✅ Sí             | ✅ Sí                  | `{user.name}`, `{2 * 3}`   |
| **Sentencia** | ❌ No             | ❌ No                  | `if (...) {}`, `for (...)` |

1 + 1               // devuelve 2
usuario.nombre      // devuelve el valor de nombre
true && "Hola"      // devuelve "Hola"
lista.map(fn)       // devuelve un nuevo array
() => "Hola"        // devuelve una función
