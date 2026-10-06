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

<h2>Tarefa 3</h2>

> `a)` Qual é o evento com maior número de ocorrências?

`Resposta`:
O evento com maior número de ocorrências é Visualização de páginas (page_view), com 18.500 ocorrências.

> `b)` Quantos utilizadores chegaram ao checkout, mas não concluíram a compra?

`Resposta:`Checkout: 1.500
Compras: 600
Logo: 1.500 − 600 = 900, 
900 utilizadores chegaram ao checkout, mas não concluíram a compra.

> `c)` Qual é a taxa de conclusão do checkout?

`Resposta:`
Fórmula: Compras ÷ Checkouts × 100, então, 
600 ÷ 1.500 × 100 = 40%.
A taxa de conclusão do checkout é de 40%. Consequentemente, a taxa de abandono nesta etapa é: 100% − 40% = 60%

> `d)` Qual é a taxa de conversão de compra relativamente aos 18.500 eventos de visualização?

`Resposta:`
600 ÷ 18.500 × 100 = 3,24%.
A taxa de conversão de compra relativamente às visualizações é de aproximadamente 3,24%.

> `e)` Que etapa parece necessitar de maior atenção?

`Resposta:` A etapa que mais chama a atenção é o checkout.
Dos 1.500 utilizadores que iniciaram o checkout, apenas 600 concluíram a compra.
Isso representa: 40% de conclusão, 60% de abandono e 900 utilizadores perdidos

> `f)` Que informação adicional gostaria de consultar no GA4?

`Resposta:` Eu analisaria:
1. Taxa de abandono por dispositivo;
2. Taxa de abandono por navegador;
3. Tempo médio no checkout;
4. Erros ocorridos durante o pagamento;
5. Métodos de pagamento utilizados;
6. Localização dos utilizadores;
7. Origem/canal dos utilizadores;
8. Produtos mais abandonados;
9. Valor médio do carrinho;
10. Número de tentativas de pagamento;
11. Desempenho mobile vs. desktop;
12. Páginas específicas onde ocorre o abandono.

# PARTE III — ANÁLISE DE AQUISIÇÃO

| Canal | Utilizadores | Conversões | Taxa de conversão |
|---|---:|---:|---:|
| Pesquisa orgânica | 3.000 | 180 | **6%** |
| Facebook/Instagram | 4.000 | 120 | **3%** |
| Google Ads | 2.500 | 200 | **8%** |
| Email | 1.000 | 150 | **15%** |
| Acesso direto | 1.500 | 90 | **6%** |

### Cálculos

- **Pesquisa orgânica:** `180 ÷ 3.000 × 100 = 6%`
- **Facebook/Instagram:** `120 ÷ 4.000 × 100 = 3%`
- **Google Ads:** `200 ÷ 2.500 × 100 = 8%`
- **Email:** `150 ÷ 1.000 × 100 = 15%`
- **Acesso direto:** `90 ÷ 1.500 × 100 = 6%`

### 1. Maior volume de utilizadores

**Facebook/Instagram — 4.000 utilizadores.**

### 2. Maior número de conversões

**Google Ads — 200 conversões.**

### 3. Volume de tráfego vs. resultados

Sim. O Facebook/Instagram possui o maior volume de utilizadores, mas apresenta apenas **3% de conversão**.

O Email possui apenas 1.000 utilizadores, mas apresenta **15% de conversão**.

### 4. Canais a analisar com maior detalhe

1. **Email** — melhor taxa de conversão: 15%.
2. **Google Ads** — 200 conversões e 8%.
3. **Facebook/Instagram** — elevado volume, mas apenas 3%.

### 5. Outras métricas a consultar

- CPA — Custo por Aquisição
- ROI
- ROAS
- Receita por canal
- Valor médio da compra
- Engagement
- Tempo de interação
- Taxa de abandono
- Novos vs. recorrentes
- Conversões assistidas
- Dispositivo utilizado

---

# PARTE IV — COMPORTAMENTO E ENGAGEMENT

## Dados

| Página | Utilizadores | Tempo médio | Cliques no CTA |
|---|---:|---:|---:|
| Homepage | 5.000 | 35s | 250 |
| Produto A | 3.500 | 1m45s | 700 |
| Produto B | 3.000 | 1m20s | 450 |
| Blog | 2.500 | 2m30s | 150 |
| Contacto | 1.000 | 55s | 300 |

### Página com maior engagement

**Blog — 2m30s de interação média.**

### Página com mais cliques no CTA

**Produto A — 700 cliques.**

### Página com oportunidade de melhoria

**Blog.**

### Possível explicação

O Blog pode gerar alto engagement, mas baixo número de ações porque o utilizador está principalmente em modo de **consumo de informação**, e não necessariamente em modo de compra.

> **Resposta: Tempo de interação elevado não significa automaticamente desempenho elevado.**

---

