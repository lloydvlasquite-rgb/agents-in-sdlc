---
slug: pt-br/real-world-development/cli
title: "GitHub Copilot CLI"
description: "Desenvolva, verifique e entregue duas alterações na Tailspin Toys enquanto aprende os modos, as personalizações, as ferramentas MCP e a automação de pull requests do Copilot CLI."
authors:
  - geektrainer
lastUpdated: 2026-09-18
---

O **[GitHub Copilot CLI][about-copilot-cli]** leva o GitHub Copilot ao terminal como assistente de programação agêntico. Ele explora bases de código, gera código, executa comandos e se conecta a ferramentas externas — tudo pela linha de comando, para que você continue trabalhando sem alternar para um editor gráfico.

O workshop acompanha um fluxo de trabalho contínuo na Tailspin Toys:

1. Prepare o projeto no GitHub Codespaces, instale o Copilot CLI e conheça seus recursos.
2. Faça uma pequena alteração de classificação por estrelas, revise-a no navegador e faça o merge manual do primeiro pull request (PR).
3. Comece pela issue de filtragem, defina a abordagem no modo Plan, implemente no modo Autopilot e revise no modo Interactive.
4. Atualize as instruções do repositório e aplique-as ao trabalho de filtragem.
5. Personalize a skill existente `quality-checks` e use-a para executar as verificações do projeto.
6. Adicione o servidor Playwright Model Context Protocol (MCP) e use-o para explorar a filtragem no navegador.
7. Crie um agente personalizado de garantia de qualidade (QA) e use-o para revisar requisitos, cobertura e evidências de verificação.
8. Revise todas as alterações de filtragem e use o Agent Merge no PR de filtragem.
9. Explore comandos de barra úteis para contexto, modelos, compartilhamento e delegação opcional na nuvem.

Para manter o foco do workshop, você criará dois PRs: um para as classificações por estrelas e outro para a filtragem, com as atualizações de instruções e da skill, o perfil de QA e os testes. O trabalho de filtragem e qualidade compartilha uma conversa e uma ramificação, permitindo que você aproveite o que já fez ao explorar cada ferramenta.

## Lições

| Lição | Tópico | Descrição |
| ------ | ----- | ----------- |
| [0. Pré-requisitos][ex0] | Configuração | Crie seu repositório e Codespace |
| [1. Instale o Copilot CLI][ex1] | Instalação | Instale e autentique o Copilot CLI e conheça seus recursos |
| [2. Adicione classificações por estrelas: uma melhoria rápida][ex2] | Primeira alteração | Exiba as classificações existentes e a alternativa quando não houver uma; depois, faça merge do primeiro PR |
| [3. Modos de agente: Plan e Autopilot][ex3] | Modos de agente | Planeje o recurso a partir da issue, implemente com Autopilot e revise no modo Interactive |
| [4. Oriente o Copilot com instruções personalizadas][ex4] | Contexto | Explore e atualize as instruções e aplique-as à filtragem |
| [5. Personalize e use uma skill de verificações de qualidade][ex5] | Verificações repetíveis | Explore a skill existente, altere o formato do relatório e execute-a |
| [6. Valide a funcionalidade com Playwright MCP][ex6] | Observação no navegador | Configure o MCP na CLI e inspecione o comportamento da filtragem |
| [7. Crie e use um agente de QA][ex7] | Requisitos e cobertura | Crie e selecione um perfil especializado e reúna as evidências finais de verificação |
| [8. Crie e faça merge do PR do recurso][ex8] | Revisão e merge | Revise todas as alterações, crie o PR e use o Agent Merge |
| [9. Comandos de barra no GitHub Copilot CLI][ex9] | Recursos da CLI | Explore contexto, modelos, compartilhamento e delegação opcional para o agente na nuvem |
| [10. Encerramento e próximas etapas][ex10] | Resumo | Revise o fluxo de trabalho, as personalizações reutilizáveis e outros recursos |
| [Opcional: incorpore o Foundry][foundry] | Agentes hospedados | Prepare um modelo, implante um agente fundamentado em catálogo e conecte-o ao site |

## Pré-requisitos

Antes de participar deste workshop, verifique se você tem:

- [ ] Uma conta do GitHub com um plano ativo **Copilot Student, Pro, Pro+, Business ou Enterprise**
- [ ] Permissão para criar um repositório e um Codespace
- [ ] Conhecimentos básicos de terminal ou linha de comando

> [!TIP]
> Não tem um plano pago? Estudantes verificados podem obter o GitHub Copilot gratuitamente pelo [GitHub Education][student-plan]. O plano **Copilot Student** inclui os recursos de agente, MCP, revisão de código e Copilot CLI usados neste workshop.

> [!NOTE]
> Se você usa o Copilot Business ou o Copilot Enterprise, confirme se o administrador habilitou o Copilot CLI.

## Comece

**[Comece pelos pré-requisitos →][ex0]**

[about-copilot-cli]: https://docs.github.com/copilot/concepts/agents/about-copilot-cli
[student-plan]: https://github.com/education/students
[ex0]: 0-prerequisites/
[ex1]: 1-install-copilot-cli/
[ex2]: 2-add-star-rating/
[ex3]: 3-agent-modes/
[ex4]: 4-custom-instructions/
[ex5]: 5-agent-skills/
[ex6]: 6-mcp-playwright/
[ex7]: 7-qa-agent/
[ex8]: 8-create-pull-request/
[ex9]: 9-cli-power-tools/
[ex10]: 10-review/
[foundry]: 8-foundry-agent/
