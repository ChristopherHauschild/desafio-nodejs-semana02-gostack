<div align="center">
  <img src="https://github.com/ChristopherHauschild/bootcamp-gostack-13-rocketseat/blob/master/gostack.png?raw=true">
</div> <br />

<div align="center">
  <img src="https://img.shields.io/static/v1?label=nodejs&message=backend&color=success&style=for-the-badge&logo=NODE.JS"/>
</div>

# <p align="center">Desafio - Primeiro projeto com Node.js</p>

:information_source: <i>Códigos desenvolvidos durante o desafio Primeiro projeto com Node.js, na segunda semana do Bootcamp GoStack 13, ofertado pela plataforma de ensino [Rocketseat](https://rocketseat.com.br/).</i>

<p align="justify">
Esse desafio tem como objetivo fixar os conhecimentos aprendidos em Node.js junto ao TypeScript, utilizando o conceito de models, repositories e services. A mesma consiste numa aplicação para armazenar transações financeiras de entrada e saída, permitindo o cadastro e a listagem dessas transações.
</p>

## :twisted_rightwards_arrows: Rotas da aplicação:

- **`POST /transactions`**: A rota deve receber `title`, `value` e `type` dentro do corpo da requisição, sendo `type` o tipo da transação, que deve ser `income` para entradas (depósitos) e `outcome` para saídas (retiradas). Ao cadastrar uma nova transação, ela deve ser armazenada dentro de um objeto com o seguinte formato :

```json
{
  "id": "uuid",
  "title": "Salário",
  "value": 3000,
  "type": "income"
}
```

- **`GET /transactions`**: Essa rota deve retornar uma listagem com todas as transações que você cadastrou até agora, junto com o valor de soma de entradas, retiradas e total de crédito. Essa rota deve retornar um objeto com o formato a seguir:

```json
{
  "transactions": [
    {
      "id": "uuid",
      "title": "Salário",
      "value": 4000,
      "type": "income"
    },
    {
      "id": "uuid",
      "title": "Freela",
      "value": 2000,
      "type": "income"
    },
    {
      "id": "uuid",
      "title": "Pagamento da fatura",
      "value": 4000,
      "type": "outcome"
    },
    {
      "id": "uuid",
      "title": "Cadeira Gamer",
      "value": 1200,
      "type": "outcome"
    }
  ],
  "balance": {
    "income": 6000,
    "outcome": 5200,
    "total": 800
  }
}
```

## :pushpin: Maiores informações:

Para encontrar maiores informações sobre o desafio, como por exemplo o template utilizado e a bateria de testes implementadas, você pode acessar este [link](https://github.com/rocketseat-education/bootcamp-gostack-desafios/tree/master/desafio-fundamentos-nodejs).

<hr>

Códigos desenvolvidos por Christopher Hauschild Schott

