# 📚 Guia Completo – Padrões de Projeto para Microsserviços
**Stack:** Java 25 + Spring Boot 4  
Organização: 5 semanas, 26 tópicos (1 artigo + 1 POC por dia útil).  

---

## 📑 Índice
- [Semana 1 – Fundamentos de Resiliência](#-semana-1--fundamentos-de-resiliência)
- [Semana 2 – Persistência e Processamento de Dados](#-semana-2--persistência-e-processamento-de-dados)
- [Semana 3 – Event-Driven e Escalabilidade](#-semana-3--event-driven-e-escalabilidade)
- [Semana 4 – Infraestrutura e Deploy](#-semana-4--infraestrutura-e-deploy)
- [Semana 5 – Estratégias de Modernização e Deploy](#-semana-5--estratégias-de-modernização-e-deploy)

---
# 📅 Semana 1 – Fundamentos de Resiliência
Guia de estudo com **Java 25 + Spring Boot 4**.  
Cada tópico é acompanhado de um **prompt estruturado** para gerar artigos e POCs.  

---

## 1. Circuit Breaker  
**Prompt:**  
Você é um arquiteto de software sênior, especialista em ecossistema Spring (Spring Boot 4.x/Spring Framework 6.x+) e Java moderno (Java 25), com vasta experiência em microsserviços resilientes e sistemas distribuídos. Seu papel é ser um mentor didático, criando planos de aprendizagem estruturados e práticos.  

**Instruções:** Crie um plano de estudo detalhado do absoluto ZERO ao HERÓI para dominar o padrão **Circuit Breaker** em microsserviços com Java 25 e Spring Boot 4.  

O plano deve ser dividido em fases ou módulos progressivos. Para cada módulo, detalhe:  
- **Nome e Objetivo da Fase**  
- **Conceitos-Chave**  
- **Prática Proposta**  
- **Exemplos de Código** (`resilience4j.circuitbreaker` em `application.yml` e uso de `@CircuitBreaker`)  
- **Recursos Recomendados**  
- **Duração Estimada**  
- **Checkpoint de Conclusão**  

**Foco Específico do Plano:**  
- Problema que o Circuit Breaker resolve (falhas em cascata).  
- Estados: fechado, aberto, meio-aberto.  
- Implementação com Resilience4j.  
- Configuração de thresholds e métricas.  
- Integração com observabilidade.  

**Público-Alvo:** Dev Java intermediário em Spring Boot (MVC), iniciante em padrões de resiliência.  
**Tom de Voz:** Didático, encorajador e técnico.  
**Formato de Saída Esperado:** Estrutura organizada em Markdown.  

---

## 2. Retry (com Backoff + Jitter)  
**Prompt:**  
Você é um arquiteto de software sênior, especialista em ecossistema Spring (Spring Boot 4.x/Spring Framework 6.x+) e Java moderno (Java 25), com vasta experiência em microsserviços resilientes e sistemas distribuídos. Seu papel é ser um mentor didático, criando planos de aprendizagem estruturados e práticos.  

**Instruções:** Crie um plano de estudo detalhado para dominar o padrão **Retry** em microsserviços com Java 25 e Spring Boot 4, enfatizando estratégias seguras como **exponencial backoff** e **jitter**.  

**Foco Específico do Plano:**  
- Riscos de Retry Storms.  
- Implementação com Resilience4j (`@Retry`).  
- Configuração de backoff exponencial e jitter no `application.yml`.  
- Laboratório: API instável → aplicar Retry + observabilidade.  

**Público-Alvo:** Dev Java intermediário em Spring Boot.  
**Formato Esperado:** Markdown com fases e exemplos práticos.  

---

## 3. Timeout  
**Prompt:**  
Você é um arquiteto de software sênior, especialista em ecossistema Spring (Spring Boot 4.x/Spring Framework 6.x+) e Java moderno (Java 25). Seu papel é ser um mentor didático, criando planos de aprendizagem estruturados e práticos.  

**Instruções:** Crie um plano de estudo detalhado para entender e aplicar **Timeouts** em chamadas de microsserviços Spring Boot 4 com Java 25.  

**Foco Específico do Plano:**  
- Diferença entre client timeout e server timeout.  
- Configuração de timeouts no `RestClient`/`WebClient`.  
- Ajustes de timeouts em JDBC (HikariCP).  
- Laboratório: API lenta → configurar timeout + fallback.  

**Formato Esperado:** Markdown estruturado com fases, práticas e checkpoints.  

---

## 4. Rate Limiter  
**Prompt:**  
Você é um arquiteto de software sênior, especialista em ecossistema Spring (Spring Boot 4.x/Spring Framework 6.x+) e Java moderno (Java 25). Seu papel é ser um mentor didático, criando planos de aprendizagem estruturados e práticos.  

**Instruções:** Crie um plano de estudo detalhado para aplicar o padrão **Rate Limiter** em microsserviços com Spring Boot 4 e Java 25.  

**Foco Específico do Plano:**  
- Limites de requisições (por usuário, IP, token).  
- Configuração de `resilience4j.ratelimiter`.  
- Implementação de Rate Limiter por endpoint.  
- Laboratório: simular 1000 requisições concorrentes → validar bloqueio/resposta 429.  

**Formato Esperado:** Markdown estruturado com fases, práticas e exemplos.  

---

## 5. Bulkhead  
**Prompt:**  
Você é um arquiteto de software sênior, especialista em ecossistema Spring (Spring Boot 4.x/Spring Framework 6.x+) e Java moderno (Java 25). Seu papel é ser um mentor didático, criando planos de aprendizagem estruturados e práticos.  

**Instruções:** Crie um plano de estudo detalhado para dominar o padrão **Bulkhead** em microsserviços com Spring Boot 4 e Java 25.  

**Foco Específico do Plano:**  
- Isolamento de recursos (pool de threads/conexões).  
- Configuração de Bulkhead com Resilience4j.  
- Diferença entre Bulkhead Semaphore e ThreadPool.  
- Laboratório: microsserviço com duas operações → isolar recursos para evitar impacto cruzado.  

**Formato Esperado:** Markdown estruturado com fases, práticas e checkpoints.  

---


# 📅 Semana 2 – Persistência e Processamento de Dados
Guia de estudo com **Java 25 + Spring Boot 4**.  
Cada tópico é acompanhado de um **prompt estruturado** para gerar artigos e POCs.  

---

## 6. Idempotência  
**Prompt:**  
Você é um arquiteto de software sênior, especialista em ecossistema Spring (Spring Boot 4.x/Spring Framework 6.x+) e Java moderno (Java 25), com vasta experiência em microsserviços resilientes e sistemas distribuídos. Seu papel é ser um mentor didático, criando planos de aprendizagem estruturados e práticos.  

**Instruções:** Crie um plano de estudo detalhado para dominar a **Idempotência** em microsserviços com Java 25 e Spring Boot 4.  

**Foco Específico do Plano:**  
- Conceito de idempotência em operações REST.  
- Estratégias com bancos relacionais e NoSQL.  
- Uso de tokens de idempotência.  
- Implementação em Spring Boot 4 (camada de serviço + repositório).  
- Laboratório: API de pagamentos que evita duplicidade de processamento.  

**Formato Esperado:** Markdown com fases, práticas e checkpoints.  

---

## 7. DLQ (Dead Letter Queue)  
**Prompt:**  
Você é um arquiteto de software sênior, especialista em ecossistema Spring (Spring Boot 4.x/Spring Framework 6.x+) e Java moderno (Java 25). Seu papel é ser um mentor didático, criando planos de aprendizagem estruturados e práticos.  

**Instruções:** Crie um plano de estudo detalhado para dominar o uso de **Dead Letter Queues (DLQ)** em microsserviços Java 25 + Spring Boot 4.  

**Foco Específico do Plano:**  
- O que são DLQs e por que são necessárias.  
- Configuração de DLQ em SQS e Kafka.  
- Consumidores Spring Boot 4 com tratamento de mensagens inválidas.  
- Estratégias de reprocessamento e monitoramento.  
- Laboratório: microsserviço consumidor que envia falhas para DLQ.  

**Formato Esperado:** Markdown estruturado com fases, práticas e exemplos.  

---

## 8. Saga Pattern (Orquestração vs Coreografia)  
**Prompt:**  
Você é um arquiteto de software sênior, especialista em ecossistema Spring (Spring Boot 4.x/Spring Framework 6.x+) e Java moderno (Java 25). Seu papel é ser um mentor didático, criando planos de aprendizagem estruturados e práticos.  

**Instruções:** Crie um plano de estudo detalhado para dominar o **Saga Pattern** em microsserviços, cobrindo tanto **orquestração** quanto **coreografia**, usando Spring Boot 4 e Java 25.  

**Foco Específico do Plano:**  
- Consistência eventual em sistemas distribuídos.  
- Diferença entre Saga Orquestrada e Coreografada.  
- Implementação em Spring Boot 4 usando orquestrador simples e eventos Kafka.  
- Laboratório: fluxo de pedido → pagamento → entrega.  

**Formato Esperado:** Markdown estruturado com fases, práticas e exemplos.  

---

## 9. API Composition  
**Prompt:**  
Você é um arquiteto de software sênior, especialista em ecossistema Spring (Spring Boot 4.x/Spring Framework 6.x+) e Java moderno (Java 25). Seu papel é ser um mentor didático, criando planos de aprendizagem estruturados e práticos.  

**Instruções:** Crie um plano de estudo detalhado para dominar o padrão **API Composition** em microsserviços com Java 25 + Spring Boot 4.  

**Foco Específico do Plano:**  
- Quando usar API Composition vs CQRS.  
- Implementação com `RestClient`/`WebClient`.  
- Estratégias de agregação e performance.  
- Laboratório: microsserviço que compõe dados de catálogo e preços em uma única resposta.  

**Formato Esperado:** Markdown estruturado com fases, práticas e exemplos.  

---

## 10. CQRS (Command Query Responsibility Segregation)  
**Prompt:**  
Você é um arquiteto de software sênior, especialista em ecossistema Spring (Spring Boot 4.x/Spring Framework 6.x+) e Java moderno (Java 25). Seu papel é ser um mentor didático, criando planos de aprendizagem estruturados e práticos.  

**Instruções:** Crie um plano de estudo detalhado para dominar o padrão **CQRS** em microsserviços com Java 25 + Spring Boot 4.  

**Foco Específico do Plano:**  
- Separação entre comandos e consultas.  
- Implementação em Spring Boot 4 (camada de comando + camada de leitura).  
- Integração com mensageria/eventos.  
- Laboratório: microsserviço de pedidos com persistência assíncrona de leitura.  

**Formato Esperado:** Markdown estruturado com fases, práticas e exemplos.  

---


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


# 📅 Semana 4 – Infraestrutura e Deploy
Guia de estudo com **Java 25 + Spring Boot 4**.  
Cada tópico é acompanhado de um **prompt estruturado** para gerar artigos e POCs.  

---

## 16. Service Discovery  
**Prompt:**  
Você é um arquiteto de software sênior, especialista em ecossistema Spring (Spring Boot 4.x/Spring Framework 6.x+) e Java moderno (Java 25), com vasta experiência em microsserviços distribuídos. Seu papel é ser um mentor didático, criando planos de aprendizagem estruturados e práticos.  

**Instruções:** Crie um plano de estudo detalhado para dominar **Service Discovery** em microsserviços com Java 25 + Spring Boot 4.  

**Foco Específico do Plano:**  
- Conceito de descoberta de serviços em ambientes distribuídos.  
- Diferença entre client-side e server-side discovery.  
- Exemplos com Eureka, Consul e AWS Cloud Map.  
- Laboratório: microsserviço Spring Boot 4 registrado e descoberto automaticamente.  

**Formato Esperado:** Markdown estruturado com fases, práticas, exemplos e checkpoints.  

---

## 17. Configuração Externa  
**Prompt:**  
Você é um arquiteto de software sênior, especialista em ecossistema Spring (Spring Boot 4.x/Spring Framework 6.x+) e Java moderno (Java 25). Seu papel é ser um mentor didático, criando planos de aprendizagem estruturados e práticos.  

**Instruções:** Crie um plano de estudo detalhado para aplicar **Configuração Externa** em microsserviços com Java 25 + Spring Boot 4.  

**Foco Específico do Plano:**  
- Conceito de externalizar configuração.  
- Uso de Spring Cloud Config, AWS Parameter Store, AWS Secrets Manager.  
- Estratégias de versionamento e segurança.  
- Laboratório: microsserviço com configs centralizadas.  

**Formato Esperado:** Markdown estruturado com fases, práticas, exemplos e checkpoints.  

---

## 18. Health Checks  
**Prompt:**  
Você é um arquiteto de software sênior, especialista em ecossistema Spring (Spring Boot 4.x/Spring Framework 6.x+) e Java moderno (Java 25). Seu papel é ser um mentor didático, criando planos de aprendizagem estruturados e práticos.  

**Instruções:** Crie um plano de estudo detalhado para dominar **Health Checks** em microsserviços com Java 25 + Spring Boot 4.  

**Foco Específico do Plano:**  
- Diferença entre liveness e readiness probes.  
- Integração com Kubernetes e ECS.  
- Implementação com Spring Boot Actuator.  
- Laboratório: microsserviço com health endpoints integrados a orquestrador.  

**Formato Esperado:** Markdown estruturado com fases, práticas, exemplos e checkpoints.  

---

## 19. API Gateway / BFF  
**Prompt:**  
Você é um arquiteto de software sênior, especialista em ecossistema Spring (Spring Boot 4.x/Spring Framework 6.x+) e Java moderno (Java 25). Seu papel é ser um mentor didático, criando planos de aprendizagem estruturados e práticos.  

**Instruções:** Crie um plano de estudo detalhado para aplicar **API Gateway** e **BFF (Backend for Frontend)** em microsserviços com Java 25 + Spring Boot 4.  

**Foco Específico do Plano:**  
- Papel do API Gateway (roteamento, segurança, rate limiting).  
- Padrão BFF para múltiplos clientes.  
- Implementação com Spring Cloud Gateway.  
- Laboratório: microsserviço com API Gateway servindo apps web e mobile.  

**Formato Esperado:** Markdown estruturado com fases, práticas, exemplos e checkpoints.  

---

## 20. Sidecar Pattern  
**Prompt:**  
Você é um arquiteto de software sênior, especialista em ecossistema Spring (Spring Boot 4.x/Spring Framework 6.x+) e Java moderno (Java 25), com experiência em service mesh. Seu papel é ser um mentor didático, criando planos de aprendizagem estruturados e práticos.  

**Instruções:** Crie um plano de estudo detalhado para dominar o **Sidecar Pattern** em microsserviços com Java 25 + Spring Boot 4.  

**Foco Específico do Plano:**  
- Conceito de sidecar em arquiteturas distribuídas.  
- Exemplos com Envoy, Istio e Linkerd.  
- Integração com observabilidade, segurança e roteamento.  
- Laboratório: microsserviço Spring Boot 4 com sidecar Envoy em Kubernetes.  

**Formato Esperado:** Markdown estruturado com fases, práticas, exemplos e checkpoints.  

---


# 📅 Semana 5 – Estratégias de Modernização e Deploy
Guia de estudo com **Java 25 + Spring Boot 4**.  
Cada tópico é acompanhado de um **prompt estruturado** para gerar artigos e POCs.  

---

## 21. Strangler Fig Pattern  
**Prompt:**  
Você é um arquiteto de software sênior, especialista em ecossistema Spring (Spring Boot 4.x/Spring Framework 6.x+) e Java moderno (Java 25), com vasta experiência em modernização de sistemas legados. Seu papel é ser um mentor didático, criando planos de aprendizagem estruturados e práticos.  

**Instruções:** Crie um plano de estudo detalhado para dominar o **Strangler Fig Pattern** em microsserviços com Java 25 + Spring Boot 4.  

**Foco Específico do Plano:**  
- Conceito do padrão e analogia com a planta “estranguladora”.  
- Estratégias para migrar módulos legados gradualmente.  
- Implementação com roteamento progressivo via API Gateway.  
- Laboratório: migrar endpoint legado para microsserviço Spring Boot 4 mantendo compatibilidade.  

**Formato Esperado:** Markdown estruturado com fases, práticas, exemplos e checkpoints.  

---

## 22. Blue-Green Deployment  
**Prompt:**  
Você é um arquiteto de software sênior, especialista em ecossistema Spring (Spring Boot 4.x/Spring Framework 6.x+) e Java moderno (Java 25), com vasta experiência em pipelines CI/CD. Seu papel é ser um mentor didático, criando planos de aprendizagem estruturados e práticos.  

**Instruções:** Crie um plano de estudo detalhado para aplicar **Blue-Green Deployment** em microsserviços com Java 25 + Spring Boot 4.  

**Foco Específico do Plano:**  
- Conceito de ambientes Blue e Green.  
- Estratégias de switch instantâneo.  
- Deploy em Kubernetes/AWS ECS.  
- Laboratório: microsserviço com troca de tráfego simulando Blue → Green.  

**Formato Esperado:** Markdown estruturado com fases, práticas, exemplos e checkpoints.  

---

## 23. Canary Release  
**Prompt:**  
Você é um arquiteto de software sênior, especialista em ecossistema Spring (Spring Boot 4.x/Spring Framework 6.x+) e Java moderno (Java 25), com vasta experiência em microsserviços e observabilidade. Seu papel é ser um mentor didático, criando planos de aprendizagem estruturados e práticos.  

**Instruções:** Crie um plano de estudo detalhado para dominar **Canary Release** em microsserviços com Java 25 + Spring Boot 4.  

**Foco Específico do Plano:**  
- Conceito de liberar para pequena porcentagem de usuários.  
- Estratégias de monitoramento durante o canário.  
- Integração com métricas (Datadog, Prometheus, Grafana).  
- Laboratório: microsserviço Spring Boot 4 com release gradual controlado.  

**Formato Esperado:** Markdown estruturado com fases, práticas, exemplos e checkpoints.  

---

## 24. Feature Flags  
**Prompt:**  
Você é um arquiteto de software sênior, especialista em ecossistema Spring (Spring Boot 4.x/Spring Framework 6.x+) e Java moderno (Java 25). Seu papel é ser um mentor didático, criando planos de aprendizagem estruturados e práticos.  

**Instruções:** Crie um plano de estudo detalhado para aplicar **Feature Flags** em microsserviços com Java 25 + Spring Boot 4.  

**Foco Específico do Plano:**  
- Conceito de ativação/desativação de features.  
- Ferramentas (Unleash, LaunchDarkly, Togglz).  
- Integração com Spring Boot 4.  
- Laboratório: microsserviço com feature habilitada/desabilitada em runtime.  

**Formato Esperado:** Markdown estruturado com fases, práticas, exemplos e checkpoints.  

---

## 25. Shadow Deployment  
**Prompt:**  
Você é um arquiteto de software sênior, especialista em ecossistema Spring (Spring Boot 4.x/Spring Framework 6.x+) e Java moderno (Java 25). Seu papel é ser um mentor didático, criando planos de aprendizagem estruturados e práticos.  

**Instruções:** Crie um plano de estudo detalhado para dominar **Shadow Deployment** em microsserviços com Java 25 + Spring Boot 4.  

**Foco Específico do Plano:**  
- Conceito de duplicação de tráfego sem impactar usuários finais.  
- Estratégias de roteamento paralelo.  
- Monitoramento de consistência entre versões.  
- Laboratório: microsserviço recebendo tráfego shadow em paralelo à versão produtiva.  

**Formato Esperado:** Markdown estruturado com fases, práticas, exemplos e checkpoints.  

---

## 26. Observabilidade aplicada à Resiliência  
**Prompt:**  
Você é um arquiteto de software sênior, especialista em ecossistema Spring (Spring Boot 4.x/Spring Framework 6.x+) e Java moderno (Java 25), com experiência em observabilidade. Seu papel é ser um mentor didático, criando planos de aprendizagem estruturados e práticos.  

**Instruções:** Crie um plano de estudo detalhado mostrando como aplicar **Observabilidade** para medir a eficácia de padrões de resiliência (Circuit Breaker, Retry, Timeout) em microsserviços com Java 25 + Spring Boot 4.  

**Foco Específico do Plano:**  
- Logs estruturados, métricas e tracing distribuído.  
- Integração com Micrometer, OpenTelemetry e Datadog.  
- Dashboards de resiliência (taxa de fallback, latência, throughput).  
- Laboratório: microsserviço com CB/Retry/Timeout + observabilidade completa.  

**Formato Esperado:** Markdown estruturado com fases, práticas, exemplos e checkpoints.  

---
