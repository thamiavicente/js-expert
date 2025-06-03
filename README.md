# Introdução
Esse projeto tem por finalidade trazer um resumo do aprendizado obtido do curso "JS Expert", ministrado por Erick Wendel, e serve como um guia para quem quer aprender um pouco mais sobre JS, mas não tem ideia de por onde começar.

Entenda mais sobre assuntos como testes, ciclos de vida, regex e muito mais, de forma resumida e com exemplos inspirados no curso, mas feitos por mim.

Caso queira deixar um feedback, fique a vontade para usar a aba de issues.

# Sumário

# Testes

## Testes unitários

### Mocks
Os mocks são unidades de código que simulam unidades reais. Com elas vocês consegue validar trechos de código de forma independente, sem precisar do resultado de outras unidades.

No exemplo a seguir, temos uma função que recebe um arquivo e valida seu conteúdo. Nesse momento não precisamos testar as unidades de recebimento ou upload de arquivos, apenas se nosso código está validando o conteúdo corretamente.

**[Exemplo de mocks](https://github.com/thamiavicente/js-expert/tree/main/Exemplos/1-Mocks)**

# Conclusão

## Glossário e mais informações
Nessa seção você encontra alguns termos que apareceram durante o curso e que fui buscar mais informações sobre.
- **IIFE (Immediately Invoked Function Expression):** Um função que é definida e executada imediatamente após sua criação. (() => {...})(); 
- **Modos de importação e exportação no JS:**
**Module.export**
- Usado no Node.js
- Anterior ao suporte nativo de ESModules
- Export:
const saudacao = () => 'Olá!';
module.exports = saudacao;
- Import:
const saudacao = require('./arquivo');
console.log(saudacao());
**Export**
- Usado em navegadores e também no Node.js com "type": "module" no package.json
- Export:
export default function saudacao() {
  return 'Olá!';
}
- Import
import saudacao from './arquivo.js';
- **assert:** Valida se determinada condição é verdadeira, caso não seja, returna "error"
  
## Certificado
