# 🚀 Domain 4: Modern Development 

## 🛠️ GitHub Codespaces

- Ambiente de desenvolvimento **baseado em nuvem**, integrado ao VS Code.
- Permite codar direto do navegador com as mesmas extensões e configurações do local.
- Ideal para:
  - Onboarding rápido em projetos
  - Colaboração remota
  - Evitar problemas de "funciona na minha máquina"

### Benefícios:
- Configurado com `.devcontainer`.
- Integração perfeita com GitHub Actions e Pull Requests.


## 🤖 GitHub Copilot

- **Assistente de codificação com IA**, desenvolvido pela GitHub + OpenAI.
- Sugere automaticamente:
  - Trechos de código
  - Funções completas
  - Testes automatizados
- Suporte para várias linguagens: JavaScript, Python, TypeScript, Go, C#, entre outras.

### Como usar:
- Disponível como extensão para VS Code e Codespaces.
- Basta começar a digitar — o Copilot sugere em tempo real.

## ⚙️ GitHub Actions (CI/CD)

- Permite **automatizar fluxos de trabalho** com arquivos `.yml` no diretório `.github/workflows/`.
- Usado para **build**, **testes**, **deploy**, **verificações de segurança** e muito mais.

### Componentes:
- **Workflow:** Processo automatizado (ex: CI, deploy).
- **Job:** Conjunto de etapas executadas em um runner.
- **Step:** Comando individual (ex: `npm install`).
- **Runner:** Ambiente onde o código é executado (Linux, Windows, macOS).

### Exemplos de uso:
- Executar testes automáticos a cada `push`.
- Deploy automático para o GitHub Pages ou cloud.
- Verificações antes de aceitar um Pull Request.

## 🧪 Integração Contínua (CI)

- Prática de rodar **testes automáticos a cada alteração** no código.
- Detecta falhas cedo no ciclo de desenvolvimento.
- Implementada com **GitHub Actions** ou outras ferramentas (ex: Travis CI, CircleCI).

## 🔐 Segurança no GitHub

### Dependabot:
- Analisa dependências e **abre PRs automáticas** para corrigir vulnerabilidades.
- Exibe alertas no repositório com detalhes do problema e da correção.

### Code Scanning:
- Verifica falhas de segurança no código-fonte (estático).
- Pode usar ferramentas como CodeQL.

### Secret Scanning:
- Detecta **vazamentos de chaves/API tokens** nos commits e PRs.


## 🧩 GitHub Marketplace

- Loja de ações e apps prontos para integrar com repositórios.
- Facilita a adição de workflows sem escrever tudo do zero.

## 🌐 GitHub Pages

- Hospedagem gratuita de sites estáticos direto do repositório.
- Pode ser usado para portfólios, documentação ou páginas de projeto.
- Integrado com Jekyll para geração automática de páginas.

## ✅ Boas Práticas em Desenvolvimento Moderno

- Configure CI/CD para validar o código automaticamente.
- Use **branches específicas** para novas features e correções.
- Mantenha o código limpo e testado com **GitHub Actions**.
- Habilite Dependabot para segurança automatizada.
- Use **Codespaces** para ambiente de desenvolvimento portátil.
- Aproveite o **Copilot** para acelerar e melhorar sua produtividade.
- Use GitHub Pages para documentar e compartilhar projetos.

📚 **Dica bônus:** Comece com templates de workflows prontos no GitHub (ex: `Node.js`, `Python`, `Docker`) e explore o potencial do Copilot para testes, documentação e automações!
