Perfeito. Aqui está a **Etapa 1: Diagnóstico Inicial** do projeto **PowerGuard**, com respostas claras, diretas e alinhadas ao seu escopo real de entrega:

---

## 🔹 Etapa 1: Diagnóstico Inicial

### 1. **O que é?**

> Um sistema inteligente para registro, análise e resposta a falhas no fornecimento de energia elétrica em regiões afetadas por eventos climáticos extremos.

---

### 2. **O que faz?**

> Permite que usuários relatem quedas de energia diretamente pelo aplicativo, registra tempo de interrupção, local e prejuízos, oferece orientações de segurança, e sincroniza essas informações com servidores para gerar relatórios e insights para autoridades públicas e concessionárias.

---

### 3. **O que não é?**

> Não é um sistema de previsão climática, não realiza reparos automáticos na rede elétrica e não substitui a atuação técnica das concessionárias.
> Também não depende de conexão contínua à internet para funcionar.

---

### 4. **O que resolve?**

> A ausência de um canal simples, rápido e acessível para notificação de quedas de energia e a falta de visibilidade das autoridades sobre os impactos reais sofridos por cidadãos em regiões afetadas.

---

### 5. **O que oferece?**

> - Registro detalhado de falhas
> - Histórico local e por tempo
> - Suporte offline com armazenamento local
> - Dados organizados para mapeamento e resposta rápida
> - Reforço à cidadania digital e autonomia dos usuários

---

### 6. **O que representa?**

> Uma resposta tecnológica estratégica à vulnerabilidade energética, simbolizando resiliência, empoderamento do cidadão e uso ético da tecnologia para reduzir impactos sociais de desastres.

---

### 7. **O que sustenta?**

> - Conceitos de Engenharia de Software com arquitetura modular e escalável
> - React Native, Spring Boot, C#, Python e Oracle Database
> - Princípios de interoperabilidade, usabilidade, segurança e continuidade operacional
> - Alinhamento às diretrizes de desenvolvimento resiliente e urbano

---

Perfeito! Vamos retomar a **ENTREGA 1.1 – Visão de Arquitetura (TOGAF)** da disciplina de **Testing & Compliance (QA)**, que representa os primeiros 15 pontos.

Aqui está novamente, agora em **formato definitivo para modelagem no Archi**, com os componentes organizados:

---

## ✅ **ENTREGA 1.1 – Visão de Arquitetura TOGAF – PowerGuard**

### 🔹 **Stakeholders**

| Stakeholder                   | Papel                                                         |
| ----------------------------- | ------------------------------------------------------------- |
| **Cidadão afetado**           | Usuário final que registra falhas e recebe orientações        |
| **Equipe técnica municipal**  | Analisa relatórios e toma decisões operacionais               |
| **Concessionária de energia** | Receptor das informações para agir e mapear áreas críticas    |
| **Equipe de desenvolvimento** | Responsável pela criação e manutenção da solução              |
| **Serviços de emergência**    | Beneficiados indiretamente com maior visibilidade dos eventos |

---

### 🔹 **Drivers**

| Driver                        | Motivação                                                      |
| ----------------------------- | -------------------------------------------------------------- |
| Alta frequência de quedas     | Causa prejuízos financeiros e riscos à população               |
| Falta de resposta rápida      | Aumenta o impacto dos apagões e reduz a confiança da população |
| Ausência de dados organizados | Impede que prefeituras e empresas atuem de forma preventiva    |
| Dificuldade de comunicação    | População não consegue relatar falhas de forma eficiente       |

---

### 🔹 **Objetivos**

| Objetivo                                        | Resultado Esperado                                           |
| ----------------------------------------------- | ------------------------------------------------------------ |
| Permitir registro de falhas                     | Cidadão registra local, tempo e prejuízo com facilidade      |
| Armazenar dados offline                         | Garantir uso mesmo sem internet                              |
| Gerar relatórios automáticos                    | Facilitar análise e tomada de decisão por órgãos             |
| Oferecer recomendações úteis                    | Apoiar usuários durante e após o apagão                      |
| Integrar sistema a servidores externos (futuro) | Escalar uso da plataforma para prefeituras e concessionárias |

---

### 🔹 **Assessment**

| Situação Atual                         | Diagnóstico                                                   |
| -------------------------------------- | ------------------------------------------------------------- |
| Acesso à internet instável             | Exige persistência local via AsyncStorage                     |
| Pouca integração com serviços públicos | Inicialmente sem conexão direta com concessionárias           |
| Alta experiência técnica da equipe     | Possibilidade de integração futura com APIs externas          |
| Plataforma Azure disponível            | Uso como infraestrutura padrão (backend, banco, autenticação) |

---

### 🔹 **Princípios Arquiteturais**

| Princípio          | Aplicação no PowerGuard                                                                  |
| ------------------ | ---------------------------------------------------------------------------------------- |
| Modularidade       | Divisão em microserviços independentes                                                   |
| Usabilidade        | App intuitivo e acessível para qualquer cidadão                                          |
| Escalabilidade     | Uso de Azure com microserviços separados para backoffice e mobile                        |
| Interoperabilidade | APIs REST padronizadas para comunicação entre app, backend e futuramente outros sistemas |
| Resiliência        | Armazenamento offline, tolerância à falha de rede                                        |

