<p align="center">
  <img src="assets/docs/banner-dev.svg" width="100%" alt="Portfólio Dev - ETE Porto Digital"/>
</p>

<p align="center">
  <img src="https://img.shields.io/github/stars/WallaceMichael/portfolio-dev-etepd?style=flat&color=818CF8" />
  <img src="https://img.shields.io/github/last-commit/WallaceMichael/portfolio-dev-etepd?style=flat&color=F472B6" />
  <img src="https://img.shields.io/badge/status-ativo-4ade80?style=flat" />
  <img src="https://img.shields.io/badge/license-MIT-818CF8?style=flat" />
</p>

---

## 💡 Sobre o projeto

Portfólio desenvolvido durante a oficina prática de **Git e GitHub** na [ETE Porto Digital](https://www.instagram.com/eteportodigital/). O projeto tem como foco ensinar desenvolvedores em formação a criar, versionar e publicar seus próprios portfólios com ferramentas reais do mercado.

---

## 🎯 Objetivos da oficina

- [x] Apresentar o Git e GitHub de forma prática
- [x] Ensinar os comandos essenciais de versionamento
- [x] Desenvolver um portfólio em HTML, CSS e JavaScript
- [x] Publicar o projeto online via GitHub Pages
- [x] Incentivar a criação de projetos autorais

---

## 🛠️ Tecnologias utilizadas

| Tecnologia | Versão | Uso |
|---|---|---|
| ![HTML5](https://img.shields.io/badge/HTML5-0A0A0A?style=flat-square&logo=html5&logoColor=818CF8) | 5 | Estrutura das páginas |
| ![CSS3](https://img.shields.io/badge/CSS3-0A0A0A?style=flat-square&logo=css3&logoColor=818CF8) | 3 | Estilização e responsividade |
| ![JavaScript](https://img.shields.io/badge/JavaScript-0A0A0A?style=flat-square&logo=javascript&logoColor=F472B6) | ES6+ | Interatividade e filtros |
| ![Git](https://img.shields.io/badge/Git-0A0A0A?style=flat-square&logo=git&logoColor=F472B6) | — | Versionamento |
| ![GitHub](https://img.shields.io/badge/GitHub-0A0A0A?style=flat-square&logo=github&logoColor=818CF8) | — | Hospedagem e deploy |

---

## 📂 Estrutura do projeto

```
portfolio-dev-etepd/
│
├── assets/
│   ├── css/
│   ├── docs/
│   │   └── banner-dev.svg        ← banner do README
│   ├── images/
│   │   └── foto.jpg
│   └── js/
│
├── data/
│   └── projects.json
│
├── index.html
├── about.html
├── projects.html
├── skills.html
├── contact.html
├── favicon.ico
└── README.md
```

---

## ⚙️ Funcionalidades

- **Hero Section** — apresentação com status de disponibilidade
- **Projetos dinâmicos** — listagem carregada via `projects.json`
- **Filtro e busca** — filtra projetos por tecnologia em tempo real
- **Skills** — barras de progresso animadas e certificações
- **Contato** — formulário com validação e links sociais
- **Download de currículo** — disponível direto na página
- **Tema dark/light** — alternância com preferência salva no navegador

---

## 🚀 Como rodar o projeto

### 1. Clone o repositório

```bash
git clone https://github.com/WallaceMichael/portfolio-dev-etepd.git
cd portfolio-dev-etepd
```

### 2. Abra no VS Code

```bash
code .
```

### 3. Rode com Live Server

Clique em **Go Live** na barra inferior do VS Code e acesse `http://127.0.0.1:5500`.

> 💡 Sem o Live Server? Instale pela aba de **Extensões** (`Ctrl+Shift+X`).

---

## 📧 Configuração do formulário (EmailJS)

O formulário de contato utiliza o [EmailJS](https://www.emailjs.com) para enviar mensagens sem precisar de back-end.

### Passo 1 — Criar conta

Acesse [emailjs.com](https://www.emailjs.com), clique em **Sign Up** e crie sua conta.

### Passo 2 — Criar um serviço de e-mail

1. Vá em **Email Services** → **Add New Service**
2. Escolha seu provedor (ex: Gmail) e conecte sua conta
3. Copie o **Service ID** gerado

### Passo 3 — Criar um template de e-mail

1. Vá em **Email Templates** → **Create New Template**
2. Monte seu template usando as variáveis abaixo:

| Variável | Descrição |
|---|---|
| `{{nome}}` | Nome do remetente |
| `{{email}}` | E-mail do remetente |
| `{{assunto}}` | Assunto da mensagem |
| `{{mensagem}}` | Corpo da mensagem |
| `{{time}}` | Data/hora do envio |

3. Salve e copie o **Template ID**

### Passo 4 — Obter a Public Key

1. Acesse **Account → API Keys**
2. Copie sua **Public Key**

### Passo 5 — Configurar no projeto

No arquivo `assets/js/script.js`, localize a seção do formulário e substitua os valores indicados pelos comentários:

```js
emailjs.init("SUA_PUBLIC_KEY");

emailjs.send("SEU_SERVICE_ID", "SEU_TEMPLATE_ID", templateParams);
```

---

## 🔗 Acesse o projeto

<p>
  <a href="https://github.com/WallaceMichael/portfolio-dev-etepd">
    <img src="https://img.shields.io/badge/Ver%20repositório-0A0A0A?style=for-the-badge&logo=github&logoColor=818CF8" alt="GitHub"/>
  </a>
  &nbsp;
  <a href="https://wallacemichael.github.io/portfolio-dev-etepd/">
    <img src="https://img.shields.io/badge/Ver%20deploy-0A0A0A?style=for-the-badge&logo=githubpages&logoColor=4ade80" alt="Deploy"/>
  </a>
</p>

---

## 👨‍💻 Autor

<table>
  <tr>
    <td align="center">
      <img src="https://github.com/WallaceMichael.png" width="80px" style="border-radius:50%"/><br/>
      <strong>Wallace Michael</strong><br/>
      <sub>Desenvolvedor em formação 🚀</sub><br/><br/>
      <a href="https://github.com/WallaceMichael">
        <img src="https://img.shields.io/badge/GitHub-0A0A0A?style=flat-square&logo=github&logoColor=818CF8"/>
      </a>
      &nbsp;
      <a href="https://linkedin.com/in/wallacemichael">
        <img src="https://img.shields.io/badge/LinkedIn-0A0A0A?style=flat-square&logo=linkedin&logoColor=818CF8"/>
      </a>
    </td>
  </tr>
</table>

---

<p align="center">
  Feito com ❤️ durante a oficina de <strong>Git &amp; GitHub</strong> · ETE Porto Digital
</p>