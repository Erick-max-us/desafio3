
# Agenda de Contatos em Python

Este é um programa simples de agenda de contatos desenvolvido em Python. Ele permite cadastrar, listar, buscar e remover contatos de forma interativa pelo terminal.

## Funcionalidades

- **Cadastrar Contato**: Adiciona um novo contato à agenda com nome, telefone e e-mail.
- **Listar Contatos**: Exibe todos os contatos salvos na agenda.
- **Buscar Contato**: Permite encontrar um contato pelo nome ou número de telefone.
- **Remover Contato**: Remove um contato da agenda com base no nome ou telefone.
- **Sair**: Encerra o programa.

## Estrutura do Código

### Lista de Contatos
```python
agenda = []
```
Lista global que armazena os contatos como tuplas no formato `(nome, telefone, email)`.

### Funções

#### `cadastrar_contato(nome, telefone, email)`
Adiciona um novo contato à lista `agenda`.

#### `listar_contatos()`
Exibe todos os contatos cadastrados. Mostra uma mensagem se a agenda estiver vazia.

#### `buscar_contato(termo_busca)`
Busca contatos pelo nome (ignorando maiúsculas/minúsculas) ou número de telefone.

#### `remover_contato(termo_busca)`
Remove o primeiro contato encontrado que corresponda ao nome ou telefone fornecido.

#### `menu()`
Exibe o menu principal e executa as funções conforme a escolha do usuário. O loop continua até que o usuário escolha sair (`opção 5`).

### Observações
- Corrigir o erro de digitação na função `listar_contatos()`:
  - De: `enumer2ate(agenda)`
  - Para: `enumerate(agenda)`

## Execução

Para executar o programa, salve o código em um arquivo `.py` e rode com Python 3:

```bash
python agenda_contatos.py
```

## Exemplo de Uso

```
----- Agenda de Contatos -----
1. Cadastrar contato
2. Listar contatos
3. Buscar contato
4. Remover contato
5. Sair
```

## Licença

Uso educacional e livre para modificações.
