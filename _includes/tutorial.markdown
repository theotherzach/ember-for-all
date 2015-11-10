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

### Create A Component

`$ ember g component hello-world`

### Use A Component

`{{hello-world}}`

### Change A Component

*app/templates/hello-world.hbs*

```handlebars
<h1>Hello World</h1>
```

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


Example 1: Hello World

Review Concepts

+ components

New Concepts



Example 2: Schedule Appointment

Review Concepts

+ components
+ properties
+ actions
+ set

New Concepts

+ if
+ each
+ action arguments
{% endraw %}
