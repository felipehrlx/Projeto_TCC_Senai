# FoodPLM - Plataforma de Gestão

O **FoodPLM** é um sistema web para a gestão do ciclo de vida de produtos (PLM - Product Lifecycle Management), controle de usuários e geração de relatórios dinâmicos. A aplicação possui uma interface responsiva no front-end que consome dados diretamente de uma API estruturada no back-end.

## 🛠️ Tecnologias Utilizadas

O projeto foi desenvolvido do zero focando em desempenho e simplicidade, utilizando as linguagens nativas:

- **Front-end:**
  - **HTML:** Estruturação semântica das páginas, painéis, formulários e modais.
  - **CSS:** Estilização responsiva, layout estruturado com Flexbox/Grid e uso de variáveis globais (`:root`) para consistência visual.
  - **JavaScript :** Manipulação dinâmica do DOM, controle de fluxos de telas, gerenciamento de modais e consumo da API nativa via `Fetch API`.

- **Back-end:**
  - **JavaScript :** Lógica do servidor, gerenciamento das rotas da API, regras de negócio e controle de autenticação/segurança.

- **Banco de Dados:**
  - **MySQL:** Banco de dados relacional encarregado do armazenamento seguro, persistente e estruturado de todas as entidades do sistema (Usuários e Relatórios).

---

## 📁 Estrutura de Arquivos

A organização do projeto separa de forma limpa as responsabilidades de interface, lógica visual e lógica de servidor:

```text
├── recuperacao.html     # Tela de recuperação de senha do usuário
├── Relatorios.html      # Painel de filtros, métricas e listagem de relatórios
├── usuarios.html        # Interface de gerenciamento e listagem da equipe
│
├── style.CSS            # Estilos globais da aplicação e do painel principal
├── Relatorios.css       # Layout e elementos específicos da área de relatórios
├── Usuario.CSS          # Design dedicado ao módulo de gestão de usuários
│
├── app.js               # Configuração e funções de integração direta com a API local
├── script.JS            # Comportamento do Dashboard (menus, tarefas e modais)
├── relatorios.js        # Lógica de criação dinâmica e exportação local de relatórios (CSV)
│
└── server.js            # Servidor back-end em JavaScript (Node.js) e tratamento de rotas

