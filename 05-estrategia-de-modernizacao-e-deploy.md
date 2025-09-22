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
