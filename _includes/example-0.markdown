{% raw %}
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

<iframe width="560" height="315" src="https://www.youtube.com/embed/eSrTQcFh3kY?rel=0&amp;showinfo=0" frameborder="0" allowfullscreen></iframe>


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

<iframe width="560" height="315" src="https://www.youtube.com/embed/ZigWewtisuI?rel=0&amp;showinfo=0" frameborder="0" allowfullscreen></iframe>

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

<iframe width="560" height="315" src="https://www.youtube.com/embed/Y9xAMBdiYOw?rel=0&amp;showinfo=0" frameborder="0" allowfullscreen></iframe>

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

<iframe width="560" height="315" src="https://www.youtube.com/embed/AxU0Ryb12Z0?rel=0&amp;showinfo=0" frameborder="0" allowfullscreen></iframe>

{% endraw %}
