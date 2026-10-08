# 🗺️ Roadmap — Gestor de Orçamentos

Documento que mostra o caminho planejado para o desenvolvimento do projeto, organizado em fases.

---

## 🎯 Visão Geral

O projeto está dividido em *5 fases*, começando pelo MVP (versão mínima viável) até se tornar uma ferramenta completa com múltiplas integrações.

| Fase | Período | Foco |
|------|---------|------|
| *Fase 1* | Mês 1 | MVP — Cadastro + Orçamento básico |
| *Fase 2* | Mês 2 | Envio + Aprovação + Pagamento |
| *Fase 3* | Mês 3 | Relatórios + Gamificação |
| *Fase 4* | Mês 4–5 | Integrações + Mobile |
| *Fase 5* | Mês 6+ | Escala + Monetização |

---

## 🚀 FASE 1 — MVP (Mês 1)

*Objetivo:* Ter um sistema funcional onde o freelancer consiga cadastrar clientes, serviços e criar um orçamento em PDF.

### ✅ Entregas

- [ ] Tela de *Login / Cadastro* com autenticação
- [ ] Cadastro de *Clientes* (nome, e-mail, telefone)
- [ ] Cadastro de *Serviços* (nome, descrição, valor)
- [ ] Criação de *Orçamento* com múltiplos serviços
- [ ] Cálculo automático de total
- [ ] *Exportação em PDF* com identidade do freelancer
- [ ] Persistência em *banco de dados* (SQLite para começar)

### 🛠️ Stack

- Backend: *Python + FastAPI*
- Banco: *SQLite*
- Frontend: *HTML + HTMX*
- PDF: *ReportLab*

### 📊 Métricas de Sucesso

- 10 freelancers de teste conseguem criar 1 orçamento
- Tempo médio de criação: *< 5 minutos*

---

## 📤 FASE 2 — Envio e Aprovação (Mês 2)

*Objetivo:* Permitir que o orçamento chegue até o cliente e que ele possa aprovar ou recusar.

### ✅ Entregas

- [ ] *Link público único* por orçamento
- [ ] Envio por *WhatsApp* (link direto)
- [ ] Envio por *e-mail* com PDF anexo
- [ ] *Status do orçamento* (Rascunho → Enviado → Aprovado/Recusado → Pago)
- [ ] *Notificação* ao freelancer quando cliente responder
- [ ] Controle de *validade* do orçamento (ex: 7 dias)

### 📊 Métricas de Sucesso

- Taxa de aprovação: *> 40%*
- Tempo médio de resposta do cliente: *< 48h*

---

## 📊 FASE 3 — Relatórios e Engajamento (Mês 3)

*Objetivo:* Mostrar o valor do sistema para o freelancer através de dados e gamificação.

### ✅ Entregas

- [ ] *Dashboard* com totais do mês
- [ ] *Relatório mensal* com gráficos
- [ ] Taxa de conversão de propostas
- [ ] *Exportação de relatório em PDF*
- [ ] Sistema de *metas mensais* (gamificação)
- [ ] *Badges/Conquistas* (primeiro orçamento, 10 clientes, etc.)

### 📊 Métricas de Sucesso

- Freelancer acessa o relatório *pelo menos 1x por semana*
- Taxa de retenção: *> 60%*

---

## 📱 FASE 4 — Integrações e Mobile (Mês 4–5)

*Objetivo:* Levar o sistema para o celular e integrar com ferramentas que o freelancer já usa.

### ✅ Entregas

- [ ] *PWA* (app instalável no celular sem loja)
- [ ] Integração com *Mercado Pago / Pix*
- [ ] Assinatura digital do cliente
- [ ] Templates *personalizáveis* de orçamento
- [ ] Modo *offline* (funciona sem internet)
- [ ] Integração com *Google Agenda*

### 📊 Métricas de Sucesso

- *> 50%* dos acessos via mobile
- Tempo de criação de orçamento: *< 2 minutos*

---

## 🚀 FASE 5 — Escala e Monetização (Mês 6+)

*Objetivo:* Transformar o projeto em um *produto comercial* com planos pagos.

### ✅ Entregas

- [ ] Sistema de *assinaturas* (Free / Pro / Business)
- [ ] *Multiusuário* (equipes)
- [ ] *API pública* para integração
- [ ] Programa de *indicação* (indique e ganhe)
- [ ] Painel *administrativo*
- [ ] *Blog/SEO* para aquisição orgânica

### 💰 Metas de Negócio

- *1.000 usuários* cadastrados
- *100 assinantes* pagos
- Receita mensal: *R$ 5.000*

---

## 📅 Cronograma Visual