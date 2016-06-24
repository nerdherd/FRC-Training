# Object Oriented Programming
Java is an object oriented programming language, meaning it is centered around objects and their methods. This lesson will first discuss the basic principles of objects and then delve deeper into actual coded examples.
### Objects
Imagine common household objects -- a lamp, for instance. The lamp has two states: on or off. You can change the state of the lamp by flipping a switch. This may seem like a simple analogy, but it covers most of the basics of object oriented languages. In this case, your object is the lamp, and the action you invoke -- the method -- is what changes the state of the lamp. If we were coding this, we might write something like this:
```
class Lamp {
	Lamp(){}
	void switch() {
		//Turn the light on or off 
	}
}
```