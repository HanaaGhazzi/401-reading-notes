# Component Composition 

- the component lifecycle:  The component lifecycle is exactly what it sounds like: it details the life of a component. Like us, components are born, do some things during their time here on earth, and then they die ☹️

![/](https://cdn-media-1.freecodecamp.org/images/1*U13Mlxz_ktcajaeJCyYkwg.png)

_A component can only be in one stage at a time. It starts with mounting and moves onto updating. It stays updating perpetually until it gets removed from the virtual DOM. Then it goes into the unmounting phase and gets removed from the DOM._

- Higher-Order Components HOCs:
is a function that takes a component and returns a new component.

- React State and setState():
The only way you should change state is via the setState method.

- React Context :
allows you to create global context objects that can be given to any component you make.This allows you to share data without having to pass props down all the way through the DOM tree

### Composition vs Inheritance

- Inheritance can be overused
- Composition of behavior can be simpler and easier
- React supports using composition over deep inheritance


#### Composition - When Inheritance?

- Facebook doesn't use inheritance beyond initial Component Classes
- Frontends can be built using a mixture of 'general' and 'specific' components
- Use Props to pass specific attributes and children to render specific behavior
- Behavior shared within Components such as logic or utilities can be shared as- JavaScript libraries or modules
- Using import is more useful and less restricting then extends

