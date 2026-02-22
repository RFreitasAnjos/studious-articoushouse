# Problema de Negócio — Plataforma Anti-Fraude para E-commerce de Vinis e Artigos de Música

## 1. Contexto

O comércio eletrônico de vinis, discos raros e artigos musicais apresenta características específicas que aumentam significativamente o risco de fraude em transações digitais.  
Trata-se de um nicho com produtos de alto valor agregado, edições limitadas, vendas internacionais frequentes e baixa recorrência de compra por usuário.

Nesse cenário, fraudes financeiras causam impacto direto não apenas financeiro, mas também reputacional, afetando a confiança de clientes legítimos e parceiros comerciais.

---

## 2. Problema Central

Empresas que atuam no segmento de vinis e artigos de música enfrentam dificuldades em distinguir, em tempo real, transações legítimas de tentativas de fraude, especialmente em compras de alto valor ou realizadas a partir de diferentes regiões geográficas.

A ausência de um mecanismo antifraude próprio e explicável resulta em:
- Perdas financeiras por chargebacks
- Bloqueio indevido de clientes legítimos (falsos positivos)
- Dependência excessiva de soluções externas pouco adaptadas ao nicho
- Falta de rastreabilidade e explicabilidade das decisões de bloqueio

---

## 3. Características do Nicho que Impactam o Risco

- Produtos raros ou de edição limitada, com alto valor de revenda
- Compras internacionais recorrentes
- Divergência frequente entre país do comprador, país do pagamento e endereço de entrega
- Baixo histórico de compras por cliente (compras pontuais)
- Tentativas repetidas de pagamento em curto intervalo de tempo
- Uso de VPNs ou proxies para ocultação de origem

Essas características tornam inadequado o uso de regras genéricas de antifraude, exigindo um modelo de avaliação de risco adaptado ao domínio.

---

## 4. Impactos da Fraude no Negócio

### 4.1 Impacto Financeiro
- Chargebacks e estornos
- Custos operacionais adicionais
- Penalizações por adquirentes e gateways de pagamento

### 4.2 Impacto Operacional
- Necessidade de revisão manual de pedidos
- Aumento do tempo de processamento de compras
- Sobrecarga da equipe de atendimento

### 4.3 Impacto Reputacional
- Insatisfação de clientes legítimos
- Perda de confiança na plataforma
- Avaliações negativas e abandono do serviço

---

## 5. Necessidade de Negócio

Diante desse cenário, torna-se necessário o desenvolvimento de uma plataforma antifraude que:

- Avalie o risco de cada transação em tempo real
- Produza decisões claras: **Aprovar**, **Revisar** ou **Negar**
- Seja explicável e auditável
- Esteja alinhada às boas práticas de segurança da informação
- Seja adaptada especificamente ao nicho de vinis e artigos musicais

---

## 6. Objetivo do Sistema

O sistema tem como objetivo principal **reduzir perdas financeiras e operacionais causadas por fraudes**, mantendo uma boa experiência para clientes legítimos.

Para isso, o sistema deverá:
- Calcular um score de risco por transação
- Aplicar regras antifraude baseadas em características do pedido, do usuário e do contexto
- Registrar decisões e motivos de forma auditável
- Permitir evolução contínua das regras de risco

---

## 7. O Que o Sistema Não Pretende Resolver

Para manter o escopo controlado, este sistema **não tem como objetivo**:
- Substituir gateways de pagamento
- Implementar modelos avançados de machine learning na fase inicial
- Realizar análise manual de pedidos
- Armazenar dados sensíveis como informações completas de cartões

---

## 8. Público-Alvo

- Pequenos e médios e-commerces especializados em vinis e artigos musicais
- Lojas com vendas internacionais
- Operações que necessitam de maior controle antifraude sem perda de explicabilidade

---

## 9. Critérios de Sucesso

O projeto será considerado bem-sucedido se:
- Reduzir o número de fraudes confirmadas
- Manter baixo índice de falsos positivos
- Permitir auditoria clara das decisões antifraude
- Demonstrar uma arquitetura segura, organizada e escalável
