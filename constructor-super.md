# Without `super()`

```jsx
class A {
  constructor() {
    this.a = 'hello'
  }
}

class B extends A {
  constructor(){
    console.log(this.a) //throws an error
  }
}

console.log(new B())
```

# With `super()`

```jsx
class A {
  constructor(props) {
    this.props = props
  }
}

class B extends A {
  constructor(props) {
    super(props)
    console.log(this.props)
  }
}

console.log(new B({title: 'hello world'}))
```