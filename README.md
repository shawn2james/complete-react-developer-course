# Complete React Developer in 2021 (w/ Redux, Hooks, GraphQL)
[Udemy course](https://www.udemy.com/course/complete-react-developer-zero-to-mastery/)<br><br>

## Table of Contents
* [Lifecycle Methods](#lifecycle-methods)
    * [Mounting](#mounting)
    * [Updating](#updating)
    * [Unmounting](#unmounting)

## Lifecycle Methods
<a name="lifecycle-methods"></a>
[Lifecycle Methods Diagram](https://projects.wojtekmaj.pl/react-lifecycle-methods-diagram/)
<img src="images/lifecycle-methods.jpg" alt="Lifecycle Methods diagram">

### Mounting
<a name="mounting"></a>
The process of creating instances and DOM nodes corresponding to React components, and inserting them into the DOM, is called mounting.<br>
The <a href="https://reactjs.org/docs/react-component.html#componentdidmount">componentDidMount()</a> lifecycle method gets fired after the component is mounted.

### Updating
<a name="updating"></a>
A component gets updated when:
* its parent element gets rerendered
* a new state/props value is provided to the component
* the component is force updated using <a href="https://reactjs.org/docs/react-component.html#forceupdate">forceUpdate()</a> method

The <a href="https://reactjs.org/docs/react-component.html#componentdidupdate">componentDidUpdate()</a> lifecycle method gets fired after the component is updated.<br>

It is good practice to use the <a href="https://reactjs.org/docs/react-component.html#shouldcomponentupdate">shouldComponentUpdate</a> lifecycle method which returns a boolean value to specify whether the component should be rerendered.<br>
For example, the component need not be rerendered when the parent element gets updated, if the props passed to the component remains the same.

### Unmounting
<a name="unmounting"></a>
The process of removing a component from the DOM is called unmounting.<br>
The <a href="https://reactjs.org/docs/react-component.html#componentwillunmount">componentWillUnmount()</a> is called just before the component is unmounted.