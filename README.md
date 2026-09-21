<div align="center">

# ⚡ Task CRM

**CRM inteligente com IA nativa, WhatsApp integrado e multi-tenant.**

**Agentes de IA que atendem, qualificam e vendem por você — dentro de uma plataforma completa, self-hosted e white-label.**

[![Stack](https://img.shields.io/badge/Stack-Next.js%2016%20·%20TypeScript%20·%20Supabase-blue)](/)
[![Status](https://img.shields.io/badge/deploy-Live%20on%20Render-brightgreen)](https://task-crm-v2.onrender.com)
[![License](https://img.shields.io/badge/license-Proprietary-red)](LICENSE)

[**🚀 Demo**](https://task-crm-v2.onrender.com) · [**📋 Changelog**](#-roadmap) · [**🛠️ Instalação**](#-instalação) · [**⚙️ Configuração**](#-configuração)

</div>

---

## 🧠 O que é

O Task CRM é uma plataforma completa de vendas e atendimento que reúne em um único lugar:

| Módulo | O que faz |
|---|---|
| 📥 **Inbox** | Recebe, organiza e responde mensagens de WhatsApp, Instagram e Meta |
| 🎯 **Funil** | Pipeline visual de vendas com cards, tags coloridas e tracking de contatos |
| 📅 **Agenda** | Marcação inteligente com Google Calendar e disponibilidade compartilhada |
| 🤖 **Agentes IA** | Atendente virtual com RAG, guardrails e handoff automático para humanos |
| 📊 **Análise** | Dashboard com métricas de vendas, conversões e performance de IA |
| 🎙️ **Voz** | Ligações VoIP integradas com IA conversacional |
| 💰 **Financeiro** | Comandas, faturamento recorrente, comissões e relatórios |
| 🗺️ **Radar** | Prospecção inteligente — descobre empresas, filtra e entra em contato |
| 🧩 **Extensões** | Adicione funcionalidades por organização sem reiniciar |

---

## 🎨 Identidade visual

| Item | Valor |
|---|---|
| **Nome** | Task CRM |
| **Cor principal** | `#1447e6` |
| **Fundos** | Tema escuro + claro |
| **Tipografia** | System UI / Inter |

---

## 🚀 Instalação

### Pré-requisitos

- **Node.js 22+**
- **pnpm 9.15.9+**
- **Supabase** (Postgres + Auth + Realtime + Storage)
- **Vercel** (opcional — para IA)

### Passos

```bash
# 1. Clonar
git clone https://github.com/CozmosAI/Task-crm-v2.git
cd Task-crm-v2

# 2. Instalar
pnpm install

# 3. Configurar envs
cp .env.example .env
# Edite .env com suas chaves

# 4. Rodar dev server
pnpm dev

# 5. Abrir http://localhost:3000
```

---

## ⚙️ Configuração

### Variáveis de ambiente

| Variável | Descrição | Onde obter |
|---|---|---|
| `OPENROUTER_API_KEY` | IA principal (chat + embeddings) | [openrouter.ai](https://openrouter.ai) |
| `GEMINI_API_KEY` | Catálogo de modelos Gemini | [aistudio.google.com](https://aistudio.google.com) |
| `ANTHROPIC_API_KEY` | IA alternativa (opcional) | [console.anthropic.com](https://console.anthropic.com) |
| `OPENAI_API_KEY` | Transcrição (backup) | [platform.openai.com](https://platform.openai.com) |
| `SUPABASE_URL` | URL do banco | dashboard.supabase.com → Settings |
| `SUPABASE_SERVICE_KEY` | Chave de service role | dashboard.supabase.com → Settings |
| `META_APP_ID` | Meta WhatsApp oficial | [developers.facebook.com](https://developers.facebook.com) |
| `META_APP_SECRET` | Secret do Meta App | developers.facebook.com |
| `GOOGLE_CALENDAR_CLIENT_ID` | OAuth Google Calendar | [console.cloud.google.com](https://console.cloud.google.com) |
| `GOOGLE_CALENDAR_CLIENT_SECRET` | Secret do Google | console.cloud.google.com |
| `WAHA_API_KEY` | WhatsApp alternativo (WAHA) | WAHA dashboard |
| `AZURE_SPEECH_KEY` | Transcrição de áudio | [portal.azure.com](https://portal.azure.com) |

Ver `.env.example` para a lista completa.

---

## 🧭 Roadmap

- [x] **Multi-tenant** — RLS por organização
- [x] **WhatsApp** — Canal oficial Meta + alternativo WAHA
- [x] **Agentes IA** — Chat com RAG e handoff
- [x] **Agenda** — Google Calendar sync
- [x] **Funil** — Kanban visual com drag-and-drop
- [x] **Dashboard** — Métricas em tempo real
- [x] **Financeiro** — Comandas, recorrência, faturamento
- [x] **Voz VoIP** — Chamadas com IA poragente
- [x] **Extensões** — Sistema de módulos por instalação
- [ ] **Mobile** — App nativo iOS/Android
- [ ] **Integrações** — Shopify, Nuvemshop, ERPs

---

## 🛡️ Segurança & Conformidade

- **Multi-tenant**: RLS (Row Level Security) no banco
- **Criptografia**: AES-256-GCM para credenciais sensíveis
- **Auditoria**: Trilha completa de ações na plataforma
- **LGPD**: Exportação e anonimização de dados por usuário

---

## 📄 Licença

**Proprietária — Todos os direitos reservados.**

Este software é licenciado sob os termos do distribuidor. Não é permitida
redistribuição, modificação ou uso comercial sem autorização expressa.

Para uso autorizado, entre em contato: **cozmos.atendimento@gmail.com**

---

<div align="center">

**Task CRM** — Feito com ❤️ para times de vendas que valorizam seu tempo.

</div>
