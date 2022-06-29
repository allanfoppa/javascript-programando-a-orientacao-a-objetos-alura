# JAVASCRIPT - PROGRAMANDO A ORIENTAÇÃO A OBJETOS ALURA

## ATRIBUTOS PRIVADOS

Esta em fase 3: #privateAttribute  
Link da proposta [aqui](https://github.com/tc39/proposal-class-fields#private-fields)  

A convenção diz que utliza-se: _privateAttribute, diferente do # esse pode sim ser acessado. Mas, tratar como privado.

```javascript
class MyClass {
  // Public
  name;
  // Private
  // #age
  _age;

  method() {
    // logic here
  }

}
```

## COMPOSIÇÃO DE CLASSES

Uma classe utiliza outra, podendo fazer o uso de seus atributos e lógica.

## GERENCIAMENTO DE MEMÓRIA

[Link](https://medium.com/reactbrasil/como-o-javascript-funciona-gerenciamento-de-mem%C3%B3ria-como-lidar-com-4-vazamentos-comuns-de-5cfa341b9e39)

## GETTERS E SETTERS

```javascript
class Aluno {
  constructor(nome, curso, semestre){
    this.nome = nome,
    this.curso = curso,
    this.semestre = semestre
  }
  get nomeAluno(){
    return this.nome
  }
  set nomeAluno(nomeAluno) {
    this.nome = nomeAluno
  }
}

let lucas = new Aluno('', 'Engenharia', 5)
lucas.nomeAluno = 'Lucas'
console.log(lucas.nome) //Lucas
```

## CONSTRUTORES

Construtores são utilizados para inicializar os atributos
