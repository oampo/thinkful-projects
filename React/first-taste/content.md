## Build

Jackson Bros., a firm of personal injury shysters, have developed a React application to help them work out how much blame can be attributed in an accident, and what the total value of a lawsuit will be.  You have been asked to make some small tweaks to the application.

## Milestones

### Milestone 1: Add some new causes

[The application](http://codepen.io/jturner-thinkful/pen/bdXyOY) currently uses a React component called `Cause` to represent the causes of the accident.  Currently there are two possible causes of accident, sunshine and moonlight.  For example, if half of the blame can be attributed to moonlight then the component would look like this:

```
<Cause name="Moonlight">0.5</Cause>
```

To complete this milestone you should fork the app, and make it display accidents caused by Good Times, and Boogieing.

#### Sample Code

When you have completed this milestone, compare your code with [this sample](http://codepen.io/jturner-thinkful/pen/MwNdZz).

### Milestone 2: Add an icon prop

To improve the display of the causes, you have been asked to add an icon next to the cause name.  To achieve this you should add a new prop to the `Cause` component which contains the name of a [Font Awesome icon](https://fortawesome.github.io/Font-Awesome/).  For example, for Sunshine your Cause could look like this:

```js
<Cause name="Sunshine" icon="sun-o">0.1</Cause>
```

Then update the render method of the Cause component to display the icons.  The HTML output to display the icon should look like this:

```
<i class="fa fa-icon-name"></i>
```

#### Sample Code

When you have completed this milestone, compare your code with [this sample](http://codepen.io/jturner-thinkful/pen/qdeGgE).

### Milestone 3: Display the value of the lawsuit

Currently there is a placeholder where the total value of the lawsuit should be stored.  The value is the total amount of blame which has been attributed, multiplied by the value multiplier (which is stored in the `BlameCalculator` components' state).  So for example, if 10% of the blame has been attributed to Sunshine, and 5% to Moonlight, and the value multiplier is $10,000 then the total value would be $1,500.

Update the `BlameCalculator` component so that the correct value is displayed in the `<output>` tag.

#### Sample Code

When you have completed this milestone, compare your code with [this sample](http://codepen.io/jturner-thinkful/pen/oXKRVj).