# PARTE V — FUNIL DE CONVERSÃO

## Dados

```text
10.000 utilizadores
        ↓
6.000 visualizaram um produto
        ↓
2.500 adicionaram produto ao carrinho
        ↓
1.500 iniciaram checkout
        ↓
900 efetuaram pagamento
        ↓
750 compras concluídas
```

## Tarefa 6 — Taxas de passagem

| Etapa | Utilizadores | Taxa de passagem |
|---|---:|---:|
| Entrada | 10.000 | **100%** |
| Visualização do produto | 6.000 | **60%** |
| Adicionar ao carrinho | 2.500 | **41,67%** |
| Checkout | 1.500 | **60%** |
| Pagamento | 900 | **60%** |
| Compra | 750 | **83,33%** |

### Cálculos

- Entrada → Produto: `6.000 ÷ 10.000 × 100 = 60%`
- Produto → Carrinho: `2.500 ÷ 6.000 × 100 = 41,67%`
- Carrinho → Checkout: `1.500 ÷ 2.500 × 100 = 60%`
- Checkout → Pagamento: `900 ÷ 1.500 × 100 = 60%`
- Pagamento → Compra: `750 ÷ 900 × 100 = 83,33%`

---

## Tarefa 7 — Diagnóstico

### 1. Maior perda de utilizadores

Em termos absolutos:

**10.000 → 6.000 = perda de 4.000 utilizadores.**

Em termos proporcionais, a maior perda ocorre entre:

**Visualização do produto → Adicionar ao carrinho**

- Passagem: **41,67%**
- Abandono: **58,33%**

### 2. Possíveis causas

- Preço pouco competitivo
- Falta de informação
- Fotografias insuficientes
- Descrição pouco convincente
- Custos adicionais inesperados
- Falta de confiança
- Problemas de usabilidade
- Experiência mobile inadequada

### 3. Dados adicionais

- Produto individual
- Preço
- Dispositivo
- Origem do tráfego
- Localização
- Tempo na página
- Scroll
- Produtos visualizados
- Taxa de abandono
- Novos vs. recorrentes

### 4. Hipótese

> Os utilizadores visualizam os produtos, mas não os adicionam ao carrinho porque a página do produto não apresenta informação ou elementos de confiança suficientes para incentivar a decisão de compra.

### 5. Ação a testar

Realizar um **teste A/B** da página do produto.

**Versão A:** página atual.

**Versão B:** página com:
- CTA mais destacado
- Fotografias adicionais
- Avaliações de clientes
- Informação sobre entrega
- Política de devolução
- Benefícios do produto

**KPI principal:** taxa de `add_to_cart`.

---

# PARTE VI — RETENÇÃO E RECORRÊNCIA

## Dados

| Tipo de utilizador | Utilizadores | Compras |
|---|---:|---:|
| Novos | 8.000 | 500 |
| Recorrentes | 2.000 | 450 |

### Taxa de compra dos novos utilizadores

`500 ÷ 8.000 × 100 = 6,25%`

**Resposta: 6,25%.**

### Taxa de compra dos utilizadores recorrentes

`450 ÷ 2.000 × 100 = 22,5%`

**Resposta: 22,5%.**

### Interpretação

Os utilizadores recorrentes apresentam uma taxa de compra de **22,5%**, enquanto os novos apresentam **6,25%**.

A taxa dos recorrentes é aproximadamente **3,6 vezes superior**.

### Estratégias para aumentar a recorrência

1. Campanhas de email marketing
2. Remarketing
3. Programa de fidelização
4. Descontos para segunda compra
5. Recomendações personalizadas
6. Notificações de novos produtos
7. Conteúdo personalizado
8. Campanhas para clientes inativos

### Eventos a acompanhar

- `login`
- `return_visit`
- `purchase`
- `newsletter_signup`
- `repeat_purchase`
- `view_item`
- `add_to_cart`
- `begin_checkout`

---

# PARTE VII — INTERPRETAÇÃO E TOMADA DE DECISÃO

## Caso prático

| Indicador | Resultado |
|---|---:|
| Tráfego | 🟢 **+35%** |
| Engagement | 🔴 **−10%** |
| Cliques nos produtos | 🟢 **+20%** |
| Abandono do carrinho | 🔴 **+30%** |
| Compras | 🔴 **−8%** |

## 1. Problema principal

**O aumento do tráfego não está a resultar em aumento de vendas.**

As compras diminuíram **8%**, enquanto o abandono do carrinho aumentou **30%**.

## 2. Evidências

- Tráfego: **+35%**
- Cliques nos produtos: **+20%**
- Engagement: **−10%**
- Abandono do carrinho: **+30%**
- Compras: **−8%**

## 3. Possíveis causas

- Tráfego de baixa qualidade
- Campanhas a atrair utilizadores pouco qualificados
- Problemas no checkout
- Preço ou custos de entrega
- Problemas de pagamento
- Experiência mobile deficiente
- Lentidão do website
- Falta de confiança
- Diferença entre expectativa do anúncio e página de destino

