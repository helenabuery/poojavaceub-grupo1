```mermaid
classDiagram
  class Usuario {
  - nome: string
  + cpf: int
}

  class Cliente {
  - nome: string
  + código: int
  - frequencia(): void
  -compras(): void
  - endereço(): string
}

class Funcionario {
  -nome: string
  -codigo: int
  -venda(): void
  -salario(): string
}

Funcionario <|-- Usuario
Cliente <|-- Usuario 

