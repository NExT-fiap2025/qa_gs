Perfeito. Abaixo está a **estrutura completa da Entrega 1 (60 pts)** da disciplina de **Testing & Compliance (QA)**, feita **exatamente no padrão TOGAF e ArchiMate**, pronta para ser modelada no software **[Archi](https://www.archimatetool.com/)**.

---

# ✅ **📦 ENTREGA 1 – ARQUITETURA DA SOLUÇÃO (60 pts)**

**Projeto:** PowerGuard
**Ferramenta:** Archi – com linguagem ArchiMate 3.1
**Framework:** TOGAF 9.2

---

## 🔷 **MODELO NO PADRÃO TOGAF + ArchiMate (Dividido em 4 Modelos Visuais no Archi)**

---

### 🔹 **1. Visão de Arquitetura (Motivation Viewpoint)** – 15 pts

🧩 No Archi, crie uma **"Motivation View"** e use os elementos:

| Elemento ArchiMate | Conteúdo                                                              |
| ------------------ | --------------------------------------------------------------------- |
| `Stakeholder`      | Cidadão, Concessionária, Prefeitura, Equipe Técnica                   |
| `Driver`           | Alta frequência de quedas, Falta de resposta rápida                   |
| `Goal`             | Permitir registro de falhas, gerar relatórios, orientar usuários      |
| `Assessment`       | Conectividade limitada, baixa visibilidade de impacto, falta de canal |
| `Principle`        | Usabilidade, Resiliência, Modularidade, Interoperabilidade            |
| `Requirement`      | Persistência offline, registro simples, API REST, banco Oracle        |
| `Constraint`       | Conectividade instável, uso de Azure, tecnologias definidas           |

🔁 Relacione com setas:

- `Stakeholder` → `Driver`
- `Driver` → `Goal`
- `Goal` → `Requirement`
- `Requirement` → `Constraint`

---

### 🔹 **2. Arquitetura de Negócio (Business Layer View)** – 15 pts

🧩 Crie uma **"Business Process View"** e use:

| Elemento ArchiMate  | Exemplo no PowerGuard                                        |
| ------------------- | ------------------------------------------------------------ |
| `Business Actor`    | Usuário Final, App Mobile, Autoridade Pública                |
| `Business Role`     | Cidadão, Receptor de Dados, Responsável por Ações            |
| `Business Function` | Registro de Evento, Consulta de Histórico, Geração de Alerta |
| `Business Process`  | Registrar Queda de Energia, Receber Recomendação             |
| `Business Object`   | Evento de Falha, Relatório, Recomendação                     |

🔁 Relacionamentos:

- `Actor` → `Role` → `Process` → `Function` → `Business Object`

---

### 🔹 **3. Arquitetura de Sistemas (Application Layer View)** – 15 pts

🧩 Crie uma **"Application Structure View"** com:

| Elemento ArchiMate      | Exemplo no PowerGuard                                               |
| ----------------------- | ------------------------------------------------------------------- |
| `Application Component` | App Mobile, API Gateway, Serviço de Registro, Serviço de Relatórios |
| `Application Service`   | Registrar Evento, Gerar Relatório, Fornecer Recomendações           |
| `Data Object`           | Evento, Relatório, Recomendação                                     |

🔁 Ligações:

- `Component` → `Service` → `Data Object`

📌 Destaque: incluir comunicação REST entre app e serviços.

---

### 🔹 **4. Arquitetura de Tecnologia (Technology Layer View)** – 15 pts

🧩 Crie uma **"Infrastructure View"** com:

| Elemento ArchiMate     | Exemplo no PowerGuard                                         |
| ---------------------- | ------------------------------------------------------------- |
| `Device`               | Smartphone Android, Azure Server                              |
| `System Software`      | Oracle Database, Spring Boot, .NET, React Native runtime      |
| `Technology Service`   | API Gateway (HTTPS), Banco Oracle, Storage                    |
| `Technology Interface` | TCP/IP, JDBC, REST, AsyncStorage                              |
| `Node`                 | Servidor de Aplicação, Servidor de Banco, Ambiente Mobile     |
| `Artifact`             | Código do App, Scripts de Deploy, Pacote de instalação Oracle |

🔁 Estrutura:

- `Node` hospeda `System Software`
- `System Software` expõe `Technology Service`
- `Device` acessa `Interface` → `Service`

---

## 🧾 Documento de Apoio: Conformidade Metodológica (incluir no .doc/.pdf)

> A arquitetura foi modelada com base no **framework TOGAF 9.2**, utilizando a linguagem **ArchiMate 3.1**.
> Os quatro modelos criados no Archi refletem:
>
> - **Motivation Viewpoint** para visão estratégica
> - **Business Layer** para processos e papéis
> - **Application Layer** para os serviços de aplicação e componentes
> - **Technology Layer** para infraestrutura, rede e execução

---

## ✅ Próximo passo:

1. Abra o Archi ([https://www.archimatetool.com/](https://www.archimatetool.com/))
2. Crie um novo modelo (File > New > ArchiMate Model)
3. Para cada entrega (1.1 a 1.4), crie uma **View** separada com o nome:

   - “01 – Visão de Arquitetura”
   - “02 – Arquitetura de Negócio”
   - “03 – Arquitetura de Sistemas”
   - “04 – Arquitetura de Tecnologia”

4. Exporte tudo como PDF: **File > Export View as PDF**
5. Inclua no `.zip` final com o documento descritivo e link do vídeo.
