🤝 Promises-Node.js

Este projeto tem como objetivo ensinar e demonstrar o uso de Promises em Node.js, uma forma moderna e mais clara de lidar com operações assíncronas, evitando o chamado callback hell.

Promises representam um valor que pode estar disponível agora, no futuro ou nunca, e permitem que você escreva código assíncrono de forma mais estruturada e legível.

📌 O que são Promises em Node.js?

No Node.js, Promises são um objeto que representa a eventual conclusão (ou falha) de uma operação assíncrona e seu valor resultante. Elas possuem três estados principais:

Pending: ainda em execução

Fulfilled: concluída com sucesso

Rejected: concluída com erro

Esse padrão ajuda a trabalhar com operações que demorariam para retornar — como leitura de arquivos, chamadas de API ou consultas a banco de dados — sem bloquear o restante do código.

🚀 Começando

Para executar este projeto localmente, siga os passos abaixo:

🧾 Pré-requisitos

Você precisa ter instalado:

Node.js (versão 12 ou superior)

npm ou Yarn como gerenciador de pacotes

📦 Instalar dependências

Após clonar o repositório:

git clone https://github.com/Douglas-Pedroso/promises-node.js
cd promises-node.js
npm install


ou com Yarn:

yarn

▶️ Como rodar

Para iniciar o projeto:

node index.js


ou (se foi configurado script no package.json):

npm start


Depois disso, você verá exemplos de Promises sendo executados no terminal — por exemplo, operações simuladas que resolvem ou rejeitam com base no tempo ou em valores retornados.

📌 O que este projeto demonstra

Este projeto mostra:

🎯 Criação de Promises simples
✔ Exemplo de função que retorna uma Promise, usando resolve e reject para controlar o resultado.

🔗 Encadeamento com .then() e .catch()
✔ Como lidar com resultados e erros de forma limpa e sequencial.

⚡ Uso de async/await (se implementado)
✔ Sintaxe moderna para trabalhar com Promises de forma parecida com código síncrono.

📊 Execução paralela com Promise.all() (se incluído)
✔ Como esperar vários processos assíncronos ao mesmo tempo.

🧪 Exemplos de uso
🟡 Criar uma Promise
const promise = new Promise((resolve, reject) => {
  setTimeout(() => {
    const success = true;
    if (success) {
      resolve("OK, operação concluída!");
    } else {
      reject("Algo deu errado.");
    }
  }, 1000);
});

promise
  .then(resultado => console.log(resultado))
  .catch(erro => console.error(erro));

📁 Estrutura do projeto
promises-node.js/
├── index.js            # Arquivo principal com exemplos de Promise
├── README.md           # Documentação deste projeto
└── package.json        # Configuração e scripts npm

💡 Onde as Promises são úteis

Promessas são fundamentais em Node.js para:

Leitura/escrita de arquivos sem bloquear o programa

Chamadas a APIs externas

Consultas a bancos de dados

Qualquer operação cuja resposta é demorada ou depende de recursos externos

🤝 Contribuindo

Contribuições são bem-vindas! Se você quiser sugerir melhorias ou adicionar exemplos:

Abra um fork do repositório

Crie uma branch com sua feature

Faça commit das suas alterações

Envie um Pull Request com a descrição clara das mudanças

📜 Licença

Este projeto pode ser licenciado conforme sua escolha (por exemplo, MIT).
