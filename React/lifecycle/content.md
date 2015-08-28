## Build

One of your colleagues is having a hard time understanding what happens in what order in a React app.  React apps are full of initial states, mounting and unmounting, updates and renders.  What are they all for, and when do they run?

To answer the question you decide that the best solution is to [get meta](http://cdn.gifbay.com/2013/04/infinite_patrick-45487.gif), and write a React app which demonstrates the React lifecycle.


## Milestones

### Milestone 1: Displaying events

Create a simple component which sets up an `events` state, which will contain a list of the events which have taken place.  In the render method you should return a `ul` containing each of the events in `<li>`s.

The events list should initially contain a string describing how the `getInitialState` method has been called.  This should be the only `li` which you see initially.

#### Sample Code

When you have completed this milestone, compare your code to [this sample](http://codepen.io/jturner-thinkful/pen/OyLJJO).

### Milestone 2: The easy parts - `componentWillMount` and `componentDidMount`

Add `componentWillMount` and `componentDidMount` methods to your component.  These will be called before and after the component has been mounted in the DOM respectively.  In the methods you should add strings to the events list, describing what has taken place.

#### Sample Code

When you have completed this milestone, compare your code to [this sample](http://codepen.io/jturner-thinkful/pen/PPYowJ).

### Milestone 3: The smelly parts - `shouldComponentUpdate` and `componentWillUpdate`

Add `shouldComponentUpdate` and `componentWillUpdate` methods to the component.  The `shouldComponentUpdate` method will be called each time the props or state are updated.  If it returns true then the component will be re-rendered, otherwise it will not.  If `shouldComponentUpdate` returns true, then `componentWillUpdate` is called before each render.

Updating the state in these methods is considered very harmful.  But as we have no other way of signalling that the events have taken place, so just this once you should hold your nose and directly update the state without using `this.setState`.

#### Sample Code

When you have completed this milestone, compare your code to [this sample](http://codepen.io/jturner-thinkful/pen/epOYYo).

### Milestone 4: The recursive part - `componentDidUpdate`

Add a `componentDidUpdate` method which calls `setState` to add an event to the list in the correct way.  This method will be called after each render.

But now there is a problem: if you update the state following a `render`, then another update loop will start.  You will enter an infinite loop.  To escape the loop, keep a `count` variable in the state which is incremented in `componentDidUpdate` method.  Then only return true in `shouldComponentUpdate` for the first five loops through the lifecycle.

#### Sample Code

When you have completed this milestone, compare your code to [this sample](http://codepen.io/jturner-thinkful/pen/MagWYL).
