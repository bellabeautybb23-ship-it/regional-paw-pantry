# PetRecorrente - Despensa Regional de Ração

> E-commerce de assinatura de ração com logística por cidade. MVP desenvolvido com Lovable.

**Link do App Publicado: (https://regional-paw-pantry.lovable.app/)
**Repositório:(https://github.com/bellabeautybb23-ship-it/regional-paw-pantry)

### 1. O Problema e a Solução
Tutores esquecem de comprar ração e petshops locais perdem venda recorrente. O PetRecorrente cria assinaturas por cidade, garantindo entrega mensal e fidelização.

### 2. Funcionalidades
- Landing Page: "Ração na porta, todo mês"
- Catálogo por cidade e tipo de ração
- Carrinho e Checkout
- Painel Admin: pedidos agrupados por cidade para entrega
- Exportação CSV de pedidos

### 3. Tecnologias
Lovable + Supabase (PostgreSQL) + React + Tailwind

### 4. Como Rodar
App já publicado no Lovable. Código 100% via prompt.

### 4.1 Segurança e Desafios
**Falhas identificadas pelo Lovable:** RLS desabilitado em profiles/products/cities, validação de preço no frontend, inputs sem sanitização.

**Correção aplicada:**
- Tentei usar "Try to fix all" mas a funcionalidade agora exige plano Pro (print anexado).
- Plano gratuito limitado a 5 créditos/dia, com renovação em 11h (print anexado com "0 crédito restante").
- Supabase gerenciado pelo Lovable não permite acesso direto via dashboard.supabase.com com project_id xfsvdxdmjhlbzfcsihpi - exige acesso pelo painel do Lovable.
- **Solução:** Correção planejada com prompt único de baixo custo: "Enable RLS on all tables. Public can read products/cities, user can only read own profile" - para aplicar assim que os créditos renovarem às 08:43. Isso demonstra consciência de LGPD.

### 5. Prompt Principal (Mega Prompt)
O projeto foi criado com prompt inicial detalhado com persona, requisitos funcionais e estrutura de banco (products, cities, subscriptions, orders).

### 6. Prints
<img width="899" height="1599" alt="m2" src="https://github.com/user-attachments/assets/fcd47624-f053-4b50-9e22-c6035a7e7c53" />
<img width="1599" height="899" alt="mm" src="https://github.com/user-attachments/assets/c5ae5639-42cb-4b2b-b3d3-f3bea5d6c6d7" />


