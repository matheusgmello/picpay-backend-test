# Teste Técnico do PicPay 

Minha solução para o teste técnico do [PicPay](https://github.com/PicPay/picpay-desafio-backend) foi desenvolvida com o objetivo de criar um PicPay simplificado. Optei por adicionar testes unitários, tratamento de erros e seguir padrões de design.

# Configurações 

### Requisitos

- [Java](https://www.oracle.com/java/technologies/javase/jdk17-archive-downloads.html)

**Clone o projeto e acesse a pasta**

``` bash
git clone git@github.com:matheusgmello/picpay-backend-test.git && cd picpay-backend-test
```
- Rode a aplicação (`./mvnw spring-boot:run`)
- Teste a api no Rest Client no endereço (`localhost:8080`)

## Rotas


### GET `/users`

- Faz a listagem de usuários


### POST `/transactions`

- Faz uma transação para um usuário

#### Request Body
``` json
{
  "senderId": 1,
  "receiverId": 2,
  "value": 10
}
```

### POST `/users`

- Faz a criação de um novo usuário


#### Request Body
``` json

{
  "firstName": "Joao",
  "lastName": "Silva",
  "document": "123456789",
  "email": "joao@example.com",
  "type": "COMMON",
  "balance": 10
}

```

## Testes Unitários 

- Deve obter o usuário com sucesso do banco de dados.
- Não deve obter o usuário do banco de dados quando o usuário não existe.
- Deve criar a transação com sucesso quando tudo estiver OK.
- Deve lançar uma exceção quando a transação não é permitida.

## Tecnologias

- [Java](https://www.oracle.com/java/technologies/javase/jdk17-archive-downloads.html)
- [Spring Boot](https://spring.io/projects/spring-boot)
<!--START_SECTION:footer-->
<br />

## 🔗 Connect with me
[![LinkedIn](https://img.shields.io/badge/linkedin-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/matheusgmello)
[![Reddit](https://img.shields.io/badge/Reddit-%23FF4500.svg?style=for-the-badge&logo=Reddit&logoColor=white)](https://www.reddit.com/user/math7zw)
[![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/matheusgmello/)

<!--END_SECTION:footer-->