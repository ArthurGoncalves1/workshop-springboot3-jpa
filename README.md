# workshop-springboot3-jpa

# Sobre o projeto
Webservice com Spring Boot e JPA/Hibernate, que representa um modelo de domínio de uma loja, em que foram disponibilizadas diferentes URIs para suas 
entidades independentes, que são: Category, Product, Order e User. Suas exceções também foram tratadas. Esse projeto é parte do 
curso Java Completo, ministrado pelo professor Nélio Alves.

### Exemplo
```bash
(GET) http://localhost:8080/orders/2
{
    "id": 2,
    "moment": "2019-07-21T03:42:10Z",
    "orderStatus": "CANCELED",
    "client": {
        "id": 2,
        "name": "alex@gmail.com",
        "email": "977777777",
        "phone": "Alex Green",
        "password": "123456"
    },
    "items": [
        {
            "quantity": 2,
            "price": 1250.0,
            "subTotal": 2500.0,
            "product": {
                "id": 3,
                "name": "Macbook Pro",
                "description": "Nam eleifend maximus tortor, at mollis.",
                "price": 1250.0,
                "imgUrl": "",
                "categories": [
                    {
                        "id": 3,
                        "name": "Computers"
                    }
                ]
            }
        }
    ],
    "payment": null,
    "total": 2500.0
}
```

![Modelo de dominio](https://user-images.githubusercontent.com/76923742/211578652-bcd16add-bccb-43f7-bc96-04491bfa6dff.png)

## Tecnologias usadas
- Java
- Spring Boot
- Apache Tomcat
- Maven
- Banco de dados H2
- Postman

## Como executar o projeto
```bash
#Clonar Repositório
git clone https://github.com/ArthurGoncalves1/workshop-springboot3-jpa

# entrar na pasta do projeto back end
cd workshop-springboot3-jpa

# executar o projeto
./mvnw spring-boot:run

```


