# 📅 Semana 3 – Event-Driven e Escalabilidade
Guia de estudo com **Java 25 + Spring Boot 4**.  
Cada tópico é acompanhado de um **prompt estruturado** para gerar artigos e POCs.  

---

## 11. Event Sourcing  
**Prompt:**  
Você é um arquiteto de software sênior, especialista em ecossistema Spring (Spring Boot 4.x/Spring Framework 6.x+) e Java moderno (Java 25), com vasta experiência em microsserviços orientados a eventos. Seu papel é ser um mentor didático, criando planos de aprendizagem estruturados e práticos.  

**Instruções:** Crie um plano de estudo detalhado do ZERO ao HERÓI para dominar o padrão **Event Sourcing** em microsserviços com Java 25 + Spring Boot 4.  

**Foco Específico do Plano:**  
- Conceito de armazenar eventos em vez de estado.  
- Reconstrução de estado a partir de eventos.  
- Implementação em Spring Boot 4 usando Kafka/EventStore.  
- Laboratório: serviço de pedidos reconstruindo histórico completo a partir dos eventos.  

**Formato Esperado:** Markdown estruturado com fases, práticas, exemplos e checkpoints.  

---

## 12. Outbox Pattern  
**Prompt:**  
Você é um arquiteto de software sênior, especialista em ecossistema Spring (Spring Boot 4.x/Spring Framework 6.x+) e Java moderno (Java 25). Seu papel é ser um mentor didático, criando planos de aprendizagem estruturados e práticos.  

**Instruções:** Crie um plano de estudo detalhado para dominar o **Outbox Pattern** em microsserviços com Java 25 + Spring Boot 4.  

**Foco Específico do Plano:**  
- Problema de inconsistência entre banco e mensageria.  
- Estratégia de Outbox (tabela intermediária + processador).  
- Integração com Debezium/Kafka.  
- Laboratório: microsserviço de pagamentos → garantir publicação de eventos sem perda.  

**Formato Esperado:** Markdown estruturado com fases, práticas, exemplos e checkpoints.  

---

## 13. CDC (Change Data Capture)  
**Prompt:**  
Você é um arquiteto de software sênior, especialista em ecossistema Spring (Spring Boot 4.x/Spring Framework 6.x+) e Java moderno (Java 25). Seu papel é ser um mentor didático, criando planos de aprendizagem estruturados e práticos.  

**Instruções:** Crie um plano de estudo detalhado para dominar **Change Data Capture (CDC)** em microsserviços com Java 25 + Spring Boot 4.  

**Foco Específico do Plano:**  
- Conceito de captura de alterações em bases.  
- Uso de Debezium ou Striim.  
- Integração Spring Boot 4 + Kafka.  
- Laboratório: replicar alterações de uma tabela relacional para tópicos Kafka.  

**Formato Esperado:** Markdown estruturado com fases, práticas, exemplos e checkpoints.  

---

## 14. Sharding & Partitioning  
**Prompt:**  
Você é um arquiteto de software sênior, especialista em ecossistema Spring (Spring Boot 4.x/Spring Framework 6.x+) e Java moderno (Java 25). Seu papel é ser um mentor didático, criando planos de aprendizagem estruturados e práticos.  

**Instruções:** Crie um plano de estudo detalhado para dominar **Sharding e Partitioning** em bancos de dados e mensageria usando Java 25 + Spring Boot 4.  

**Foco Específico do Plano:**  
- Diferença entre sharding (dados) e partitioning (mensageria).  
- Estratégias de distribuição de carga.  
- Configuração em bancos relacionais e NoSQL.  
- Laboratório: dividir base de clientes em múltiplos shards.  

**Formato Esperado:** Markdown estruturado com fases, práticas, exemplos e checkpoints.  

---

## 15. Backpressure  
**Prompt:**  
Você é um arquiteto de software sênior, especialista em ecossistema Spring (Spring Boot 4.x/Spring Framework 6.x+) e Java moderno (Java 25), com experiência em programação reativa. Seu papel é ser um mentor didático, criando planos de aprendizagem estruturados e práticos.  

**Instruções:** Crie um plano de estudo detalhado para dominar o conceito de **Backpressure** em pipelines reativos usando Java 25 + Spring WebFlux.  

**Foco Específico do Plano:**  
- Problema de produtores rápidos vs consumidores lentos.  
- Uso de Project Reactor (Flux, Mono, operadores).  
- Estratégias de buffering, dropping, windowing.  
- Laboratório: API reativa que consome stream de dados com controle de backpressure.  

**Formato Esperado:** Markdown estruturado com fases, práticas, exemplos e checkpoints.  

---
