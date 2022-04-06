# codepix
O CodePix é um projeto para fins de estudo do Bootcamp Imersão Full Cycle.

O projeto envolve uma aplicação que faz a intermediação de transações Pix entre bancos.

Como requisitos a aplicação deve:
- Não pode perder transações, mesmo que esteja offline ou um o banco destino esteja offline
- Deve ser capaz de trabalhar com filas de transações e criações de chaves Pix
- Deve ser capaz de validar/criar novas chaves Pix
- Deve ser capaz de validar/criar contas e bancos para as quais a transação será realizada.

# O que foi utilizado
Para este projeto foi utilizada a linguagem Go.

Foi aplicada uma metodologia de arquitetura hexagonal, onde temos entidadeds que possuem suas regras de negócio definidas e disponibilizam métodos publicos representando o que essa entidade pode fazer....


# Comandos aulas
```
Comandos Docker
  para iniciar os containers:
    docker-compose up -d

  Para listar os containers:
    docker-compose ps

  Para entrar no Container em modo iteração:
    docker exec -it [Nome do container] bash


Comandos Go

  Para rodar os testes:
    go test ./...

Comando protoc

  protoc --go_out=application/grpc/pb --go_opt=paths=source_relative --go-grpc_out=application/grpc/pb --go-grpc_opt=paths=source_relative --proto_path=application/grpc/protofiles application/grpc/protofiles/*.proto


Comando client grpc evans
	evans -r repl
  
  Dentro do evans é possível fazer uma call com o comando `call` e o nome do servico disponibilizado pelo servidor grpc
```