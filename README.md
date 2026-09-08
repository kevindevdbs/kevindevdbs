<h1 align="center">Olá 👋, eu sou o Kevin Dias</h1>

<p align="center">
  <b>Desenvolvedor Fullstack · Foco em Backend .NET</b><br>
  🇧🇷 Belo Horizonte — MG
</p>

<p align="center">
  <a href="https://kevin-portfolio-phi-ten.vercel.app" target="_blank">
    <img src="https://img.shields.io/badge/Portf%C3%B3lio-Acessar-ff9f1c?style=for-the-badge&logo=vercel&logoColor=white" />
  </a>
  <a href="https://www.linkedin.com/in/kevin-dias-765729372/" target="_blank">
    <img src="https://img.shields.io/badge/LinkedIn-Kevin%20Dias-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" />
  </a>
  <a href="mailto:kevindevdbs@gmail.com">
    <img src="https://img.shields.io/badge/Email-kevindevdbs-EA4335?style=for-the-badge&logo=gmail&logoColor=white" />
  </a>
</p>

---

## 👨‍💻 Sobre mim

Construo **APIs REST em C# e .NET**, com atenção a arquitetura, testes e código que a
próxima pessoa consiga ler sem precisar perguntar nada.

- 📚 Cursando **Análise e Desenvolvimento de Sistemas**
- 🎯 Em busca de estágio ou da primeira oportunidade como desenvolvedor
- 🧩 Gosto de entender o problema antes de sair codando
- 🎮 No tempo livre, jogos e séries

---

## 🧠 No que eu trabalho

- 🏗️ **APIs REST** em ASP.NET Core, organizadas em camadas
- 🧱 **Clean Architecture** — regra de negócio no domínio, não espalhada pelo sistema
- 🗄️ **EF Core** com SQL Server e PostgreSQL — migrations, relacionamentos, índices
- 🧪 **Testes automatizados** — unitários e de integração contra banco real em container
- 🐳 **Docker** — projeto que sobe igual em qualquer máquina
- 🌿 **Git** com branch por feature e pull request explicando a decisão tomada

---

## 🛠️ Tecnologias

### Backend

![C#](https://img.shields.io/badge/C%23-512BD4?style=for-the-badge&logo=csharp&logoColor=white)
![.NET](https://img.shields.io/badge/.NET-512BD4?style=for-the-badge&logo=dotnet&logoColor=white)
![ASP.NET Core](https://img.shields.io/badge/ASP.NET%20Core-5C2D91?style=for-the-badge&logo=dotnet&logoColor=white)
![EF Core](https://img.shields.io/badge/Entity%20Framework%20Core-512BD4?style=for-the-badge&logo=dotnet&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)

### Banco de dados

![SQL Server](https://img.shields.io/badge/SQL%20Server-CC2927?style=for-the-badge&logo=microsoftsqlserver&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![Prisma](https://img.shields.io/badge/Prisma-2D3748?style=for-the-badge&logo=prisma&logoColor=white)

### Frontend

![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-FFD43B?style=for-the-badge&logo=javascript&logoColor=000)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)
![Tailwind](https://img.shields.io/badge/TailwindCSS-38BDF8?style=for-the-badge&logo=tailwindcss&logoColor=white)

### Testes & Ferramentas

![xUnit](https://img.shields.io/badge/xUnit-5C2D91?style=for-the-badge&logo=dotnet&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![Swagger](https://img.shields.io/badge/Swagger-85EA2D?style=for-the-badge&logo=swagger&logoColor=000)
![VS Code](https://img.shields.io/badge/VS%20Code-007ACC?style=for-the-badge&logo=visualstudiocode&logoColor=white)

---

## 📌 Projeto em destaque

### [Subscription Manager](https://github.com/kevindevdbs/subscription-manager)

API REST de assinaturas recorrentes: clientes contratam planos, o sistema emite as
faturas mensais e controla o ciclo de vida de contratos e faturas até o pagamento, o
vencimento ou o cancelamento.

`.NET 10` · `ASP.NET Core` · `EF Core` · `SQL Server` · `Docker` · `xUnit` · `Testcontainers`

**O que ele mostra:**

- **Entidades ricas, não sacos de propriedade** — todo setter é privado e o estado só
  muda por método que valida a transição. Não existe caminho para uma fatura paga ser
  paga de novo.
- **Erro de negócio vira HTTP em um lugar só** — as exceções carregam o próprio status
  e um filtro as converte na resposta. Nenhum controller tem `try/catch`.
- **Regra crítica em duas camadas** — um cliente não assina o mesmo plano duas vezes:
  a consulta no handler devolve 409 legível, e um índice único filtrado garante a
  regra quando duas requisições passam ao mesmo tempo.
- **Teste contra banco de verdade** — a integração sobe um SQL Server descartável em
  container. Índice único, tipo de coluna e transação são exercitados de verdade, não
  simulados em memória. São 251 testes no total.

Sobe inteiro com um comando:

```bash
docker compose up -d --build
```

> O raciocínio de cada mudança está nas descrições dos pull requests — o que foi
> entregue, o que foi descartado no caminho e por quê.

---

<img src="https://raw.githubusercontent.com/kevindevdbs/kevindevdbs/output/snake.svg" alt="Snake animation" />

---

<p align="center">
  <i>"Código bom é o que a próxima pessoa entende sem precisar perguntar —<br>
  inclusive eu mesmo daqui a seis meses."</i>
</p>

<p align="center">
  ⭐ Aberto a estágio, primeira oportunidade e projetos colaborativos
</p>
