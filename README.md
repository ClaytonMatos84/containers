# Containers de Serviços para Desenvolvimento

Este repositório contém ambientes prontos para uso local de diversos serviços populares, utilizando Docker Compose. Ideal para desenvolvimento, testes e integração de aplicações.

## Serviços Disponíveis

- **MongoDB**: Banco de dados NoSQL orientado a documentos.
- **MySQL**: Banco de dados relacional amplamente utilizado.
- **PostgreSQL**: Banco de dados relacional avançado e open source.
- **RabbitMQ**: Broker de mensagens para filas e pub/sub.
- **WordPress**: Plataforma de CMS para blogs e sites.
- **n8n**: Plataforma de automação de workflows.

## Estrutura do Projeto

Cada serviço possui seu próprio diretório com arquivos `docker-compose.yml` e `Makefile` para facilitar a inicialização e gerenciamento dos containers. Alguns serviços possuem o diretório de `volumes` na própria pasta para persistência de dados.

```
mongodb/
mysql/
n8n/
postgres/
rabbitmq/
wordpress/
```

## Como Usar

1. Entre no diretório do serviço desejado, por exemplo:
   ```sh
   cd mongodb
   ```
2. Suba o serviço com Docker Compose:
   ```sh
   docker-compose up -d
   ```
   Ou utilize o Makefile (se disponível):
   ```sh
   make create
   ```

## Requisitos

- [Docker](https://www.docker.com/)
- [Docker Compose](https://docs.docker.com/compose/)
- (Opcional) [Make](https://www.gnu.org/software/make/)

## Observações

- Os arquivos de configuração podem ser customizados conforme a necessidade.
- Consulte o `docker-compose.yml` de cada serviço para detalhes de portas, volumes e variáveis de ambiente.
- Caso precise de variáveis de ambiente adicionar um arquivo .env na raiz do diretório desejado.

---

Sinta-se à vontade para contribuir ou sugerir melhorias!
