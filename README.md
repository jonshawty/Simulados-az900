# Simulado AZ-900

Três simulados interativos para a certificação **Microsoft Certified: Azure Fundamentals (AZ-900)**, feitos em HTML/CSS/JS puro — sem dependências, sem build, basta abrir no navegador.

Usei os três para estudar, junto com o curso abaixo, e fui aprovado na prova real com **880/1000**.

- Curso usado como base de estudo: https://youtu.be/4ub1uGKQK6U?si=rfGdmA5V7p8Fu9vh

## Sobre

São três versões com propósitos diferentes:

**`az900-simulado.html`** — simulado básico, de aquecimento. 50 questões de múltipla escolha (4 alternativas), uma por conceito, para revisar vocabulário e serviços do Azure.

**`az900-simulado-avancado.html`** — simulado avançado, mais próximo do nível real da prova. 50 itens divididos em três formatos:
- 30 questões de cenário, com alternativas da mesma categoria (distratores mais difíceis de eliminar por exclusão)
- 10 baterias de 3 afirmações Sim/Não sobre um mesmo contexto — o item só conta como acerto se as 3 estiverem corretas
- 10 questões de múltipla seleção, em que é preciso marcar exatamente o conjunto certo de alternativas

**`az900-simulado-3.html`** — terceiro simulado, montado em cima de temas e formatos que caíram de verdade na prova real. 40 itens em seis formatos:
- Questões de cenário, Sim/Não e múltipla seleção (iguais ao avançado)
- Completar a frase, com um menu suspenso para escolher a palavra certa e preencher a lacuna
- Verdadeiro ou falso, com uma única afirmação por questão
- Identificar na tela, em que é preciso clicar no ícone certo numa recriação simplificada da barra do portal do Azure

Cobre especificamente pontos como VNet Peering vs. VPN vs. ExpressRoute, prazo máximo de Reserved Instances, Microsoft Purview, e escalabilidade horizontal/vertical.

## Funcionalidades

- Ordem das questões sorteada a cada tentativa
- Cronômetro regressivo com finalização automática ao zerar
- Navegação livre entre questões por uma grade lateral, com indicação de respondida/não respondida
- Pontuação final geral e por domínio do exame, com classificação por cor (dominado / a reforçar / revisar)
- Revisão completa ao final, questão por questão, com a resposta certa, a sua resposta e uma explicação
- Tema claro/escuro automático (segue a preferência do sistema)
- Responsivo, funciona em celular

## Banco de questões

As questões dos três simulados seguem os pesos oficiais dos três domínios do exame AZ-900:

| Domínio | Básico | Avançado | III | Peso oficial |
|---|---|---|---|---|
| Conceitos de nuvem | 14 | 14 | 11 | 25–30% |
| Arquitetura e serviços do Azure | 19 | 19 | 15 | 35–40% |
| Gerenciamento e governança do Azure | 17 | 17 | 14 | 30–35% |
| **Total** | **50** | **50** | **40** | |

## Como usar

Não tem instalação nem dependência. Basta baixar o repositório e abrir o arquivo `.html` desejado direto no navegador:

```bash
git clone <url-do-repositorio>
cd <pasta-do-repositorio>
open az900-simulado.html            # ou az900-simulado-avancado.html, ou az900-simulado-3.html
```

(em Linux, use `xdg-open` no lugar de `open`)

## Tecnologias

HTML, CSS e JavaScript puro. Nenhuma biblioteca externa além da fonte (Google Fonts, com fallback para fontes do sistema).

## Aviso

Este material é um simulado de estudo criado para fins pessoais e não é afiliado, endossado ou revisado pela Microsoft. A pontuação exibida é um percentual de acertos usado como referência aproximada — a prova real pontua em escala de 1 a 1000, com nota mínima de 700. As questões do tipo "identificar na tela" usam uma recriação simplificada do portal do Azure, feita à mão, e não uma captura de tela real.