## 4. Hipótese

> O aumento de tráfego está a trazer utilizadores menos qualificados e, simultaneamente, existem fricções na jornada de compra que estão a aumentar o abandono do carrinho e a reduzir as compras.

## 5. Ação corretiva

### Ação 1 — Analisar o checkout
Identificar exatamente onde os utilizadores abandonam.

### Ação 2 — Segmentar o tráfego
Comparar Facebook/Instagram, Google Ads, pesquisa orgânica, Email e acesso direto.

### Ação 3 — Realizar testes A/B
Testar diferentes versões de:
- Página de produto
- CTA
- Checkout
- Métodos de pagamento
- Informação sobre entrega

## 6. KPIs

**KPI principal:** Taxa de conversão de compra.

**KPIs secundários:**
- `add_to_cart`
- `begin_checkout`
- `purchase`
- Taxa de abandono do carrinho
- Receita
- Valor médio do pedido
- CPA
- ROAS

---

# PARTE VIII — DESAFIO FINAL

## Mini Plano de Otimização

### Problema identificado

**Elevado abandono no processo de compra, principalmente entre visualização do produto e adição ao carrinho.**

### Dados que comprovam

Dos **6.000 utilizadores que visualizaram produtos**, apenas **2.500 adicionaram um produto ao carrinho**.

- Taxa de passagem: **41,67%**
- Taxa de abandono: **58,33%**

### Hipótese

> Os utilizadores demonstram interesse pelos produtos, mas a informação apresentada, o preço, a confiança ou o processo de decisão não são suficientemente fortes para levá-los a adicionar o produto ao carrinho.

### Ação proposta

Implementar um **teste A/B das páginas de produto**, adicionando:

- CTA mais visível
- Fotografias adicionais
- Avaliações
- Informação de entrega
- Política de devolução
- Benefícios do produto
- Elementos de confiança

### KPI

**Taxa de `add_to_cart`.**

### KPIs secundários

- `begin_checkout`
- `purchase`
- Abandono do carrinho
- Receita por utilizador

### Resultado esperado

Aumentar a taxa de passagem:

**Produto → Carrinho**

de **41,67%** para **50% ou mais**.

### Como testar

**Grupo A:** página atual.

**Grupo B:** página otimizada.

Comparar:

```text
view_item
    ↓
add_to_cart
    ↓
begin_checkout
    ↓
purchase
```

---

# 📌 DIAGNÓSTICO FINAL

## Principal descoberta

O problema não está simplesmente na quantidade de tráfego.

Existe uma diferença clara entre **atrair utilizadores** e **transformá-los em clientes**.

| Canal | Utilizadores | Conversões | Taxa |
|---|---:|---:|---:|
| Facebook/Instagram | **4.000** | 120 | **3%** |
| Google Ads | 2.500 | **200** | **8%** |
| Email | 1.000 | 150 | **15%** |

O Facebook/Instagram apresenta o maior volume de utilizadores, mas o Email apresenta a melhor taxa de conversão e o Google Ads apresenta o maior número de conversões.

---

# 🎯 RESUMO DOS PRINCIPAIS RESULTADOS

| Indicador | Resultado |
|---|---:|
| Maior evento | **18.500 page_views** |
| Abandono no checkout | **900 utilizadores** |
| Conclusão do checkout | **40%** |
| Conversão compra/page_views | **3,24%** |
| Canal com mais utilizadores | **Facebook/Instagram — 4.000** |
| Canal com mais conversões | **Google Ads — 200** |
| Melhor taxa de conversão | **Email — 15%** |
| Página com maior engagement | **Blog — 2m30s** |
| Mais cliques CTA | **Produto A — 700** |
| Maior perda absoluta no funil | **4.000 utilizadores** |
| Maior perda proporcional | **Produto → Carrinho — 58,33%** |
| Taxa de compra novos | **6,25%** |
| Taxa de compra recorrentes | **22,5%** |
| Problema do caso final | **+30% abandono / −8% compras** |

---

# 💡 CONCLUSÃO

Uma análise de Growth & Analytics não deve limitar-se a perguntar:

> **“Quantas pessoas visitaram o website?”**

É necessário compreender toda a jornada:

```text
Aquisição
    ↓
Engagement
    ↓
Produto
    ↓
Carrinho
    ↓
Checkout
    ↓
Pagamento
    ↓
Compra
    ↓
Retenção
```

O objetivo final é transformar dados em decisões:

```text
DADOS
  ↓
PROBLEMA
  ↓
HIPÓTESE
  ↓
AÇÃO
  ↓
KPI
  ↓
TESTE
  ↓
OTIMIZAÇÃO
```
---

## 📚 Exercício Prático 5 — *Tracking, Eventos, Conversões e Análise de Desempenho*