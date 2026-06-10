# 🧺 Wash Express 👕

> **Sistema inteligente de gerenciamento de lavanderia**

O **Wash Express** é uma plataforma dedicada à automação de operações em lavanderias. O sistema resolve o desafio da gestão manual de ordens de serviço (OS), proporcionando uma interface para atendentes, controle de status em tempo real e um sistema de notificações. Foi projetado com uma arquitetura modular que garante rastreabilidade total, desde a entrada da roupa até a entrega final ao cliente.

---

## 📚 Índice
- [Sobre o Projeto](#-sobre-o-projeto)
- [Funcionalidades Principais](#-funcionalidades-principais)
- [Arquitetura do Sistema](#-arquitetura-do-sistema)
- [Estrutura de Dados](#-estrutura-de-dados)
- [Autores](#-autores)

---

## 📝 Sobre o Projeto
O Wash Express nasceu para digitalizar e otimizar processos em lavanderias. O objetivo central é eliminar erros manuais, garantir a organização dos itens de cada cliente e agilizar a comunicação. O sistema é estruturado para suportar o crescimento do negócio, mantendo a integridade dos dados e a eficiência operacional.

---

## ✨ Funcionalidades Principais

* **Cadastro e Gestão de Clientes:** Centralização de dados para histórico e agilidade no atendimento.
* **Gerenciamento de Ordens de Serviço (OS):** Criação de pedidos com itens detalhados e status atualizados.
* **Rastreabilidade de Ciclo de Vida:** Acompanhamento visual de cada estado da roupa (lavagem, secagem, pronta).
* **Notificações Inteligentes:** Sistema desenhado para alertar o cliente automaticamente sobre a conclusão do serviço.

---

## 🏗 Arquitetura do Sistema
O sistema é organizado de forma modular, separando a interface do usuário das regras de negócio e da persistência.

* **Camada de Apresentação:** Interface direta do atendente.
* **Camada de Aplicação (Controladores):** Orquestra as requisições e valida as regras de negócio.
* **Camada de Domínio (Modelos):** Representa as entidades do negócio (Cliente, OS, Item).
* **Camada de Infraestrutura:** Responsável pela comunicação com o banco de dados e mensageria.

| Categoria | Diagrama |
| :--- | :--- |
| **Visão Geral** | [Arquitetura](./diagramas/diagrama_arquitetura.png) \| [Componentes](./diagramas/diagrama_componentes.png) \| [Implantação](./diagramas/diagrama_implantacao.png) |
| **Comportamento** | [Casos de Uso](./diagramas/diagrama_caso_uso.png) \| [Estados](./diagramas/diagrama_estados.png) \| [Comunicação](./diagramas/diagrama_comunicacao.png) |
| **Estrutura** | [Classes](./diagramas/diagrama_classes.png) \| [Modelo de Dados](./diagramas/modelo_dados.png) |

### Fluxos de Sequência
Os fluxos detalhados do sistema:
* [Abrir Ordem de Serviço](./diagramas/sequencia_abrir_os.png)
* [Atualizar Status](./diagramas/sequencia_atualizar_status.png)
* [Cadastrar Cliente](./diagramas/sequencia_cadastrar_cliente.png)
* [Registrar Retirada](./diagramas/sequencia_registrar_retirada.png)
* [Visão Geral do Sistema](./diagramas/sequencia_sistema.png)

---


## 💾 Estrutura de Dados
O modelo de dados segue as boas práticas de normalização para garantir a consistência das informações.

* **Cliente:** Entidade principal com os dados de contato.
* **Ordem de Serviço:** Entidade relacional que conecta o cliente aos serviços contratados.
* **Itens de Serviço:** Composição da OS, permitindo detalhamento minucioso de cada peça de roupa.

*(Insira aqui o seu Diagrama Entidade-Relacionamento - DER)*

---

## 👥 Autores
| 👤 Nome | 💼 Perfil |
|---------|----------|
| [Arthur Henrique de Lima Santos] | [[Link para GitHub](https://github.com/ArthurkkLS)] |

---

## 🙏 Agradecimentos
Agradeço à equipe de Engenharia de Software da PUC Minas e ao corpo docente pela orientação na estruturação deste projeto.

---

## 📄 Licença
Este projeto é distribuído sob a Licença MIT.
