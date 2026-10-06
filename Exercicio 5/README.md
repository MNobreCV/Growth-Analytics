# <h1>EXERCÍCIO PRÁTICO 5</h1>

<h2>Tracking, Eventos, Conversões e Análise de Desempenho</h2>

Ferramenta | Formação | Participante | Ano
---------- | -------- | ------------ | ------
Google Analytics 4 — GA4| Growth & Analytics | Mauro Nobre | 2026

# PARTE I — PLANEAMENTO DO TRACKING

<h2>Tarefa 1 — Identificação dos eventos</h2>

> O objetivo é distinguir as principais ações realizadas pelo utilizador e identificar quais representam efetivamente uma conversão. O próprio exercício estabelece como exemplos page_view e search como eventos que não são necessariamente conversões.

| Ação do utilizador | Evento GA4 | É uma conversão? |
|---|---|---|
| Visualizar uma página | `page_view` | ❌ Não |
| Pesquisar um produto | `search` | ❌ Não |
| Clicar em “Adicionar ao carrinho” | `add_to_cart` | ❌ Não |
| Iniciar checkout | `begin_checkout` | ❌ Não |
| Efetuar compra | `purchase` | ✅ Sim |
| Subscrever newsletter | `sign_up` | ✅ Sim |
| Enviar formulário de contacto | `generate_lead` | ✅ Sim |

> Podem ser considerados microconversões, pois demonstram intenção do utilizador, mas não representam necessariamente o objetivo final de venda.

<h2>Tarefa 2 — Definição de 5 objetivos</h2>

1. Objetivo 1 
    * Objetivo Aumentar o número de compras realizadas no website
    * Evento: purchase
    * KPI: Taxa de conversão de compra
    
2. Objetivo 2 
    * Objetivo Aumentar o número de potenciais clientes interessados
    * Evento: generate_lead
    * KPI: Número de leads / taxa de conversão de leads.

3. Objetivo 3 
    * Objetivo: Aumentar o número de utilizadores inscritos.
    * Evento: sign_up
    * KPI: Taxa de inscrição.

4. Objetivo 4 
    * Objetivo: Aumentar o número de utilizadores que passam do carrinho para o checkout.
    * Evento: begin_checkout
    * KPI: Taxa de passagem do carrinho para checkout.

5. Objetivo 5
    * Objetivo: Aumentar o número de utilizadores que adicionam produtos ao carrinho.
    * Evento: add_to_cart
    * KPI: Taxa de adição ao carrinho.
