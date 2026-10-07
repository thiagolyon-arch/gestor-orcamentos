# 🎭 Caso de Uso — Gestor de Orçamentos

Documento que descreve as principais interações entre os usuários e o sistema.

---

## 👥 Atores

| Ator | Descrição |
|------|-----------|
| *Freelancer* | Usuário principal. Cria orçamentos, gerencia clientes e serviços. |
| *Cliente* | Recebe o orçamento por link, aprova ou recusa. |
| *Sistema* | Gera PDFs, envia e-mails e controla status. |

---

## 🎯 Casos de Uso Principais

### UC-01 — Cadastrar Cliente

*Ator principal:* Freelancer  
*Pré-condição:* Estar logado  
*Fluxo principal:*
1. Freelancer acessa "Clientes" → "Novo Cliente"
2. Preenche nome, e-mail e telefone
3. Clica em "Salvar"
4. Sistema valida os dados e grava no banco
5. Sistema exibe mensagem de sucesso

*Fluxo alternativo:*  
- Se o e-mail já existir, sistema avisa e pede para usar outro

---

### UC-02 — Cadastrar Serviço

*Ator principal:* Freelancer  
*Pré-condição:* Estar logado  
*Fluxo principal:*
1. Freelancer acessa "Serviços" → "Novo Serviço"
2. Informa nome, descrição e valor
3. Clica em "Salvar"
4. Sistema valida e grava
5. Serviço fica disponível para uso em orçamentos

---

### UC-03 — Criar Orçamento

*Ator principal:* Freelancer  
*Pré-condição:* Ter pelo menos 1 cliente e 1 serviço cadastrados  
*Fluxo principal:*
1. Freelancer clica em "Novo Orçamento"
2. Seleciona um cliente
3. Adiciona um ou mais serviços
4. Sistema calcula o valor total automaticamente
5. Freelancer revisa e clica em "Gerar Orçamento"
6. Sistema salva e gera um PDF com a marca do freelancer
7. Sistema gera um link público único

*Fluxo alternativo:*  
- Se não houver serviços, sistema sugere cadastrar antes

---

### UC-04 — Enviar Orçamento ao Cliente

*Ator principal:* Freelancer  
*Pré-condição:* Ter um orçamento criado  
*Fluxo principal:*
1. Freelancer abre o orçamento
2. Clica em "Enviar"
3. Escolhe o canal: Link / WhatsApp / E-mail
4. Sistema envia e marca o status como *Enviado*

---

### UC-05 — Aprovar ou Recusar Orçamento

*Ator principal:* Cliente  
*Pré-condição:* Ter recebido o link do orçamento  
*Fluxo principal:*
1. Cliente acessa o link público
2. Visualiza o PDF ou a página do orçamento
3. Clica em "Aprovar" ou "Recusar"
4. Sistema registra a decisão
5. Freelancer recebe notificação

---

### UC-06 — Marcar Orçamento como Pago

*Ator principal:* Freelancer  
*Pré-condição:* Orçamento estar com status *Aprovado*  
*Fluxo principal:*
1. Freelancer abre o orçamento aprovado
2. Clica em "Marcar como Pago"
3. Sistema muda o status para *Pago*
4. Valor entra no relatório mensal

---

### UC-07 — Visualizar Relatório Mensal

*Ator principal:* Freelancer  
*Pré-condição:* Ter pelo menos 1 orçamento no mês  
*Fluxo principal:*
1. Freelancer acessa "Relatórios"
2. Escolhe o mês desejado
3. Sistema exibe:
   - Total de propostas enviadas
   - Total aprovado
   - Total pago
   - Taxa de conversão
4. Freelancer pode exportar em PDF

---

## 🔄 Fluxo Resumido do Sistema
|                      |                      |
|-- cadastra cliente ->|                      |
|-- cadastra serviço ->|                      |
|-- cria orçamento --->|                      |
|                      |-- gera PDF + link -->|
|                      |                      |
|                      |<-- aprova/recusa ----|
|<-- notificação ------|                      |
|-- marca como pago -->|                      |
|                      |                      |
## 📌 Status possíveis de um Orçamento

| Status | Significado |
|--------|-------------|
| 🟡 *Rascunho* | Em construção, ainda não enviado |
| 🔵 *Enviado* | Aguardando resposta do cliente |
| 🟢 *Aprovado* | Cliente aceitou |
| 🔴 *Recusado* | Cliente não aceitou |
| ✅ *Pago* | Valor recebido |