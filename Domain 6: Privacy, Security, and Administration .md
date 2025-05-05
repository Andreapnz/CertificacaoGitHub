# 🔐 Domain 6: Privacy, Security, and Administration

## 👁️ Níveis de Visibilidade do Repositório

- **Público:** Qualquer pessoa pode acessar e clonar.
- **Privado:** Apenas colaboradores convidados têm acesso.
- **Interno (Enterprise):** Acesso restrito a membros da organização (somente disponível em GitHub Enterprise).

> 🔐 A escolha correta da visibilidade ajuda a proteger dados e a restringir acesso indevido.

## 👥 Gerenciamento de Permissões

| Permissão   | Acesso                                                                |
|-------------|-----------------------------------------------------------------------|
| **Read**    | Visualizar código, issues e pull requests.                           |
| **Triage**  | Gerenciar issues e PRs sem editar o código.                          |
| **Write**   | Push, criar branches, editar código.                                 |
| **Maintain**| Gerenciar releases, tags, configurações limitadas do repositório.    |
| **Admin**   | Controle total do repositório, inclusive permissões e settings.      |

> ✅ **Dica:** Sempre conceda **o menor nível de permissão necessário**.


## 🔑 Gerenciamento de Secrets

- Armazene dados sensíveis no menu: `Settings > Secrets` ou `Actions > Secrets and variables`.
- Protege **tokens**, **chaves de API** e **credenciais** usadas em GitHub Actions.

### Exemplo em GitHub Actions:
yaml
env:
  DB_PASSWORD: ${{ secrets.DB_PASSWORD }}

##  🧪 Segurança e Automação
### 🔎 Code Scanning
- Analisa o código-fonte para detectar vulnerabilidades.
- Pode ser integrado com CodeQL, SonarQube e outras ferramentas.

### 🧬 Secret Scanning
- Detecta automaticamente chaves, tokens e credenciais acidentalmente expostas em:
  - Commits
  - Pull Requests
  - Issues

### 🛡️ Dependabot
- Monitora e atualiza automaticamente dependências inseguras.
- Abre Pull Requests com versões corrigidas quando necessário.
- Baseado em bancos de dados de vulnerabilidades conhecidos (CVE).

## 📝 Auditoria e Logs (GitHub Organizations e Enterprise)
- Disponível em níveis corporativos para rastrear:
  - Acessos de usuários
  - Alterações em configurações
  - Eventos de segurança
- Permite monitoramento detalhado de atividades suspeitas ou não autorizadas.
- Logs exportáveis para ferramentas SIEM e de conformidade.

## 🔐 Autenticação e Acesso Seguro
- 2FA (Autenticação em Dois Fatores): Reforça a segurança da conta.
- SSH Keys: Método seguro para autenticação de push/pull via terminal.
- Tokens de Acesso Pessoal (PAT): Alternativa segura a senhas.
- SSO (Single Sign-On): Disponível para integração com diretórios corporativos (SAML/Okta).

🚨 O uso de senhas simples ou armazenamento de credenciais no código é fortemente desencorajado.

## ✅ Boas Práticas de Segurança
- Ativar 2FA para todos os membros do repositório.
- Usar tokens e secrets no lugar de dados sensíveis no código.
- Manter repositórios privados, sempre que houver dados internos ou estratégicos.
- Ativar e monitorar Dependabot, Code Scanning e Secret Scanning.
- Atualizar dependências regularmente.
- Revisar periodicamente os níveis de permissão dos colaboradores.
- Adotar templates de segurança e arquivos como SECURITY.md.

📚 Dica bônus: Combine GitHub Actions com Secrets para criar pipelines seguras e automatizadas — reduzindo riscos e melhorando a confiabilidade do deploy.


