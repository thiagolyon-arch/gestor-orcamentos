# 💰 Modelo de Negócio — Gestor de Orçamentos

Documento que descreve como o produto gera valor e receita.

---

## 🎯 Resumo Executivo

O Gestor de Orçamentos é um *SaaS (Software as a Service)* com modelo de *assinatura mensal, oferecendo um plano **gratuito limitado* para atrair usuários e *planos pagos* para monetizar.

*Meta:* alcançar 1.000 assinantes em 12 meses, gerando *R$ 50.000/mês* de receita recorrente.

---

## 💵 Modelo de Monetização

### Estratégia: *Freemium + Assinatura*

- *Plano Free* → atrai usuários (aquisição)
- *Plano Pro* → converte usuários ativos
- *Plano Business* → atende equipes maiores

---

## 📊 Planos e Preços

| Plano | Preço | Limite | Público |
|-------|-------|--------|---------|
| *Free* | R$ 0 | 3 orçamentos/mês, com marca d'água | Curiosos e iniciantes |
| *Pro* | R$ 29/mês | Ilimitado, PDF sem marca d'água, WhatsApp | Freelancers ativos |
| *Business* | R$ 79/mês | Ilimitado + multiusuário + API | Equipes e pequenas empresas |

### Descontos
- *Anual:* 2 meses grátis (R$ 290/ano em vez de R$ 348)
- *Primeiros 100 clientes:* 50% off vitalício (early adopters)

---

## 💸 Estrutura de Custos (Mensal)

### Custos Fixos (MVP)

| Item | Custo estimado |
|------|----------------|
| Hospedagem (Render/Railway) | R$ 50 |
| Domínio (.com.br) | R$ 3,50 |
| E-mail transacional (Resend) | R$ 0–30 |
| *Total* | *~R$ 84/mês* |

### Custos Variáveis (por usuário)

| Item | Custo por usuário |
|------|-------------------|
| Armazenamento | R$ 0,50 |
| Envio de e-mail | R$ 0,20 |
| API WhatsApp | R$ 0,50 |
| *Total* | *~R$ 1,20/mês* |

### Custos a partir de 100 usuários

| Item | Custo |
|------|-------|
| Hospedagem maior | R$ 200 |
| Banco de dados gerenciado | R$ 100 |
| Monitoramento | R$ 50 |
| *Total* | *R$ 350/mês* |

---

## 📈 Projeção de Receita

### Cenário conservador (12 meses)

| Mês | Usuários Free | Assinantes Pro | Receita |
|-----|---------------|----------------|---------|
| Mês 1 | 50 | 5 | R$ 145 |
| Mês 3 | 300 | 25 | R$ 725 |
| Mês 6 | 1.000 | 80 | R$ 2.320 |
| Mês 12 | 5.000 | 400 | R$ 11.600 |

### Cenário otimista (12 meses)

| Mês | Usuários Free | Assinantes Pro | Receita |
|-----|---------------|----------------|---------|
| Mês 3 | 500 | 50 | R$ 1.450 |
| Mês 6 | 2.000 | 200 | R$ 5.800 |
| Mês 12 | 10.000 | 1.000 | R$ 29.000 |

---

## 📊 Métricas-Chave (KPIs)

### Aquisição
- *CAC* (Custo de Aquisição de Cliente): meta *< R$ 30*
- *Tráfego mensal* no site: 5.000 visitas/mês (mês 6)
- *Taxa de conversão* visitante → cadastro: 8%

### Conversão
- *Taxa Free → Pro: meta *> 8%**
- *Tempo até 1º orçamento: meta *< 10 minutos**

### Retenção
- *Churn mensal: meta *< 5%**
- *LTV* (Lifetime Value): meta *> R$ 300*
- *NPS* (satisfação): meta *> 50*

### Financeiro
- *MRR* (Receita Recorrente Mensal): R$ 29.000 (mês 12)
- *Razão LTV/CAC: meta *> 10x**

---

## 🎯 Canais de Aquisição

### Orgânico (baixo custo)

| Canal | Estratégia | Custo |
|-------|-----------|-------|
| *SEO* | Artigos "como fazer orçamento de X" | Tempo |
| *YouTube* | Tutoriais de precificação para freelancers | Tempo |
| *Instagram* | Conteúdo diário sobre freelancing | Tempo |
| *TikTok* | Dicas rápidas de negócio | Tempo |

### Pago (médio custo)

| Canal | Investimento | CAC esperado |
|-------|--------------|--------------|
| *Meta Ads* (Instagram/Facebook) | R$ 500/mês | R$ 25–40 |
| *Google Ads* | R$ 500/mês | R$ 30–50 |
| *Parcerias com contadores* | Comissão 20% | R$ 6 |

### Viral (crescimento exponencial)

- *Programa de indicação:* usuário ganha 1 mês grátis por amigo que assinar
- *Link de orçamento:* o cliente vê "Feito com Gestor de Orçamentos" no rodapé do PDF

---

## 🏆 Vantagens Competitivas

| Vantagem | Por quê é difícil copiar |
|----------|--------------------------|
| *Mobile-first* | Concorrentes são desktop-first |
| *Preço acessível* (R$ 29) | Concorrentes cobram R$ 79–199 |
| *Foco no freelancer BR* | Concorrentes são internacionais |
| *Suporte em português* | Diferencial real |
| *Pix e WhatsApp integrados* | Específico do Brasil |

---

## 🥊 Análise da Concorrência

| Concorrente | Preço | Pontos fortes | Pontos fracos |
|-------------|-------|---------------|---------------|
| *Bonsai* | US$ 25/mês | Internacional, robusto | Caro, em inglês |
| *Hello Bonsai* | US$ 19/mês | Bom para freelancers | Não focado no BR |
| *Conta Azul* | R$ 89/mês | Brasileiro, completo | Complexo, caro |
| *Papel + Excel* | R$ 0 | Barato | Amador, desorganizado |

*Nosso diferencial:* ser *simples, barato e brasileiro. Não competimos com ERPs — competimos com **papel e caneta*.

---

## 💡 Estratégias de Crescimento

### Fase 1 — Validação (Mês 1–3)
- 50 usuários beta gratuitos
- Feedback estruturado semanal
- Ajustes rápidos no produto

### Fase 2 — Tração (Mês 4–6)
- Lançamento oficial dos planos pagos
- Campanha de indicação
- Marketing de conteúdo (SEO + YouTube)

### Fase 3 — Escala (Mês 7–12)
- Anúncios pagos
- Parcerias com contadores
- Programa de afiliados

---

## ⚠️ Riscos e Mitigações

| Risco | Probabilidade | Mitigação |
|-------|---------------|-----------|
| *Baixa conversão Free → Pro* | Média | Testar preço, melhorar onboarding |
| *Concorrente grande copia* | Baixa | Foco em nicho (marceneiros, eletricistas) |
| *Custos de IA sobem* | Média | Limitar uso de IA no Free |
| *Churn alto* | Média | Investir em engajamento (gamificação) |
| *Problemas de LGPD* | Baixa | Contratar consultoria jurídica |

---

## 📌 Status Atual

- *Modelo:* definido ✅
- *Planos:* definidos ✅
- *Metas:* definidas ✅
- *Próximo passo:* entrevistar 5 freelancers para validar disposição de pagar