---

### 🔹 **Requisitos**

| Tipo          | Descrição                                                             |
| ------------- | --------------------------------------------------------------------- |
| Funcional     | Registrar eventos de queda com local, tempo e descrição               |
| Funcional     | Exibir histórico local de interrupções                                |
| Funcional     | Gerar orientações baseadas em tipo de evento                          |
| Funcional     | Armazenar dados localmente (AsyncStorage)                             |
| Funcional     | Exportar dados para análise externa ou integração futura com serviços |
| Não Funcional | Funcionar offline                                                     |
| Não Funcional | Interface acessível e responsiva                                      |
| Não Funcional | Código modular com separação por camadas (Controller, Service, etc.)  |

---

### 🔹 **Restrições**

| Restrição                                       | Justificativa                                              |
| ----------------------------------------------- | ---------------------------------------------------------- |
| Conectividade instável                          | Exige design offline-first                                 |
| Infraestrutura restrita à Azure                 | Uso obrigatório conforme requisitos da disciplina          |
| Linguagens pré-definidas                        | React Native, Spring Boot, C#, Python                      |
| Aplicativo deve funcionar sem serviços externos | MVP inicial não pode depender de concessionária ou governo |

---

Perfeito! Vamos agora para a **ENTREGA 1.2 – Arquitetura de Negócio**, valendo **15 pontos**, conforme exigido na disciplina de QA (Testing & Compliance).

Aqui está a estrutura completa, já pensada para ser implementada no **Archi** com linguagem **ArchiMate**, separando:

- **Atores**
- **Papéis**
- **Funções**
- **Processos de Negócio**

---

## ✅ **ENTREGA 1.2 – Arquitetura de Negócio – PowerGuard**

---

### 🔹 **Atores e Papéis**

| Ator                        | Papel no Sistema                                             |
| --------------------------- | ------------------------------------------------------------ |
| **Cidadão / Usuário Final** | Reporta falhas, recebe recomendações, acessa histórico local |
| **App Mobile**              | Intermediário da interação, coleta e exibe dados             |
| **Servidor Backend**        | Armazena, processa e disponibiliza dados agregados           |
| **Autoridades Públicas**    | Futuro consumidor dos relatórios de falhas energéticas       |
| **Equipe Técnica (Dev)**    | Desenvolvedores e mantenedores do sistema                    |

---

### 🔹 **Funções de Negócio**

| Função                            | Descrição Operacional                                             |
| --------------------------------- | ----------------------------------------------------------------- |
| **Coleta de Dados Locais**        | Captura e armazenamento de dados sobre quedas de energia pelo app |
| **Persistência Offline**          | Armazenamento local no dispositivo usando AsyncStorage            |
| **Geração de Relatórios**         | Criação de relatórios para análise posterior                      |
| **Fornecimento de Recomendações** | Exibição de orientações com base no tipo de evento registrado     |
| **Visualização de Histórico**     | Exibição dos eventos salvos, categorizados por local/data         |
| **Exportação de Dados (futuro)**  | Geração de dados estruturados para análise externa                |

---

### 🔹 **Processos de Negócio**

| Processo                                   | Etapas ou Subprocessos                                                     |
| ------------------------------------------ | -------------------------------------------------------------------------- |
| **Registrar Evento de Falha**              | Captura de localização → tempo → descrição → persistência local            |
| **Consultar Histórico de Ocorrências**     | Acesso ao armazenamento local → listagem e filtragem dos dados             |
| **Receber Recomendações de Segurança**     | Identificação do tipo de evento → retorno de conteúdo estático ou dinâmico |
| **Sincronizar Dados com Backend (futuro)** | Detecção de conectividade → envio para API REST                            |
| **Gerar Relatório de Falhas Agregadas**    | (No backend) Processamento dos dados → estruturação por local e período    |
| **Consumir Relatórios por Autoridades**    | (No futuro) Acesso via portal ou API externa                               |

---

### 🔹 **Exemplo visual (para montar no Archi)**

Você pode estruturar da seguinte forma no Archi:

```
Business Actor: Usuário Final
 └── Business Role: Cidadão
     └── Business Process: Registrar Queda de Energia
         ├── Business Function: Captura de Localização
         ├── Business Function: Registro de Tempo
         └── Business Function: Armazenamento Offline
```

---

Ótimo! Vamos agora para a **ENTREGA 1.3 – Arquitetura de Sistemas**, valendo mais **15 pontos**, exigida na disciplina de **Testing & Compliance (QA)**.

Esta etapa foca em:

- Componentes de aplicação
- Componentes de dados
- Camadas de serviço

---

## ✅ **ENTREGA 1.3 – Arquitetura de Sistemas – PowerGuard**

---

### 🔹 **Componentes de Aplicação**

