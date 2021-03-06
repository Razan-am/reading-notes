## **Component Based Architecture**

### ***What is a component?***

- The component is a modular, portable, replaceable, and reusable set of well-defined functionality. It is also considered as a software object, intended to interact with other components.
- The software component can be defined as a unit of composition with a contractually specified interface and explicit context dependencies only.


### ***What are the charactistics of a component?***

- **Reusability**: components are resuable. 

- **Replaceable**: it can be freely replaced with other similar components.

- **Not context specific**: they are been designed to operate in different environments and contexts.

- **Extensible**: component can be extended from existing components to provide new behavior.

- **Encapsulated**: it's allow the caller to use its functionality.

- **Independent**: components are designed to have minimal dependencies on other components.

### ***What are the advantages of using component based architecture?***

- **Ease of deployment**
- **Reduced cost**
- **Ease of development**
- **Reusable**
- **Modification of technical complexity**
- **Reliability**
- **System maintenance and evolution** 
- **Independent**

---------------------------------------------------

## **What is Props and How to Use it in React**

- `React` is a component-based library which divides the UI into little reusable pieces. In some cases, those components need to communicate which send data to each other and the way to pass data between components is by using `props`.

### ***What is props short for?***

- `Props` is a special keyword in React, which stands for properties and is being used for passing data from one component to another.
It's  being passed in a uni-directional flow`one way from parent to child`.

### ***How are props used in React?***

-  The props are used in react by following these steps:
   1. Firstly, define an attribute and its value(data).
   2. Then pass it to child component(s) by using Props.
   3. Finally, render the Props Data.

### ***What is the flow of props?***

- Props can only be passed to components in one-way `parent to child`, and it data is immutable `read-only` which means that data coming from the parent should not be changed by child components.

-------------------------------------------------------

## Things I want to know more about:
- I want to know more about the react and it's uses and how it will helped me as a developer.

----------------------------------------------------

**References:**

@tutorialspoint/[Component-Based Architecture
](https://www.tutorialspoint.com/software_architecture_design/component_based_architecture.htm)


@Cem Eygi/[What is Props and How to Use it in React
](https://itnext.io/what-is-props-and-how-to-use-it-in-react-da307f500da0)