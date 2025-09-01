# 🎲 Sorteio de Números Aleatórios

[![Versão](https://img.shields.io/badge/version-1.0.0-blue)]()
[![Status](https://img.shields.io/badge/status-em%20desenvolvimento-orange)]()
[![Licença](https://img.shields.io/badge/licença-MIT-green)]()

---

## 📝 Descrição

Este projeto é um **sorteador de números aleatórios únicos**, com interface simples em HTML e JavaScript.
O usuário pode escolher a quantidade de números, o intervalo mínimo e máximo, e o sistema garante que **nenhum número se repita**.

---

## 💻 Tecnologias Utilizadas

* HTML5
* CSS3
* JavaScript (ES6)

---

## ⚙️ Funcionalidades

* Validação de campos vazios ou inválidos
* Geração de números aleatórios dentro de um intervalo definido
* Garantia de que **não haverá números repetidos**
* Botão de reiniciar para limpar os campos e resultados
* Feedback visual ao habilitar/desabilitar o botão de reiniciar

---

## 🛠️ Como Usar

1. Abra o arquivo `index.html` no navegador.
2. Preencha os campos:

   * **Quantidade**: número de números a serem sorteados
   * **De**: número mínimo do intervalo
   * **Até**: número máximo do intervalo
3. Clique em **Sortear**.
4. O resultado será exibido na tela, separado por vírgulas.
5. Clique em **Reiniciar** para limpar os campos e fazer um novo sorteio.

---

## 📌 Estrutura do Projeto

```
/sorteio-numeros
│
├── index.html           # Estrutura HTML da aplicação
├── style.css            # Estilo CSS
└── script.js            # Funções JavaScript (sorteio e reinício)
```

---

## 🔧 Código Principal (JS)

```javascript
function sortear() {
    let quantidade = parseInt(document.getElementById('quantidade').value);
    let de = parseInt(document.getElementById('de').value);
    let ate = parseInt(document.getElementById('ate').value);
    
    let sorteados = [];
    let numero;

    if (isNaN(quantidade) || quantidade == 0 || isNaN(de) || isNaN(ate)) {
        alert('Preencha todos os campos corretamente');
        return;
    }

    if (quantidade > (ate - de + 1)) {
        alert("Quantidade maior que o intervalo de números disponíveis!");
        return;
    }

    for(let i = 0; i < quantidade; i++ ) {
        numero = obter
```