| Componente                   | Tecnologia/Função                                                  |
| ---------------------------- | ------------------------------------------------------------------ |
| **App Mobile**               | React Native + AsyncStorage (interface e coleta de dados)          |
| **API Gateway**              | Spring Boot (orquestra chamadas REST entre front e microsserviços) |
| **Serviço de Registro**      | C# (.NET Core) – responsável por armazenar eventos de falhas       |
| **Serviço de Relatórios**    | Java (Spring Boot) – agrega dados e estrutura relatórios           |
| **Serviço de Recomendações** | Python (microserviço leve com base de regras)                      |

---

### 🔹 **Componentes de Dados**

| Entidade de Dados         | Descrição                                                          |
| ------------------------- | ------------------------------------------------------------------ |
| **Evento de Falha**       | { id, localização, tempo início, tempo fim, descrição, prejuízos } |
| **Recomendações**         | Conteúdo estático ou baseado em tipo de evento                     |
| **Usuário (local)**       | Armazenado no app: nome, local, registros anteriores               |
| **Logs de Sincronização** | Histórico de envios ao backend                                     |
| **Relatórios Gerados**    | Dados agrupados por local/data, prontos para exportação            |

---

### 🔹 **Camadas de Serviço**

| Camada                      | Responsabilidade Principal                                               |
| --------------------------- | ------------------------------------------------------------------------ |
| **Apresentação (Frontend)** | Interface gráfica no app, formulário de registro, histórico, dicas       |
| **Serviço (API + lógica)**  | Regras de negócio, validação, transformação de dados, envio/recebimento  |
| **Dados (Persistência)**    | Armazenamento local (AsyncStorage), backend com Oracle Database na Azure |

---

### 🔸 **Fluxo de Comunicação**

```plaintext
[Mobile App] → [API Gateway] → [Serviço de Registro]
                            → [Serviço de Recomendações]
                            → [Serviço de Relatórios]
```

---

### 🔹 Exemplo de modelagem no Archi (resumo visual)

```
Application Component: Mobile App
 └── Application Service: Registrar Evento
     └── Data Object: Evento de Falha

Application Component: API Gateway
 └── Application Service: Roteamento REST

Application Component: Serviço de Registro
 └── Application Function: Armazenar Evento
     └── Data Object: Evento de Falha
```

---

Excelente! Agora fechamos a **ENTREGA 1.4 – Arquitetura de Tecnologia**, última parte da entrega 1 de **Testing & Compliance (QA)**, valendo **15 pontos**.

---

## ✅ **ENTREGA 1.4 – Arquitetura de Tecnologia – PowerGuard**

---

### 🔹 **Forma de Conexão em Rede**

| Elemento                | Descrição Técnica                                              |
| ----------------------- | -------------------------------------------------------------- |
| **App Mobile**          | Conecta à internet via rede móvel ou Wi-Fi                     |
| **Backend/API Gateway** | Hospedado na nuvem Azure, acessado por HTTPS                   |
| **Serviços internos**   | Comunicação entre microserviços via HTTP REST                  |
| **Fallback offline**    | Quando offline, dados são armazenados localmente até reconexão |

---

### 🔹 **Devices de Acesso dos Usuários**

| Dispositivo             | Papel na Solução                                 |
| ----------------------- | ------------------------------------------------ |
| **Smartphones Android** | Acesso principal dos usuários (React Native app) |
| **Tablets ou Web**      | (futuro) Acesso por autoridades via portal       |
| **Máquinas de DevOps**  | Utilizadas para deploy e manutenção dos serviços |

---

### 🔹 **Servidores e Infraestrutura**

| Elemento                  | Função                                     |
| ------------------------- | ------------------------------------------ |
| **Servidor de Aplicação** | Azure App Service com backend em Java + C# |
| **Servidor de Banco**     | Oracle Database hospedado na Azure         |
| **Servidor de Storage**   | Persistência de dados históricos e logs    |

---

### 🔹 **Softwares Necessários por Máquina**

| Máquina                       | Softwares Requeridos                                                          |
| ----------------------------- | ----------------------------------------------------------------------------- |
| **Mobile (usuário final)**    | App React Native instalado, permissões de localização e armazenamento         |
| **Servidor Backend**          | Java 17 (Spring Boot), .NET 7, Python 3.11, Oracle JDBC Client                |
| **Servidor API Gateway**      | Java 17 com Spring Cloud Gateway ou REST controller simples                   |
| **Servidor de Recomendações** | Python + regras estáticas ou MediaPipe (se integrado com visão computacional) |
| **Ambiente de DevOps**        | Git, Docker (opcional), GitHub Actions, Azure CLI                             |

---

### 🔹 Representação no Archi (exemplo visual)

```
Technology Node: Azure App Server
 └── Technology Service: API Gateway
     └── Technology Interface: HTTPS

Technology Device: Smartphone
 └── Technology Service: Mobile Interface
     └── Technology Interface: React Native App

Technology Node: Oracle DB Server
 └── Technology Service: Oracle Database
     └── Technology Interface: JDBC / TCP/IP
```

---
