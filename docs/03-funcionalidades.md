# ⚙️ Funcionalidades — Gestor de Orçamentos

Documento que descreve todas as funcionalidades do sistema, organizadas por versão.

---

## 🎯 Visão Geral das Versões

| Versão | Foco | Prazo estimado |
|--------|------|----------------|
| *v1.0 — MVP* | Cadastro + Orçamento básico | Mês 1 |
| *v1.1* | Envio + Aprovação | Mês 2 |
| *v1.2* | Relatórios + Gamificação | Mês 3 |
| *v2.0* | Mobile + Integrações | Mês 4–5 |
| *v3.0* | Escala + Monetização | Mês 6+ |

---

## 🚀 v1.0 — MVP (Mês 1)

### 👤 Autenticação
- [ ] Cadastro com e-mail e senha
- [ ] Login
- [ ] Recuperação de senha
- [ ] Logout

### 👥 Clientes
- [ ] Cadastrar cliente (nome, e-mail, telefone, endereço)
- [ ] Listar clientes
- [ ] Editar cliente
- [ ] Excluir cliente
- [ ] Buscar cliente por nome

### 🛠️ Serviços
- [ ] Cadastrar serviço (nome, descrição, valor)
- [ ] Listar serviços
- [ ] Editar serviço
- [ ] Excluir serviço

### 📝 Orçamentos
- [ ] Criar orçamento (selecionar cliente + serviços)
- [ ] Cálculo automático do total
- [ ] Gerar PDF com identidade visual
- [ ] Listar orçamentos
- [ ] Editar orçamento
- [ ] Excluir orçamento
- [ ] Duplicar orçamento

---

## 📤 v1.1 — Envio e Aprovação (Mês 2)

### 🔗 Compartilhamento
- [ ] Link público único por orçamento
- [ ] Envio por *WhatsApp* (link direto)
- [ ] Envio por *e-mail* com PDF anexo

### 🎯 Status do Orçamento
- [ ] Rascunho
- [ ] Enviado
- [ ] Aprovado
- [ ] Recusado
- [ ] Pago

### 🔔 Notificações
- [ ] Notificação ao freelancer quando cliente responder
- [ ] Lembrete automático após 3 dias sem resposta
- [ ] E-mail de boas-vindas para o cliente

### 📅 Controle
- [ ] Definir validade do orçamento (ex: 7 dias)
- [ ] Aviso de orçamento expirado

---

## 📊 v1.2 — Relatórios e Engajamento (Mês 3)

### 📈 Dashboard
- [ ] Total faturado no mês
- [ ] Total aprovado
- [ ] Total pendente
- [ ] Taxa de conversão

### 📄 Relatórios
- [ ] Relatório mensal detalhado
- [ ] Gráfico de faturamento por semana
- [ ] Gráfico de orçamentos por status
- [ ] Exportar relatório em PDF

### 🎮 Gamificação
- [ ] Metas mensais (definir objetivo de faturamento)
- [ ] Badges/conquistas:
  - 🥇 Primeiro orçamento
  - 💯 10 clientes cadastrados
  - 🚀 50 orçamentos enviados
  - 💰 R$ 10.000 faturados

---

## 📱 v2.0 — Mobile e Integrações (Mês 4–5)

### 📲 Mobile
- [ ] *PWA* (instalável no celular sem loja)
- [ ] Design responsivo mobile-first
- [ ] Modo *offline* (funciona sem internet)
- [ ] Sincronização automática quando voltar online

### 💳 Pagamentos
- [ ] Integração com *Mercado Pago*
- [ ] Cobrança via *Pix* com QR Code
- [ ] Assinatura digital do cliente

### 🎨 Personalização
- [ ] Templates de orçamento personalizáveis
- [ ] Upload de *logo* do freelancer
- [ ] Cores personalizáveis

### 🔗 Integrações
- [ ] *Google Agenda* (adicionar prazo do orçamento)
- [ ] *Google Drive* (backup de PDFs)
- [ ] *Zapier / Make* (automações)

---

## 🚀 v3.0 — Escala e Monetização (Mês 6+)

### 💰 Planos
- [ ] Plano *Free* (3 orçamentos/mês)
- [ ] Plano *Pro* (R$ 29/mês — ilimitado)
- [ ] Plano *Business* (R$ 79/mês — multiusuário)
- [ ] Pagamento via Stripe, Mercado Pago ou Pix

### 👥 Multiusuário
- [ ] Convidar membros da equipe
- [ ] Permissões diferentes (admin, editor, visualizador)
- [ ] Atividades e histórico compartilhado

### 🔌 API
- [ ] API pública documentada
- [ ] Webhooks para integrações externas
- [ ] SDKs (Python, JavaScript)

### 🎁 Programa de Indicação
- [ ] Link de indicação único
- [ ] Créditos por indicação bem-sucedida
- [ ] Ranking de indicadores

---

## 🚫 Fora de Escopo (decisão estratégica)

Para manter o foco do produto, *não entra* (nem no plano de longo prazo):

- ❌ *Emissão de nota fiscal* (integração futura com parceiros)
- ❌ *Controle financeiro completo* (é outra categoria de produto)
- ❌ *CRM avançado* (foco é orçamento, não funil de vendas)
- ❌ *Assinatura eletrônica com validade jurídica* (usaremos versão simples)
- ❌ *Chat interno* (WhatsApp já resolve)

---

## 📌 Status Atual

- *Versão em desenvolvimento:* v1.0 (MVP)
- *Progresso:* 🟡 Planejamento
- *Última atualização:* Outubro 2026