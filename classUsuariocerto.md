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


´´´mermaind
class Funcionario {
    -String nome:
    -int id
    +Funcionario(int id, String)
    +CadastrarProduto (Produto p) void
    +consultarProduto (int código) Produto
    +gerarVenda() Venda 
    +consultarVenda(int id) Venda
}

class Usuario {
    -String nome
    -String login
    String senha
    +Usuario(String nome, String login, String senha)
    +fazerLogin(String login, String senha) 

}

class Cliente {
    -String nome
    -String cpf
    -String telefone
    +Cliente(String nome, String cpf, String telefone)
    +fazerCadastro() void
    +consultarProduto(int código) Produto
    +realizarCompra() Compra  

}

Funcionario <|-- Usuario
Cliente <|-- Usuario
