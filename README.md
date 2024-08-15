# test_tecnico

## O Desafio

Construir uma pequena aplicação de ecommerce de acordo com o seguinte contexto: uma loja quer montar um site para vender seus produtos. Essa loja possui 2 fornecedores, que construíram uma API para você consumir e listar todos os produtos disponíveis nesta loja. O cliente deve ser capaz de filtrar e pesquisar por produtos específicos enquanto acessa o site. É importante que todos os produtos selecionados vão para um carrinho de compras. Além disso, você precisará registrar em um banco de dados cada compra realizada nesta loja com os dados do cliente e dos produtos comprados.

## Requisitos Implementados

* **Listar produtos**: Listar todos os produtos disponíveis pela dois fornecedores.
* **Opcao de filtro e pesquisa**: O cliente consegue pesquisar pelo nome do produto ou filtrar de acordo com sua preferência.
* **Pagina carrinho de compras**: Os produtos escolhidos vão para um carrinho de compras onde o usuario pode decidir compra-los.
* **Banco de dados**: Todos os produtos comprados são armazenados no banco e obtidos quando o usuario desejar ver suas compras.

## Tecnologias Utilizadas

* **Flutter**: Framework principal utilizado para o desenvolvimento da interface do usuário. <br>
* **Dart**: Linguagem de programação utilizada com o Flutter. <br>
* **NodeJs**: Utilizado como backend da aplicação, responsável por intermediar as requisições entre o frontend e as APIs dos fornecedores, gerenciar o carrinho de compras, e registrar as compras realizadas pelos clientes no banco de dados.
* **MongoDB**: Banco de dados NoSQL utilizado para armazenar os detalhes das compras realizadas.

## Estrutura do Projeto

implementacao/ <br>
├── lib/<br>
│   ├── components/  - Componentes reutilizáveis da UI. <br>
│   ├── models/  - Modelos do app. <br>
│   ├── pages/  - Páginas do app. <br>
│   ├── services/  - Chamadas as APIs. <br> 
│   ├── main.dart<br>
├──
├── pubspec.yaml<br>
└── README.md<br>

## Uso

Para rodar o aplicativo, siga os passos abaixo:

### 1. Clone o repositório

Primeiro, clone o repositório em sua máquina local usando o comando:

```
git clone [link do repositório]
```

### 2. Rodando o Backend (Node.js)

- Navegue até o diretório do backend:
  ```
  cd lib\services
  ```
- Instale as dependências:
  ```
  npm install
  ```
- Certifique-se de que o MongoDB está rodando localmente em sua máquina.
- Inicie o servidor Node.js
  ```
  node index.js
  ```
### 3. Rodando o Frontend (Flutter):

- Navegue até o diretório do projeto:
- Instale as dependências do Flutter
  ```
  flutter pub get
  ```
- Conecte um dispositivo ou use um emulador.
- Inicie o aplicativo Flutter:
  ```
  flutter run
  ```
  
### 4.Testando a aplicação:

Com o servidor Node.js rodando, e o aplicativo Flutter iniciado, você poderá testar todas as funcionalidades da aplicação.

## Processo de Desenvolvimento

### 1. **Planejamento**
   - Comecei identificando os principais requisitos da aplicação, como integração com dois fornecedores, gerenciamento do carrinho de compras e persistência de dados no banco de dados.
   - Decidi usar Node.js para o backend devido à sua capacidade de lidar com operações assíncronas e à facilidade de integração com APIs externas via `axios`. Além disso usei o `express` para construir a API do servidor.
   - Para o banco de dados, optei pelo MongoDB, que se alinha bem com a estrutura de dados não-relacional que a aplicação requer.

### 2. **Desenvolvimento Backend**
   - Implementei o servidor Node.js com as rotas necessárias para obter os produtos dos fornecedores, gerenciar o carrinho de compras, e registrar as compras no MongoDB.
   - Utilizei o `mongoose` para facilitar as operações com o banco de dados MongoDB e garantir a validação dos dados antes do armazenamento.

### 3. **Desenvolvimento Frontend**
   - No frontend, utilizei o Flutter para criar uma interface de usuário responsiva e moderna.
   - Configurei a comunicação com o backend usando `http` e assegurei que todas as funcionalidades do frontend estivessem sincronizadas com as operações do backend, como adicionar e remover produtos do carrinho.

### 4. **Testes**
   - Realizei testes manuais para verificar a integração entre o frontend e o backend, garantindo que as rotas do servidor respondessem corretamente e que o banco de dados estivesse armazenando as informações conforme esperado.

## Desenvolvido por Mateus de Almeida

Se tiver alguma dúvida ou sugestão, sinta-se à vontade para entrar em contato!

### Contato
- GitHub: https://github.com/Mateuszinnn
- LinkedIn: https://www.linkedin.com/in/mateusalmeidadias/
- Email: mateusdealmeida.trab@gmail.com
