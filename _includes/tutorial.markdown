{% raw %}
**Learn EmberJS. Quickly.**

To implement these concepts, you'll need a computer with the following installed

* node 0.10 or greater
* ember-cli

Ember For All aims to provide production-like examples to allow people to learn Ember in a way that gets them quick wins. These examples strive to be

* useful
* minimal
* production quality
* ordered to provide a gentle onramp

*Missing: initial setup & example repo*

## Example 0: Hello World

### New Concepts

+ components
+ properties
+ actions
+ set

## Component

### Create A Component

`$ ember g component hello-world`

### Use A Component

`{{hello-world}}`

### Change A Component

*app/templates/hello-world.hbs*

```handlebars
<h1>Hello World</h1>
```

<iframe width="560" height="315" src="https://www.youtube.com/embed/gh4ZNZP16m0?rel=0&amp;showinfo=0" frameborder="0" allowfullscreen></iframe>


## Property

*app/components/hello-world.js*

```es6
import Ember from 'ember';

export default Ember.Component.extend({
  greeting: 'Hi, World!!!',
});
```

*app/templates/hello-world.hbs*

```handlebars
<h1>{{greeting}}</h1>
```

<iframe width="560" height="315" src="https://www.youtube.com/embed/SjEDC6NYWtg?rel=0&amp;showinfo=0" frameborder="0" allowfullscreen></iframe>

## Action

*app/components/hello-world.js*

```es6
import Ember from 'ember';

export default Ember.Component.extend({
  greeting: 'Hi, world!!!',
  actions: {
    changeGreeting: function (time) {
      alert('Change greeting called.');
    }
  }
});
```

*app/templates/hello-world.hbs*

```handlebars
<h1 {{action "changeGreeting"}}>{{greeting}}</h1>
```

<iframe width="560" height="315" src="https://www.youtube.com/embed/Yv631LJuhAU?rel=0&amp;showinfo=0" frameborder="0" allowfullscreen></iframe>

## Set

*app/components/hello-world.js*

```es6
import Ember from 'ember';

export default Ember.Component.extend({
  greeting: 'Hi, world!!!',
  actions: {
    changeGreeting: function (time) {
      this.set('greeting', 'Goodbye, World!!11!');
    }
  }
});
```

*app/templates/hello-world.hbs*

```handlebars
<h1 {{action "changeGreeting"}}>{{greeting}}</h1>
```

<iframe width="560" height="315" src="https://www.youtube.com/embed/pgPlJZ7Tc9g?rel=0&amp;showinfo=0" frameborder="0" allowfullscreen></iframe>

## Example 1: Schedule Appointment

Review Concepts

+ components
+ properties
+ actions
+ set

New Concepts

+ if
+ each
+ action arguments

## Properties (Again)

<iframe width="560" height="315" src="https://www.youtube.com/embed/HenLjy4OnPc?rel=0&amp;showinfo=0" frameborder="0" allowfullscreen></iframe>

## Actions (Again)

<iframe width="560" height="315" src="https://www.youtube.com/embed/1GxP61MMx9o?rel=0&amp;showinfo=0" frameborder="0" allowfullscreen></iframe>

## Set (Again)

<iframe width="560" height="315" src="https://www.youtube.com/embed/4ApOyID6INo?rel=0&amp;showinfo=0" frameborder="0" allowfullscreen></iframe>

## If

<iframe width="560" height="315" src="https://www.youtube.com/embed/8Jc9rxeM9uU?rel=0&amp;showinfo=0" frameborder="0" allowfullscreen></iframe>

## Each Part 1

<iframe width="560" height="315" src="https://www.youtube.com/embed/v2IiwIcWhjw?rel=0&amp;showinfo=0" frameborder="0" allowfullscreen></iframe>

## Each Part 2

<iframe width="560" height="315" src="https://www.youtube.com/embed/FD6t17voyeg?rel=0&amp;showinfo=0" frameborder="0" allowfullscreen></iframe>

## Actions (Arguments)

<iframe width="560" height="315" src="https://www.youtube.com/embed/rjFB8htKizE?rel=0&amp;showinfo=0" frameborder="0" allowfullscreen></iframe>

{% endraw %}
