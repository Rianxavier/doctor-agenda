# DoctorAgenda - Plataforma de Agendamentos para Clínicas 🏥

Bem-vindo ao **DoctorAgenda**, uma plataforma SaaS desenvolvida durante o Bootcamp da Full Stack Club. Com ela, clínicas podem gerenciar médicos, pacientes e agendamentos de forma eficiente, além de acompanhar métricas por meio de um dashboard moderno.

---

## ✨ Funcionalidades

- **Autenticação Segura**
  - Criação de conta
  - Login com email e senha
  - Login com Google (OAuth)

- **Gestão de Clínica**
  - Criação de clínicas
  - Aquisição de planos pagos via Stripe

- **Gerenciamento de Pacientes**
  - Cadastro e listagem de pacientes

- **Gerenciamento de Médicos**
  - Cadastro e listagem de médicos

- **Agendamentos**
  - Criação, visualização e gerenciamento de agendamentos

- **Dashboard Interativo**
  - Acompanhamento de métricas com dados em tempo real

---

## 🚀 Tecnologias Utilizadas

- **Next.js:** Framework React Full Stack
- **React:** Construção de interfaces reativas
- **TypeScript:** Tipagem estática para maior confiabilidade
- **TailwindCSS:** Estilização rápida e moderna
- **Shadcn/UI:** Componentes acessíveis e reutilizáveis
- **Drizzle ORM:** Abstração do banco de dados PostgreSQL
- **PostgreSQL:** Banco de dados relacional robusto
- **NeonDB:** Hospedagem moderna para PostgreSQL
- **Better-auth:** Autenticação customizada para Next.js
- **Google Cloud Platform:** OAuth com Google
- **Stripe:** Processamento de pagamentos e assinaturas
- **React Hook Form:** Manipulação de formulários
- **Zod:** Validação de dados
- **Prettier + ESLint:** Padronização e qualidade de código

---

## ⚙️ Instalação

### Pré-requisitos

- Node.js >= 16.0
- Conta no [NeonDB](https://neon.tech)
- Conta no [Google Cloud Console](https://console.cloud.google.com)
- Conta no [Stripe](https://stripe.com)
  
### Passo a passo

1. Clone o repositório:

```bash
git clone https://github.com/seu-usuario/clinic-saas.git
cd clinic-saas
```

2. Instale as dependências:

```bash
npm install
```

3. Configure as variáveis de ambiente com base no exemplo abaixo:

```env
# Banco de Dados
DATABASE_URL="sua_url_do_banco_postgresql"

# Better Auth
BETTER_AUTH_SECRET="sua_chave_secreta_do_auth"
BETTER_AUTH_URL="http://localhost:3000/api/auth"

# Google OAuth
GOOGLE_CLIENT_ID="sua_google_client_id"
GOOGLE_CLIENT_SECRET="sua_google_client_secret"

# Stripe
NEXT_PUBLIC_STRIPE_PUBLISHABLE_KEY="sua_chave_publica_stripe"
STRIPE_SECRET_KEY="sua_chave_secreta_stripe"
STRIPE_ESSENTIAL_PLAN_PRICE_ID="id_do_plano_essencial"
STRIPE_WEBHOOK_SECRET="webhook_secret_stripe"

# URLs da aplicação
NEXT_PUBLIC_APP_URL="http://localhost:3000"
NEXT_PUBLIC_STRIPE_CUSTOMER_PORTAL_URL="url_do_portal_do_cliente_stripe"
```

4. Rode as migrações do banco de dados:

```bash
npx drizzle-kit push
```

5. Inicie o servidor de desenvolvimento:

```bash
npm run dev
```

### **Acesse o aplicativo** 🌐

Abra seu navegador e acesse [http://localhost:3000](http://localhost:3000).

### **Observações** 📌 

Este projeto foi desenvolvido com fins educacionais no Bootcamp da Full Stack Club. Você pode expandi-lo adicionando testes, envio de emails, filtros de agendamentos, relatórios, permissões por função, entre outros.
