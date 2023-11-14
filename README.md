# validacao-formulario
Código JS para validação de formulário em tempo real. Valida campos customizados destacando inputs válidos/inválidos. Usa funções reutilizáveis de estilização. Bloqueia envio do form com erros. Arquitetura em camadas separando responsabilidades. Permite extensão fácil para novos campos. Organização e reuso de código.
# Formulário com Validação em JavaScript

Este repositório contém um exemplo de código JavaScript para validação de formulário.

## Funcionalidades

- Validação em tempo real dos campos:
  - Username (mínimo 3 caracteres)
  - Email (formato válido) 
  - Senha (não vazio)
  - Confirmar Senha (igual a senha)

- Feedback visual ao usuário:
  - Destaca em verde campos válidos
  - Destaca em vermelho e exibe mensagem de erro para campos inválidos

- Bloqueia envio do formulário caso algum campo esteja inválido

## Arquitetura

- `functions.js`: funções reutilizáveis 
  - `togglePopup()`: exibe/oculta popup nos campos
  - `estilizarInputCorreto()`: adiciona estilo de sucesso
  - `estilizarInputIncorreto()`: adiciona estilo de erro

- `validation.js`: lógica de validação de cada campo
  - Ouve eventos e chama funções reutilizáveis
  - Armazena estado em objeto `inputsCorretos`

- `form.js`: 
  - Previne envio do form se houver campos inválidos
  - Exibe modal de sucesso ou erro  

## Tecnologias

- JavaScript
- DOM Manipulation
- CSS Dinâmico



