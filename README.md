<p align="center">
  <img src="docs/banner.png" alt="VOSS Luxury Bags - telas do sistema da loja" width="100%">
</p>

<h1 align="center">👜 Telas — VOSS Luxury Bags</h1>

<p align="center">
  Protótipo navegável das telas de um sistema para a <b>VOSS</b>, loja fictícia de bolsas de luxo: vitrine,
  coleção, produto, carrinho, login por perfil e painéis internos de gerente, administrador, vendedor e atendente.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5">
  <img src="https://img.shields.io/badge/Tailwind%20CSS-CDN-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white" alt="Tailwind CSS">
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript">
  <img src="https://img.shields.io/badge/Font%20Awesome-6.5-528DD7?style=for-the-badge&logo=fontawesome&logoColor=white" alt="Font Awesome">
</p>

<p align="center">
  <a href="#-sobre-o-projeto">Sobre</a> •
  <a href="#-funcionalidades">Funcionalidades</a> •
  <a href="#-telas">Telas</a> •
  <a href="#-como-executar">Como executar</a> •
  <a href="#-estrutura-do-projeto">Estrutura</a> •
  <a href="#-tecnologias">Tecnologias</a>
</p>

---

## 📌 Sobre o projeto

Conjunto de **21 telas em HTML** que simulam o sistema de uma loja de bolsas de luxo: a parte pública (vitrine,
coleção, produto e carrinho) e as áreas internas de cada perfil de usuário. Os dados exibidos (clientes, vendas,
metas, valores) são fixos no HTML ou gerados no navegador, apenas para demonstração; não há back-end.

## ✨ Funcionalidades

| | Recurso | Descrição |
|---|---|---|
| 🛍️ | **Vitrine** | Página inicial da loja com destaque, diferenciais e acesso à coleção e ao login |
| 👜 | **Coleção** | 45 bolsas geradas por JavaScript, com preços sorteados a cada carregamento |
| 🏷️ | **Produto e carrinho** | `produto.html?id=1` (a 3) mostra o produto; "Adicionar ao Carrinho" grava no `localStorage` e o carrinho lista e remove itens |
| 🔐 | **Login por perfil** | Contas de demonstração levam ao painel de cada perfil (veja abaixo) |
| 📝 | **Cadastro de cliente** | Formulário de criação de conta |
| 📊 | **Painel do gerente** | Indicadores, últimas atividades e menu de usuários, módulos, perfis e financeiro |
| 🧩 | **Perfis e permissões** | Tabela de permissões (visualizar, editar, excluir) por módulo |
| 💼 | **Área do vendedor** | Dashboard, clientes, vendas e metas do mês |
| 🛠️ | **Admin e atendente** | Painéis próprios com os acessos de cada perfil |

### 🔑 Contas de demonstração (`login.html`)

O login é só uma simulação em JavaScript (sem servidor). Todas usam a senha `123456`:

| E-mail | Vai para |
|---|---|
| `gerente@voss.com` | `dashboard-gerente.html` |
| `admin@voss.com` | `dashboard-admin.html` |
| `vendedor@voss.com` | `dashboard-vendedor.html` |
| `atendente@voss.com` | `dashboard-atendente.html` |
| `cliente@voss.com` | `cliente.html` (página ainda não criada) |

## 🖼️ Telas

<table>
  <tr>
    <td align="center"><b>Vitrine</b><br><img src="docs/screenshots/index.png" alt="Vitrine"></td>
    <td align="center"><b>Coleção</b><br><img src="docs/screenshots/colecao.png" alt="Coleção"></td>
  </tr>
  <tr>
    <td align="center"><b>Produto</b><br><img src="docs/screenshots/produto.png" alt="Produto"></td>
    <td align="center"><b>Login</b><br><img src="docs/screenshots/login.png" alt="Login"></td>
  </tr>
  <tr>
    <td align="center"><b>Painel do gerente</b><br><img src="docs/screenshots/gerente.png" alt="Painel do gerente"></td>
    <td align="center"><b>Perfis e permissões</b><br><img src="docs/screenshots/perfis.png" alt="Perfis e permissões"></td>
  </tr>
  <tr>
    <td align="center"><b>Área do vendedor</b><br><img src="docs/screenshots/dashboard-vendedor.png" alt="Área do vendedor"></td>
    <td align="center"><b>Celular</b><br><img src="docs/screenshots/mobile.png" alt="Vitrine no celular" width="260"></td>
  </tr>
</table>

## 🚀 Como executar

Não há build nem dependências locais:

```bash
git clone https://github.com/kauaxp77/Telas.git
cd Telas
```

Depois, abra o `index.html` no navegador. É preciso internet: o Tailwind CSS, o Font Awesome e as imagens são
carregados de CDNs/links externos.

## 📁 Estrutura do projeto

```
Telas/
├── index.html                 # Vitrine da loja
├── colecao.html               # Coleção de bolsas (gerada por JS)
├── produto.html               # Detalhe do produto (?id=1 a 3)
├── carrinho.html              # Carrinho (localStorage)
├── login.html                 # Login com redirecionamento por perfil
├── cadastro-cliente.html      # Criação de conta
├── dashboard-gerente.html     # Painel do gerente
├── gerente.html               # Painel do gerente (indicadores e atividades)
├── painel.html                # Painel geral
├── usuarios.html              # Configuração de usuários
├── modulos.html               # Configuração de módulos
├── perfis.html                # Perfis e permissões
├── financeiro.html            # Financeiro
├── interface.html             # Painel administrativo (usuários e módulos)
├── dashboard-admin.html       # Painel do administrador
├── dashboard-atendente.html   # Painel do atendente
├── dashboard-vendedor.html    # Área do vendedor
├── painel-vendedor.html       # Dashboard do vendedor
├── clientes.html              # Clientes do vendedor
├── vendas.html                # Vendas do vendedor
├── metas.html                 # Meta do mês
└── docs/
    ├── banner.png
    └── screenshots/           # Capturas de tela deste README
```

## 🛠️ Tecnologias

- **HTML5**
- **Tailwind CSS** (Play CDN): estilos
- **JavaScript**: coleção, produto, carrinho (`localStorage`) e login simulado
- **Font Awesome 6.5**: ícones

## 👨‍💻 Autor

Desenvolvido por **[kauaxp77](https://github.com/kauaxp77)**.

<p align="center">⭐ Se curtiu o projeto, deixe uma estrela!</p>
