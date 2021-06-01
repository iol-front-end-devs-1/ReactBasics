
# Table of Contents
- [Table of Contents](#table-of-contents)
- [React Basics](#react-basics)
  - [1. React JS Environment](#1-react-js-environment)
  - [2. Creating a react app - basics](#2-creating-a-react-app---basics)
  - [3. JSX(Javascript XML)](#3-jsxjavascript-xml)
  - [3. Creating Components](#3-creating-components)
  - [4. Props](#4-props)

<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>

# React Basics

## 1. React JS Environment
<br>

   + ### a. Install [VSCODE](https://code.visualstudio.com/download "Download VS CODE")

     + **VSCODE** is an open source code editor made by Microsoft. 

   <br>

   + ### b. Install [nodejs](https://nodejs.org/en/ "head to nodejs.org")
     + **Node.js** is an open-source, cross-platform, back-end JavaScript runtime environment that runs on the V8 engine and executes JavaScript code outside a web browser. <br>
     + npm is the default package manager for the JavaScript runtime environment Node.js.
 
<br>

## 2. Creating a react app - basics
   ```
      npx create-react-app
   ```
   + Create react app takes care of setting up all the things needed to make a react project.

<br>
<br>
<br>
<br>
<br>

## 3. JSX(Javascript XML)
 + looks like HTML but is still javascript
 + placed inside return statements <br>
  
   ```javascript
      //different ways of returning JSX. 1
      import React from 'react';

      function ComponentName(){
         return(
            <div>
               <h1>Hello World!</h1>
            </div>
         )
      }
   ```
   ```javascript
      //different ways of returning JSX. 2
      import React from 'react';

      const ComponentName = () => <div>
         <h1>Hello World!</h1>
      </div>
   ```
   ```javascript
      //different ways of returning JSX. 3
      import React from 'react';

      const ComponentName = () => {
         return (
            <div>
               <h1>Hello World!</h1>
            </div>
         )
      }
   ```
 + can output javascript directly inside
   ```javascript
      import React from 'react';

      //to output javascript code, just put the code inside {}
      const ComponentName = () => {
         var a = "Hello World!"

         return (
            <div>
               <h1>{a}</h1>
            </div>
         )
      }
   ```
 + accessing attributes in JSX 
      + attributes in  JSX are camelCase 
         ```javascript
             <div className="container">
               <button onClick={handleClick}>Click Me!</button>
               <input onChange={hanldeChange} />
             </div>
         ```
 + inline styling in JSX
      ```javascript
         <div style={{
            margin: "0 auto",
            display: flex,
            justifyContent:'space-around',
            alignItems:'center',
            flexDirection:'column',
            flexWrap:'wrap',
         }}>
           <div>One</div>
           <div>Two</div>
           <div>Three</div>
         </div>
      ```

<br>
<br>
<br>


## 3. Creating Components

<br>

   + ### a. Function Components
      ```javascript
         //base javascript
         import React from 'react';

         function ComponentName () {
            
            return(
               <div>
                  <h1>Hello World!</h1>
               </div>
            )
         }

         export default ComopnentName
      ```

      ```javascript
         //es6 style return component directly
         const ComopnentName = () => (
            <div>
               <h1>Hello World!</h1>
            </div>
         )
         export default ComponentName   
      ```

      ```javascript
         //es6 style execute some scripts inside function body
         const ComponentName = () => {

            const sum = 1+1

            return (
               <div>
                  <h1>Hello World!</h1>
                  <h1>The sum is {sum}</h1>
               </div>
            )
         }
         export default ComponentName   
      ```

<br>
<br>

  + ### b. Class Components

      <br>

      ```javascript 
         import React from 'react';
         class ComponentName extends React.Component {
            
            constructor(super){

            }

            render() {
               return (
                  <div>
                     <h1>Hello World!</h1>
                  </div>
               )
            }
         }
      ```



## 4. Props
   + What are props?
      + **“Props”** is a special keyword in React, which stands for properties and is being used for passing data from one component to another. 
      
   + Example
   
      ```javascript
         //Parent Component
         import React from 'react';
         import ChildComponent from './ChildComponent';

         const ParentComponent = () => {
            
            return(
               <div>
                  //you can pass prop the same way you put attributes in an html element
                  //the props names can be anything that you can think of
                  <ChildComponent name="Pizzarbonara" age={20} address="Philippines" />
               </div>
            )
         }
         
      ``` 
      
      ```javascript
         //Child Component
         import React from 'react';

         //to access the props, put props as arguments in your function
         const ChildComponent = (props) => {
            
            return(
               <div>
                  {/* to access specific props follow: props .propName */}
                  <h1>Hi my name is {props.name}</h1>
                  <h1>I am {props.age}</h1>
                  <h1>I am from the {props.address}</h1>
               </div>
            )
         }
         
      ``` 
