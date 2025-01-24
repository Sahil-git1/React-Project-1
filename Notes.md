<h1>Day-1</h1>
Composability refers to the ability to combine or compose smaller, independent, and reusable components or elements to create more complex systems.

React -> Declarative , not imperative

Initially in react createElement("element",props,childElement) was used. To create element.

Now, JSX is used , inside react convert these jsx to call createElement() method. 

We use functions as components.

Vite recommend use .jsx if using jsx syntax.

 console.log(&lt;h1>Hello&lt;/h1>) -> return a object.

Declarative -> Describe. 

createRoot(document.getElementById('root')).render( Main()) -> Works !!

PascalCase.

&lt;Page>&lt;/Page> -> Works same
Components -> Functions which return react elements.

&lt;Fragment> or &lt;> -> Avoid unnecessary nested element in html.

className b'coz of ul.className = "" in js.

Index.jsx -> App.jsx -> main etc.

padding don't collapse like margin.

list::marker

---
## Data driven react apps
```
style={{color: "red"}}
```
- ### To style an element with the inline style attribute, the value must be a JavaScript object

- ### JavaScript expressions are written inside curly braces, and since JavaScript objects also use curly braces, the styling in the example above is written inside two sets of curly braces {{}}

- ### camelCased Property Names
```
const Header = () => {
  const myStyle = {
    color: "white",
    backgroundColor: "DodgerBlue",
    padding: "10px",
    fontFamily: "Sans-Serif"
  };
  return (
    <>
      <h1 style={myStyle}>Hello Style!</h1>
      <p>Add a little style!</p>
    </>
  );
}
```
- ### You can write your CSS styling in a separate file, just save the file with the .css file extension, and import it in your application.

## CSS Modules
- ### Another way of adding styles to your application is to use CSS Modules.

- ### CSS Modules are convenient for components that are placed in separate files.

- ### The CSS inside a module is available only for the component that imported it, and you do not have to worry about name conflicts.

- ### Create the CSS module with the .module.css extension, example: my-style.module.css.

- ### Create a new file called "my-style.module.css" and insert some CSS code in it:

```
my-style.module.css:
.bigblue {
  color: DodgerBlue;
  padding: 40px;
  font-family: Sans-Serif;
  text-align: center;
}



Car.js:
import styles from './my-style.module.css'; 

const Car = () => {
  return &lt;h1 className={styles.bigblue}>Hello Car!&lt;/h1>;
}

export default Car;
```

# Reusable Components
- Data driven.
## Props
- Importance of attributes in html tag.
- Use the { } for using js.

_Note_ : react get compiled  in js .

- Try to put logic of js  and { } separately.
- We can pass any data types to  react components.
_Note_ : props are js objects, run as many times as components are called.

---
<h1>Day-2</h1>

# Destructuring The Object 
```
const {img , name} = person // important to use same names
const {img : image} = person // to rename
``` 
- ### Props can destructure in function argument space.
```
func({name , img})
```
_Note_ : Use func(props) for better differ between outside and inside function vars .

## Conditional Rendering 
- ### {value && restOfCode} 
- ### React use js under the hood so we can use js inside style={{}} also.
- ### {condition ? TrueResult : FalseResult}

## Static Asset Handling
- ### Set paths inside the jsx like this
```
 import imgURL from "./img.png" 
```
- ### _B'coz the vite restructure the whole file structure_

<h1>Day-2</h1>
# map method
-  ### array.map(callback func)
## The rect don't render objects made by us. It just render the specific type of objects like &gt;h1>Hi&gt;h1>. (via create element method)

