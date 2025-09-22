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
