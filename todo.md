Perfeito. Abaixo está o **resumo completo e detalhado** de tudo o que você deve entregar **exatamente como solicitado** na disciplina de **Testing & Compliance – GS 2025**, dividido por entregas:

---

## ✅ **ENTREGA 1 – Arquitetura da Solução via TOGAF/Archi (60 pontos)**

Cada seção vale 15 pontos:

### 🔹 1.1 Visão de Arquitetura (15 pts)

Modelo TOGAF com:

- **Stakeholders** (ex: moradores, técnicos da prefeitura, distribuidora de energia)
- **Drivers** (problema da falta de energia, lentidão na resposta, riscos à segurança)
- **Objetivos** (monitorar quedas, notificar autoridades, prevenir riscos)
- **Assessment** (ex: infraestrutura atual falha, apps não funcionam offline)
- **Princípios** (modularidade, interoperabilidade, escalabilidade, usabilidade)
- **Requisitos e restrições** (ex: deve funcionar offline; deve rodar em celulares Android; deve usar React Native)

### 🔹 1.2 Arquitetura de Negócio (15 pts)

- **Processos de negócio** (ex: registrar falha → armazenar → gerar alerta → recomendar ações)
- **Funções** (ex: coleta de dados, persistência local, geração de recomendações)
- **Atores e seus papéis** (usuário → reporta falha; app → gera alertas; servidor → analisa)

### 🔹 1.3 Arquitetura de Sistemas (15 pts)

- **Componentes de aplicação**: app mobile (React Native), backend (Spring Boot), serviço de alertas (C#), armazenamento local (AsyncStorage), banco SQL
- **Camadas de serviço**: camada de apresentação (mobile), camada de serviço (APIs), camada de dados (SQLite)
- **Componentes de dados**: eventos, localizações, tempos de interrupção, logs de alerta

### 🔹 1.4 Arquitetura de Tecnologia (15 pts)

- **Forma de conexão**: rede móvel/Wi-Fi → API REST → servidores Azure
- **Devices de acesso**: smartphones (Android), máquinas da Azure (backend), sensores (IoT com Python)
- **Servidores e softwares necessários**:

  - API Gateway (Spring Boot)
  - Backend C#
  - SQLite
  - React Native (frontend)
  - MediaPipe (IoT)
  - Archi para modelagem

✅ Todos os diagramas devem ser feitos **no Archi com ArchiMate**
✅ Gerar **um único PDF final com os 4 modelos** para a entrega

---

## ✅ **ENTREGA 2 – Documento de Apresentação do Projeto (20 pontos)**

### 🔹 2.1 Documento introdutório (10 pts)

- Nome do projeto (PowerGuard)
- Composição da equipe (Nome completo + RM)
- Descrição clara do **problema** a ser resolvido

### 🔹 2.2 Público-alvo e impacto (10 pts)

- Definir público (ex: moradores de regiões afetadas por apagões, serviços essenciais)
- Justificar com **dados/estatísticas de mercado**

  - Ex: "Mais de 95 mil quedas registradas em SP em 2023"
  - Ex: "Prejuízos estimados em R\$ 2 bilhões/ano por falhas de energia"

✅ Esse documento deve estar em formato `.docx` ou `.pdf` e ir dentro do ZIP

---

## ✅ **ENTREGA 3 – Vídeo Pitch (20 pontos)**

Requisitos:

- Duração: **máximo 5 minutos**
- Deve conter:

  - ✅ Introdução ao problema
  - ✅ Oportunidade mapeada
  - ✅ Demonstração da solução (conceito, arquitetura ou impacto)
  - ✅ Valor agregado ao ser implementado (benefícios concretos)

✅ Publicar no YouTube com link **privado ou não listado**

---

## ✅ Entrega Final no Sistema (formato ZIP)

Conteúdo do `.zip`:

1. Documento descritivo (`.doc` ou `.pdf`)
2. Arquivo `.PDF` com a arquitetura gerada no Archi
3. Link do vídeo pitch

📌 **Atenção**: se faltar qualquer um desses 3 itens → **perde 10 pontos.**

---

### Deseja que a gente comece agora pela **Entrega 1.1 – Visão de Arquitetura (TOGAF)?**

Posso montar direto a estrutura para você importar no Archi.
