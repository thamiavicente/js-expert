# Introdução
Esse projeto tem por finalidade trazer um resumo do aprendizado obtido do curso "JS Expert", ministrado por Erick Wendel, e serve como um guia para quem quer aprender um pouco mais sobre JS, mas não tem ideia de por onde começar.

Entenda mais sobre assuntos como testes, ciclos de vida, regex e muito mais, de forma resumida e com exemplos inspirados no curso, mas feitos por mim.

Caso queira deixar um feedback, fique a vontade para usar a aba de issues.

# Sumário

# Instruções
Para rodar os testes presentes nesse projeto, basta fazer o clone do repositório e rodar o comando especificado no tópico.

**Exemplo:** Rodar testes de mock
1. Clone o repositório
2. Abra o diretório raiz do projeto no terminal
3. Rode o comando abaixo no terminal
   ``` javascript
   npm run test-mocks
   ```

# Testes

## Testes unitários

### Mocks
Mocks são objetos ou funções que simulam comportamentos de dependências reais em um teste. Eles permitem isolar o código em teste e verificar como ele interage com essas dependências, sem executar a lógica real delas.

No exemplo a seguir, temos uma função que recebe um arquivo e valida seu conteúdo. Nesse momento não precisamos testar as unidades de recebimento ou upload de arquivos, apenas se nosso código está validando o conteúdo corretamente.

#### **[Exemplo de mocks](https://github.com/thamiavicente/js-expert/tree/main/Exemplos/1-Mocks)**
``` javascript
    //Comando para executar os testes
    npm run test-mocks
```

### Stubs
Um stub é um pedaço de código que substitui uma dependência externa do código que está sendo testado, como por exemplo os dados de uma API. Ele é usado para fornecer respostas pré-definidas a chamadas feitas pelo código em teste, permitindo isolar e testar o comportamento da unidade com base nesses dados controlados.

O stub e o mock podem parecer a mesma coisa, mas, diferente do mock, o stub é utilizado para fornecer dados esperados ao teste, sem necessariamente verificar como esses dados são utilizados. Já o mock também verifica interações, por exemplo, se uma função foi chamada, quantas vezes, com quais argumentos etc. Ele é útil para testar o comportamento e a comunicação entre componentes.

A baixo você pode acessar um exemplo de stub, usado para testar o tratamento dos dados recebidos da API. Como os dados são mockados, não é preciso fazer requisição para a API para ter certeza que o tratamento de dados está funcionando corretamente.

#### **[Exemplo de stubs](https://github.com/thamiavicente/js-expert/tree/main/Exemplos/2-Stubs)**
``` javascript
    //Comando para executar os testes
    npm run test-stubs
```

### Spies

#### **[Exemplo de spies](https://github.com/thamiavicente/js-expert/tree/main/Exemplos/3-Spies)**
``` javascript
    //Comando para executar os testes
    npm run test-spies
```

# Conclusão

## Glossário e mais informações
Nessa seção você encontra alguns termos que apareceram durante o curso e que fui buscar mais informações sobre.
- **IIFE (Immediately Invoked Function Expression):** Um função que é definida e executada imediatamente após sua criação. (() => {...})(); 
- **Modos de importação e exportação no JS:**
  - **Module.export**
    - Usado no Node.js
    - Anterior ao suporte nativo de ESModules
    - Export:
    ``` javascript
        const saudacao = () => 'Olá!';
        module.exports = saudacao;
    ```
    - Import:
    ``` javascript
        const saudacao = require('./arquivo');
        console.log(saudacao());
    ```
  - **Export**
    - Usado em navegadores e também no Node.js com "type": "module" no package.json
    - Export:
    ``` javascript
        export default function saudacao() {
            return 'Olá!';
        }
    ```
    - Import
    ``` javascript
        import saudacao from './arquivo.js';
    ```
- **assert:** É um módulo que valida se determinada condição é verdadeira, caso não seja, retorna um erro
  
## Certificado
