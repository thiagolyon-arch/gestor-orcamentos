# 🗺️ Diagrama de Caso de Uso — Gestor de Orçamentos

Representação visual dos casos de uso do sistema, mostrando os atores, as ações disponíveis e as dependências entre elas.

---

## 📊 Diagrama Completo

mermaid
graph TD
    %% ===== ATORES =====
    F["👨‍💼 Freelancer"]
    C["👤 Cliente"]

    %% ===== FRONTEIRA DO SISTEMA =====
    subgraph SISTEMA["🏢 Gestor de Orçamentos"]
        direction TB

        UC0(("🔐 Cadastrar / Login"))
        UC1(("👥 Cadastrar Cliente"))
        UC2(("🛠️ Cadastrar Serviço"))
        UC3(("📝 Criar Orçamento"))
        UC4(("📤 Enviar Orçamento"))
        UC5(("✅ Aprovar / Recusar"))
        UC6(("💰 Marcar como Pago"))
        UC7(("📊 Ver Relatório"))
    end

    %% ===== RELAÇÕES ATOR → CASO =====
    F --> UC0
    C --> UC5

    %% ===== DEPENDÊNCIAS ENTRE CASOS =====
    UC0 --> UC1
    UC0 --> UC2
    UC0 --> UC3
    UC0 --> UC7

    UC1 --> UC3
    UC2 --> UC3
    UC3 --> UC4
    UC4 --> UC5
    UC5 --> UC6
    UC6 --> UC7

    %% ===== ESTILOS =====
    classDef ator fill:#FFE082,stroke:#F57C00,stroke-width:2px,color:#000
    classDef caso fill:#E3F2FD,stroke:#1976D2,stroke-width:2px,color:#000
    classDef sistema fill:#F5F5F5,stroke:#9E9E9E,stroke-width:2px,stroke-dasharray:5 5

    class F,C ator
    class UC0,UC1,UC2,UC3,UC4,UC5,UC6,UC7 caso
    class SISTEMA sistema


---

## 🧠 Como ler este diagrama

### 🟡 Atores (amarelo)
- *Freelancer* — usuário principal, inicia a maioria das ações
- *Cliente* — ator secundário, apenas aprova ou recusa

### 🔵 Casos de Uso (azul)
Cada elipse representa uma *ação* que o sistema oferece:

| Código | Caso de Uso | Descrição |
|--------|-------------|-----------|
| UC0 | 🔐 Cadastrar / Login | Ponto de entrada obrigatório |
| UC1 | 👥 Cadastrar Cliente | Freelancer cadastra seus clientes |
| UC2 | 🛠️ Cadastrar Serviço | Cadastra serviços com valores |
| UC3 | 📝 Criar Orçamento | Monta um orçamento com cliente + serviços |
| UC4 | 📤 Enviar Orçamento | Envia via link, WhatsApp ou e-mail |
| UC5 | ✅ Aprovar / Recusar | Cliente decide sobre a proposta |
| UC6 | 💰 Marcar como Pago | Freelancer registra o recebimento |
| UC7 | 📊 Ver Relatório | Visualiza totais do mês |

### ⬜ Fronteira do Sistema (cinza tracejada)
Delimita o que *pertence ao sistema*. O que está fora (Freelancer e Cliente) são os atores externos.

### ➡️ Fluxo principal


Freelancer ──► Login ──► Cadastra Cliente/Serviço ──► Cria Orçamento
                                                              │
                                                              ▼
                                                        Envia ao Cliente
                                                              │
                                                              ▼
                                            Cliente ──► Aprova / Recusa
                                                              │
                                                              ▼
                                                    Marca como Pago
                                                              │
                                                              ▼
                                                      Vê Relatório


---

## 📝 Regras de Negócio Destacadas

1. *Login obrigatório* — todas as ações do Freelancer exigem autenticação
2. *Ordem de dependência* — para criar um orçamento, é preciso ter pelo menos 1 cliente e 1 serviço
3. *Envio antes da aprovação* — o cliente só pode aprovar/recusar após receber o orçamento
4. *Pagamento só após aprovação* — só se marca como pago o que foi aprovado
5. *Relatório consolida tudo* — só aparece com dados já registrados