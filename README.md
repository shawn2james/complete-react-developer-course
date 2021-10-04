# Complete React Developer in 2021 (w/ Redux, Hooks, GraphQL)
[Udemy course](https://www.udemy.com/course/complete-react-developer-zero-to-mastery/)<br><br>

# Table of Contents
* [Key React Concepts](#react-concepts)
* [The job of a React developer](#job-of-react-developer)
* [Lifecycle Methods](#lifecycle-methods)
    * [Mounting](#mounting)
    * [Updating](#updating)
    * [Unmounting](#unmounting)

## Key React Concepts
<a name="react-concepts"></a>
1. Don't touch the DOM. I'll do it
2. Build websites like lego blocks
3. Unidirectional data flow (data i.e. state, props always moves to the lower components)
4. UI, the rest is up to you

## The job of a React developer
<a href="job-of-react-developer"></a>
1. Decide on components
2. Decide the state and where it lives
3. What changes when state changes

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