# Projeto Alura Food

O projeto Alura Food foi desenvolvido com o objetivo de praticar os conceitos de microsserviços ensinados no treinamento da Alura. Abaixo estão descritas as principais tecnologias utilizadas no projeto:

## Discovery Services com Eureka Server e Eureka Client
O Eureka Server e o Eureka Client são componentes do Spring Cloud Netflix que fornecem serviços de registro e descoberta de microsserviços. O Eureka Server é responsável por receber o registro dos serviços e disponibilizá-los para consulta, enquanto o Eureka Client é utilizado pelos serviços para registrar-se no servidor e descobrir outros serviços.

## API Gateway com Spring Cloud
O API Gateway é um componente do Spring Cloud que atua como ponto de entrada único para as requisições dos clientes. Ele redireciona as requisições para os serviços correspondentes com base nas regras de roteamento configuradas. Além disso, o API Gateway também pode realizar autenticação, autorização, balanceamento de carga e cache.

## Balanceamento de Carga com o Spring Cloud API Gateway
O Spring Cloud API Gateway inclui suporte embutido para balanceamento de carga entre várias instâncias de um mesmo serviço. Ele distribui as requisições de forma equilibrada entre as instâncias disponíveis, garantindo melhor desempenho e alta disponibilidade.

## Comunicação entre serviços com Spring OpenFeign
O Spring OpenFeign é uma biblioteca do Spring Cloud que simplifica a comunicação entre os serviços em uma arquitetura de microsserviços. Ele permite definir interfaces de cliente para os serviços e automaticamente realiza o mapeamento das requisições HTTP, proporcionando uma forma fácil e declarativa de consumir outros serviços.

## Circuit Breaker com Resilience4j
O circuit breaker é um padrão de projeto que visa melhorar a resiliência e a tolerância a falhas em sistemas distribuídos. O Resilience4j é uma biblioteca que implementa esse padrão e fornece recursos como limite de tempo de resposta, limite de tentativas, fallback e monitoramento das chamadas aos serviços. Isso ajuda a evitar que falhas em um serviço afetem toda a aplicação, permitindo um tratamento adequado das falhas.

Com o uso dessas tecnologias, o projeto Alura Food demonstra como construir uma arquitetura de microsserviços robusta e escalável, onde cada serviço é responsável por uma função específica e pode se comunicar com outros serviços de forma eficiente e confiável.
