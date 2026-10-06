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

# PARTE II — MONITORIZAÇÃO DAS AÇÕES DOS UTILIZADORES

> Os dados fornecidos no exercício são:

| Evento | Ocorrências |
|---|---:|
| Visualização de páginas | 18.500 |
| Pesquisa de produtos | 4.200 |
| Adicionar ao carrinho | 2.400 |
| Iniciar checkout | 1.500 |
| Compra | 600 |
| Newsletter | 350 |
| Contacto | 180 |

<h3>Tarefa 3</h3>

> `a)` Qual é o evento com maior número de ocorrências?

`Resposta`:
O evento com maior número de ocorrências é Visualização de páginas (page_view), com 18.500 ocorrências.

> `b)` Quantos utilizadores chegaram ao checkout, mas não concluíram a compra?

Checkout:

1.500
Compras:

600
Logo:

1.500 − 600 = 900

`Resposta:`900 utilizadores chegaram ao checkout, mas não concluíram a compra.

> `c)` Qual é a taxa de conclusão do checkout?

Fórmula:

Compras ÷ Checkouts × 100
600 ÷ 1.500 × 100 = 40%

`Resposta:`
A taxa de conclusão do checkout é de 40%. Consequentemente, a taxa de abandono nesta etapa é: 100% − 40% = 60%

Ou seja, 60% dos utilizadores que iniciaram o checkout não concluíram a compra.