# 🏷️ Sistema de Leilões

Sistema desktop em Java para gerenciamento de leilões, com controle de produtos, licitantes e lances, integrado a banco de dados MySQL.

![Java](https://img.shields.io/badge/Java-ED8B00?style=flat&logo=openjdk&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat&logo=mysql&logoColor=white)
![JDBC](https://img.shields.io/badge/JDBC-007396?style=flat&logo=java&logoColor=white)
![NetBeans](https://img.shields.io/badge/NetBeans-1B6AC6?style=flat&logo=apache-netbeans-ide&logoColor=white)
![Status](https://img.shields.io/badge/status-em%20desenvolvimento-yellow)

---

## 📌 Sobre o projeto

O Sistema de Leilões é uma aplicação desktop desenvolvida para gerenciar o ciclo completo de um leilão: cadastro de produtos, registro de licitantes, controle de lances e atualização automática do status dos itens (À venda / Vendido).

O banco de dados foi modelado com diagrama entidade-relacionamento no **StarUML** antes da implementação, aplicando boas práticas de análise e projeto de sistemas.

Desenvolvido como projeto prático do Curso Técnico em Análise e Desenvolvimento de Sistemas — **Senac Online**.

---

## ✨ Funcionalidades

- 📦 Cadastro e gerenciamento de produtos leiloados
- 👤 Cadastro de licitantes
- 💰 Registro e controle de lances
- 🔄 Atualização automática de status (À venda → Vendido)
- 🗄️ Persistência completa com MySQL via JDBC

---

## 🛠️ Tecnologias utilizadas

| Tecnologia | Uso |
|---|---|
| Java SE | Linguagem principal |
| Java Swing | Interface gráfica |
| JDBC | Conexão com banco de dados |
| MySQL | Banco de dados relacional |
| StarUML | Modelagem do diagrama ER |
| NetBeans IDE | Ambiente de desenvolvimento |
| Git / GitHub | Versionamento de código |

---

## 🗂️ Estrutura do projeto

```
sistema-leiloes-java/
├── LeiloesTDSat/
│   └── src/
│       ├── modelo/         # Entidades (Produto, Licitante, Lance...)
│       ├── dao/            # Acesso ao banco de dados
│       ├── servico/        # Regras de negócio
│       └── visao/          # Interfaces Swing
├── database/               # Scripts SQL do banco de dados
├── lib/                    # Dependências (driver JDBC)
└── README.md
```

---

## ⚙️ Como executar

### Pré-requisitos
- Java JDK 17+
- MySQL 8.0+
- NetBeans IDE (recomendado)

### Passo a passo

1. Clone o repositório
```bash
git clone https://github.com/Alfhaven/sistema-leiloes-java.git
```

2. Importe o banco de dados
```bash
mysql -u root -p < database/leiloes.sql
```

3. Configure a conexão no arquivo `ConexaoBanco.java`

4. Abra o projeto no NetBeans e execute `Main.java`

---

## 👤 Autor

**Alvaro Freitas Santos**
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/alvaro-freitas-santos-aba1603a9/)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white)](https://github.com/Alfhaven)
