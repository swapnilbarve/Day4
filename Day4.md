1.What are react life cycles explain each one with examples?

=>Each component in React has a lifecycle which you can monitor and manipulate during its three main phases. The three phases are: Mounting, Updating, and Unmounting.

=>Mounting:

*constructor(): The constructor() method is called before anything else, when the component is initiated, and it is the natural place to set up the initial state and other initial values.

*getDerivedStateFromProps(): The getDerivedStateFromProps() method is called right before rendering the element.

*render(): The render() method is required, and is the method that actually outputs.

*componentDidMount(): The componentDidMount() method is called after the component is rendered.

=>Updating:

*getDerivedStateFromProps(): updates the getDerivedStateFromProps method is called. This is the first method that is called when a component gets updated.

*shouldComponentUpdate(): shouldComponentUpdate() method you can return a Boolean value that specifies whether React should continue with the rendering or not.

*render(): render() method is of course called when a component gets updated, it has to re-render the HTML to the DOM, with the new changes.

*getSnapshotBeforeUpdate(): getSnapshotBeforeUpdate() method you have access to the props and state before the update, meaning that even after the update, you can check what the values were before the update.

*componentDidUpdate(): componentDidUpdate method is called after the component is updated in the component.

=>ummount:

*componentWillUnmount(): The componentWillUnmount method is called when the component is about to be removed from the 

component.




=========================================================================================================================





2.UseReducer Hook:

=>The useReducer Hook returns the current state and a dispatch method. 
implementation part===> https://codesandbox.io/s/throbbing-shape-4kw0xp?file=/src/App.js 



========================================================================================================================

3.UseMemo Hook:

=>It returns a memoized value and it only runs when one of its dependencies update.

implementation part===> https://codesandbox.io/s/blissful-glitter-gbbv8z?file=/src/App.js


=======================================================================================================================

4.UseRef Hook:

=>The useRef Hook allows you to persist values between renders.

implementation part===> https://codesandbox.io/s/muddy-resonance-8nqbbw?file=/src/App.js


=======================================================================================================================

5.context Api:

=>The React Context API is a way for a React app to effectively produce global variables that can be passed around. This is the alternative to "prop drilling" or moving props from grandparent to child to parent, and so on. Context is also touted as an easier, lighter approach to state management using Redux.


======================================================================================================================



6.props drilling:

=>Prop drilling refers to the process of sending props from a higher-level component to a lower-level component. To pass the props down from the topmost component, we must do something like this: However, prop drilling can become an issue in itself because of its repetitive code.

state uplifting:

=>In React, sharing state is accomplished by moving it up to the closest common ancestor of the components that need it. This is called “lifting state up”


======================================================================================================================



7.useEffect:

=>The motivation behind the introduction of useEffect Hook is to eliminate the side-effects of using class-based components. For example, tasks like updating the DOM, fetching data from API end-points, setting up subscriptions or timers, etc can be lead to unwarranted side-effects.

useContext:

=>The useContext hook is the new addition in React . The useContext accepts the value provided by React. createContext and then re-render the component whenever its value changes but you can still optimize its performance by using memorization.

