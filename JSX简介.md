```
// Hello Wrold
ReactDOM.render(<h1>Hello World</h1>, document.getElementById('helloWorld'))

//JSX
function formatName(user) {
  return user.firstName + ' ' + user.lastName
}

//JSX 表达式
function getGreeting(user) {
  if (user) {
    return <h1>Hello, {formatName(user)}!</h1>
  }
  return <h1>Hello, Stranger.</h1>
}

const user = {
  firstName: 'Harper',
  lastName: 'Perez'
}

//JSX 属性
const content = 'My React'
const contentStyle = {
  color: 'red',
  //React DOM 使用 camelCase 小驼峰命名 来定义属性的名称
  fontWeight: 'bold'
}

//JSX 嵌套
const element = (
  <div className="jsx">
    {getGreeting(user)}
    <h4 title={content} style={contentStyle}>
      {content}
    </h4>
  </div>
)
ReactDOM.render(element, document.getElementById('jsx'))
```
