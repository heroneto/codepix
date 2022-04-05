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