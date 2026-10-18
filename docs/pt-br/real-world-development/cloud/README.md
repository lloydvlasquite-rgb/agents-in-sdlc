---
slug: pt-br/real-world-development/cloud
title: "Agente do GitHub Copilot na nuvem"
authors:
  - geektrainer
lastUpdated: 2026-06-30
---

O **[agente do GitHub Copilot na nuvem](https://docs.github.com/copilot/concepts/agents/cloud-agent/about-cloud-agent)** permite que o GitHub Copilot trabalhe de forma assíncrona na nuvem. Você atribui o trabalho no GitHub, e o agente na nuvem assume a tarefa em segundo plano: explora o repositório, faz alterações e abre um pull request enquanto você pode se dedicar a outras atividades.

Ao longo destes exercícios, você vai adicionar instruções personalizadas para o agente na nuvem seguir e, em seguida, atribuir uma issue do GitHub para que ele implemente o trabalho. Você vai revisar e usar agentes personalizados para orientar a abordagem, monitorar e direcionar sessões pelo painel de agentes e, por fim, revisar os pull requests e iterar sobre os resultados.

## Exercícios

| Exercício | Tópico | Descrição |
|----------|-------|-------------|
| [0. Pré-requisitos][ex0] | Configuração | Crie seu repositório e codespace |
| [1. Instruções personalizadas][ex1] | Contexto | Adicione instruções personalizadas para o agente na nuvem seguir |
| [2. Agente na nuvem][ex2] | Agente assíncrono | Atribua issues ao agente do GitHub Copilot na nuvem |
| [3. Agentes personalizados][ex3] | Agentes especializados | Revise e use agentes personalizados |
| [4. Gerenciamento de agentes][ex4] | Monitoramento | Monitore e oriente as sessões do agente |
| [5. Iteração][ex5] | Revisão | Revise pull requests, itere sobre o trabalho do Copilot e escolha as próximas etapas |

## Pré-requisitos

Antes de participar deste workshop, verifique se você tem:

- [ ] Uma conta do GitHub com um plano ativo **Copilot Student, Pro, Pro+, Business ou Enterprise**
- [ ] O agente do GitHub Copilot na nuvem habilitado para sua conta ou organização

> [!TIP]
> Não tem um plano pago? Estudantes verificados podem obter o GitHub Copilot gratuitamente pelo [GitHub Education][callout-student-plan-education]. O plano **Copilot Student** inclui os recursos de agente, MCP, revisão de código e Copilot CLI usados neste workshop, para que você possa concluir todos os percursos.

[callout-student-plan-education]: https://github.com/education/students

> [!NOTE]
> O agente na nuvem está disponível nos planos **Copilot Student, Pro, Pro+, Business e Enterprise** — todos, exceto Copilot Free. No Copilot Business ou Enterprise, um administrador precisa habilitá-lo para a organização.

> [!NOTE]
> Este percurso não aborda MCP. Para explorar o uso de servidores MCP com o Copilot, consulte o [percurso de CLI][cli] ou o [percurso de VS Code][vscode].

## Comece

**[Comece pelo Exercício 0: Pré-requisitos →][ex0]**

[ex0]: 0-prerequisites/
[ex1]: 1-custom-instructions/
[ex2]: 2-cloud-agent/
[ex3]: 3-custom-agents/
[ex4]: 4-managing-agents/
[ex5]: 5-iterating/
[cli]: ../cli/
[vscode]: ../vscode/
