<p align="center">
<a target="blank"><img src="https://dmitripavlutin.com/static/6d14625626a323816b47d301a6319626/c24d5/cover.png" width="360" alt="Dot Logo" /></a>
</a>
<h1 align="center">Using props in React</h1>
<p align="center">Now I am going to show you how to use props in react</p>

## 🔍 What are Props?

Props are arguments passed into React components. Props are passed to components via HTML attributes. props stands for properties.

## 💻 Code
In this example, the Hello component has a property called: name

```jsx
<Hello name="Marc"/>
```

## ⚡ Example
```jsx
function Hello(props){
    return <h1>Hello {props.name}</h1>
}
```

### 🎈 Return to main page

- [Click](https://github.com/elmarcz/ReactTutos)
