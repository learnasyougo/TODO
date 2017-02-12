# JavaScript Hoisting
> Hoisting is JavaScript's default behaviour of moving declarations to the top. Mind the **declarations** part, not the **assignment**.

## Declaration vs Value assignment
It's important to note, as done above, that only the declarations are being hoisted to the top - not the initialization / assignment.

```
var person = "Yves Schelpe";
alert(person.toString());

// Output: alert window with content "Yves Schelpe"
```

And...

```
person = "Yves Schelpe";
alert(person);
var person = "John Doe";

// Output: alert window with content "Yves Schelpe"
```

But...

```
alert(person);
var person = "John Doe";

// Output: alert window with content "undefined"
```

#### References
- http://www.w3schools.com/js/js_hoisting.asp