# Lista de Tarefas Simples

Uma aplicação web frontend leve e intuitiva para gerenciar tarefas pessoais, construída com HTML, CSS e JavaScript. Utiliza localStorage para persistência local e oferece uma interface amigável com temas claro e escuro. Este projeto é ideal para aprendizado ou uso em ambientes onde não há necessidade de um backend.

## Demonstração

Confira a versão hospedada em [https://todolist-marcelomd-projects.vercel.app](https://todolist-marcelomd-projects.vercel.app).

![Lista de Tarefas](./assets/frontend.png)

## Funcionalidades

- **Adicionar tarefas**: Insira novas tarefas com um clique.
- **Marcar como feita**: Altere o status das tarefas com facilidade.
- **Apagar tarefas**: Remova tarefas indesejadas rapidamente.
- **Filtrar tarefas**: Busque tarefas por texto no campo de filtro.
- **Alternar temas**: Troque entre modos claro e escuro clicando no título.
- **Persistência local**: Armazena dados usando `localStorage` do navegador.

## Estrutura do Projeto

```text
/javascript_to_do_list_frontend
├── /assets
│   └── frontend.png
├── /src    
│   ├── /public
│   │     ├── index.html
│   │     ├── script.js
│   │     └── style.css
│   └── index.js          
├── .gitignore
├── package-lock.json
├── package.json
└── README.md
```

## Instalação e execução

Para rodar o projeto localmente, siga os passos:

1. **Clone o repositório**:

   ```bash
   git clone https://github.com/marcelomduarte/javascript_to_do_list_frontend.git
   ```

2. **Acesse o diretório**:

   ```bash
   cd javascript_to_do_list_frontend
   ```

3. **Instale as dependências**:

   ```bash
   npm install
   ```

4. **Inicie a aplicação**:

   ```bash
   npm start
   ```

5. **Acesse em**: `http://localhost:8080`.

## Backend (opcional)

Originalmente, este projeto frontend foi projetado para se comunicar com uma API RESTful. O repositório do backend está disponível em [https://github.com/marcelomduarte/javascript_to_do_list_backend](https://github.com/marcelomduarte/javascript_to_do_list_backend). Se desejar usar o backend em vez do localStorage do navegador, siga os passos abaixo.

### Reverter o frontend para usar a API

Para restaurar a versão do frontend que se conecta ao backend (em vez de usar `localStorage`), volte dois commits no repositório do frontend após o clone:

   ```bash
   git reset --hard HEAD~2
   ```

- **Nota**: Este comando reverte o frontend para um estado anterior onde ele estava configurado para se comunicar com a API de Tarefas

### Configurar e executar o backend localmente

1. **Clone o repositório do backend**:

   ```bash
   git clone https://github.com/marcelomduarte/javascript_to_do_list_backend.git
   ```

2. **Acesse o diretório do backend**:

   ```bash
   cd javascript_to_do_list_backend
   ```

3. **Instale as dependências do backend**:

   ```bash
   npm install
   ```

4. **Inicie o servidor do backend**:

   ```bash
   npm start
   ```

### Integração

- Após iniciar o backend, o frontend (revertido com `git reset`) automaticamente se conectará à API em `http://localhost:3000`.

- Consulte o `README.md` no repositório do backend ([https://github.com/marcelomduarte/javascript_to_do_list_backend](https://github.com/marcelomduarte/javascript_to_do_list_backend)) para detalhes adicionais, como configuração de variáveis de ambiente ou dependências específicas.
