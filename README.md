# Vagas na Gringa

Painel pessoal no Claude para quem mora no Brasil e procura trabalho aqui ou fora. Você sobe o currículo, escolhe países e modalidade, e o Claude pesquisa vagas e projetos freelance todo dia, dá uma nota de compatibilidade para cada um e deixa o link pronto para aplicar.

## O que ele faz

- **Idiomas**: escolha até dois idiomas além do português, cada um com seu nível (o segundo pode ser "Nenhuma"). A nota de cada vaga considera os idiomas que ela pede.
- **Vagas CLT / PJ / estágio**: no Brasil ou fora, busca em LinkedIn, Gupy, Vagas.com, InfoJobs, Catho, Glassdoor, Indeed, Remotive, Himalayas, We Work Remotely, Remote OK, Wellfound, Turing e sites do Japão. Cada vaga ganha uma nota de 0 a 100, o motivo e o que falta no seu currículo.
- **Projetos freelance**: busca em Upwork, Freelancer.com, Workana, Contra, Guru, PeoplePerHour, Malt e 99Freelas, com filtro de valor mínimo e de preço fixo ou por hora.
- **Comparar currículo**: recalcula as notas das vagas que já estão no painel depois que você melhora o currículo, mostrando quanto cada uma subiu ou desceu.
- **Revisão do currículo**: nota pelo padrão de currículos que passam em triagem no mercado escolhido (Brasil, exterior ou os dois), correções em ordem de prioridade, título do LinkedIn, resumo profissional e trechos reescritos.
- **Projeto para o GitHub**: uma ideia de projeto de portfólio que cobre as skills que mais aparecem nas vagas e ainda faltam no seu currículo.
- **Busca automática**: roda de segunda a sexta às 7:43 e manda notificação no celular.

Seus dados ficam só na sua conta. Ninguém mais vê seu currículo nem suas vagas, nem quem tiver o link.

## Do que você precisa

Uma conta no [claude.ai](https://claude.ai) com artifacts, tarefas agendadas e o conector Claude Code Remote disponíveis.

## Como instalar

1. Baixe os arquivos [`painel/vagas-na-gringa.html`](painel/vagas-na-gringa.html) e [`TAREFA.md`](TAREFA.md).
2. Siga o [`PROMPT-DE-INSTALACAO.md`](PROMPT-DE-INSTALACAO.md): você abre uma conversa no Claude, anexa os dois arquivos e cola o prompt. O Claude publica o painel na sua conta e cria a busca automática.
3. Suba seu currículo no painel e clique em **Buscar vagas novas**.

## Arquivos

| Arquivo | O que é |
|---|---|
| `painel/vagas-na-gringa.html` | A página do painel |
| `TAREFA.md` | As instruções que a busca automática segue |
| `PROMPT-DE-INSTALACAO.md` | O texto para colar no Claude e instalar tudo |

## Dicas

- O painel funciona para qualquer área, mas os cargos vêm preenchidos com vagas de dados. Troque pelos seus antes de buscar.
- Para mudar o horário da busca ou adicionar uma função, abra uma conversa no Claude, cole o link do seu painel e peça.
- As vagas e projetos vêm de pesquisa na web. Confira sempre a página original antes de aplicar.
