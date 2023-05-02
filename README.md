# 📝 Documentación sobre React

<br>
<br>

# 🟡Componente

Un componente es una parte de la interfaz de usuario independiente y reutilizable. Los componentes se pueden crear en dos formas:

<br>
<br>

# 🟡Componentes Funcionales

Un componente funcional es una función de JavaScript que devuelve un elemento de React.

<br>

## function Saludo(props) {

return < h1>¡Hola, {
    props.nombre}!< /h1 >;

## }

<br>
<br>

# 🟡Componentes de Clase

Un componente de clase es una clase de JavaScript que devuelve un elemento JSX.

<br>

## class Saludo extends React.Component {
  render() {
    return < h1>¡Hola, {this.props.nombre}!< /h1>;
  }
## }

<br>
<br>


# 🟡Declaración de componentes y diferencias de un Componente VS elemento

Los nombres de los Componentes siempre deben comenzar con una letra mayúscula. Por ejemplo: Saludo

Un Componente es el conjunto de varios elementos, los elementos son las etiquetas HTML y estas se pueden manipular con un identificador, en cambio un Componente es una pieza de todos estos elementos juntos, por ejemplo, un formulario es un Componente creado con div, inputs y buttons.

<br>

### Saber diferenciarlos es facil, en general:

* Componentes = < FormularioLogin>
* elemento o etiquetas = < div>

<br>

Nota: Los props siempre son jerárquicos (investiga herencia y polimorfismo) y se pueden llamar como argumentos, parámetros o como atributos de un objeto, como por ejemplo:

## props.nombre 

donde props hace referencia a un objecto y nombre a un parametro.

<br>
<br>

# 🟡Estado en React

Las alteraciones en las variables de props solo se podían hacer con componentes funcionales.

<br>
<br>

# 🟡Hooks

Un Hook es una función especial que permite trabajar con estados para componentes funcionales, lo que facilita el trabajo con estos.

<br>
<br>

# 🟡Event Listener / Event Handler

Un Event Handler es una función de JavaScript que se ejecuta cuando se produce un evento determinado. Por ejemplo, el evento

### onclick

<br>
<br>

# 🟡JSX

JSX es la combinación de HTML y JavaScript. JSX es opcional pero aumenta el flujo de trabajo si se utiliza.

## Ventajas de usar JSX:

* Facilidad de visualización y uso
* Solución de problemas más sencilla
* En JSX, se pueden utilizar propiedades CSS escritas en camelCase en el atributo style. Por ejemplo:

<br>

## const estiloDiv = {
  color: "yellow",
  backgroundColor: "green",
## };

## function Saludo() {
  return < div style={estiloDiv}>¡Hola, mundo!</ div>;
## }

<br>

O también se puede insertar un objeto de estilo JavaScript directamente en la etiqueta:

<br>

## function Saludo() {
  return < div style={{ color: "yellow", backgroundColor: "black" }}>¡Hola, mundo!< /div>;
## }

<br>
<br>

# 🟡Renderización

La renderización de los elementos de React se realiza con la librería ReactDOM.

<br>

## import ReactDOM from 'react-dom';

const elemento = < h1>Hola mundo!< /h1>;

## ReactDOM.render (
  elemento,
  document.getElementById('root')
## );

<br>
<br>

# 🟡Self-closing tags

En React, se pueden utilizar etiquetas self-closing, como por ejemplo

<br>

## < img src="url-imagen.jpg" />.

<br>
<br>

# 🟡Variables

En React, las variables se pueden utilizar dentro de las etiquetas utilizando llaves {}.

<br>

## let nombre = "El pepe";
### < p>Bienvenido {nombre}< /p>

<br>

También se pueden utilizar operaciones matemáticas:

<br>

## < p>El resultado es: {5 * 2}< /p>

<br>

Y métodos de strings:

<br>

## let nombre = "gino";
### < p>BIENVENIDO {nombre.toUpperCase()}< /p>

<br>
<br>

# 🟡Crea un proyecto React

Para crear un proyecto de React, primero necesitamos tener Node.js instalado correctamente. Luego, abrimos una carpeta en Visual Studio Code y abrimos la consola con CTRL + Ñ.

Para crear un nuevo proyecto de React, ejecutamos el siguiente comando en la consola:

<br>

## npx create-react-app mi-app

<br>

Nota: "mi-app" es el nombre del proyecto.

<br>

Una vez creado el proyecto, podemos iniciarlo con el siguiente comando en la consola:

## cd mi-app
## npm start

<br>

Para crear el proyecto en la carpeta actual, ejecutamos el siguiente comando en la consola:

## npx create-react-app .

<br>

De hacerlo de esta manera, simplemente seria ejecutar

<br>

## npm start

<br>
