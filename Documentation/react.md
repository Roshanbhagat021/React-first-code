<!-- What is React? -->
//React is free and open Source Javascript library , which helps us create cool UI interfaces using reusable ui components.




<!-- Who made React? -->
// React library is a creation of Facebook(now Meta) but the main ideation and execution was done by a software engineer of Meta named(Jordan Walke ) ,He was influenced by XHP, an HTML component library for PHP. And it was release on 29 May 2013.






<!-- What is Babel? -->
//Babel is like a translator which convert the JSX code into plain js code which browser can understands and execute.





<!-- How does Babel convert html code in React into valid code? -->
//Babel does not convert the exactly HTML code it does converts the JSX(HTML like code), it takes the JSX code and creates a function call of React.createElement() and convert the JSX code that browser can understand and execute.
<!-- ----------------------Example:----------------------- -->
<!-- JSX code  -->
<script type="text/babel">
        // Creating the element
        const element = (<>
            <div data="abc" className='massage'> Carpe diem</div>
            <h1>Hii....</h1>
        </>)

        // defining root element
        let rootElement = ReactDOM.createRoot(document.getElementById("root"))

        // Rendering the element to root element
        rootElement.render(element)
</script>
<!-- Converted code -->
"use strict";
var element = /_#**PURE**_/React.createElement(React.Fragment, null, /_#**PURE**_/React.createElement("div", {
data: "abc",
className: "massage"
}, " Carpe diem"), /_#**PURE**_/React.createElement("h1", null, "Hii...."));
var rootElement = ReactDOM.createRoot(document.getElementById("root"));
rootElement.render(element);





<!-- What is ReactDOM is used for ? write a example? -->
//ReactDOM is a package in React that provides DOM-specific methods that can be used to enable an efficient way of managing DOM elements and manipulate DOM. 

<!-- ----------------------Example:----------------------- -->
*Here we are rendering the element with the help of one of the methods of ReactDOM  (render)**

let rootElement = ReactDOM.createRoot(document.getElementById("root"))
        // Rendering the element to root element
        rootElement.render(element)




<!-- What are the packages that you need to import for react to work with? -->
// React 
// ReactDOM
// Babel   





<!-- How do you add react to a web application? -->
//BY adding this cdn links:
//<script crossorigin src="https://unpkg.com/react@18/umd/react.development.js"></script>
//<script crossorigin src="https://unpkg.com/react-dom@18/umd/react-dom.development.js"></script>







<!-- What is React.createElement? -->
//React.createElement is a method provided by react, which returns a React element object with few properties: type : The type you have passed. props : The props you have passed.





<!-- What are the three properties that createElement accept? -->
//type
//props
//children
<!-- ----------------------Example:----------------------- -->
React.createElement("div",{className:"greeting"},"Namaste")







<!-- What is the meaning of render and root? -->
//render-->Render is a method of ReactDOM library, which converts the react element into Dom element and attaches the element to the DOM .

//root-->The root is the HTML element where you want to display the result. It is like a container for content managed by React.