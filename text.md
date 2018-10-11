# Ciclo de vida do React

![React 16 Lifecycle](https://cdn-images-1.medium.com/max/2000/1*cEWErpe-oY-_S1dOaT1NtA.jpeg)

## constructor

O `contructor` é o primeiro método a ser chamado no componente React. Ele é chamado antes de o component ser "montado". Ele que irá contruir o componente trazendo todas as funcionalidades de um componente React.

Para entender como funcionar o `super` do constructor olhar o arquivo [constructor-super.md](./constructor-super.md)

## render

Você sempre precisar ter o método `render`, porque é ele que fala para o React o que ele tem que mostrar na tela. Sem ele o seu component não irá funcionar.

## componentDidMount

Esse método é chamado depois do componente ter renderizado pelo primeira vez. Aqui é o local certo para você fazer os seus requests para APIs. E caso haja uma mudança no `state`, o render é chamado novamente.

## shouldComponentUpdate

O `shouldComponentUpdate` é o cara que decide se o seu componente deve ou não ser atualizado. Quando ele retoranar `true` ele atualiza, quando retorna `false` ele não atualiza. O React ja faz ele lógica para você, então normalmente você não precisa se preocupar com isso. 

## componentDidUpdate

O `componentDidUpdate` é chamado após o seu componente ter sido atualizado

## Outros métodos

Existem alguns métodos do ciclo de vida do React que não existem mais e alguns que estão parando de serem usado. Esses métodos são os que começam com `componentWill...`. (`componentWillMount`, `componentWillReceiveProps`, `componentWillUpdate`)

Na versão 16 do React alguns métodos novos foram criados (`getDerivedStateFromProps`, `getSnapshotBeforeUpdate`, `componentDidCatch`), mas a gente verá eles aqui, porque eles não são tão importantes e dão uma complexidade muito grande. A gente também não irá ver o `componentWillUnmount`, que apesar de começar com `componentWill..` ele ainda é utilizado.

# bind.(this)
[Link para o Medium](https://medium.com/tableless/https-medium-com-tableless-react-this-bind-so-sei-que-e-assim-73e75f2adbd3)






