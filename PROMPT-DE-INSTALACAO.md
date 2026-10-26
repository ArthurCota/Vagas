# Prompt de instalação

Abra uma conversa nova no Claude, **anexe os arquivos `painel/vagas-na-gringa.html` e `TAREFA.md`** deste repositório e cole o texto abaixo.

---

```
Quero instalar o painel "Vagas na Gringa" na minha conta. Anexei dois arquivos: vagas-na-gringa.html (a página) e TAREFA.md (o prompt da busca automática). Faça nesta ordem:

1. Leia os dois arquivos inteiros antes de publicar qualquer coisa.

2. Publique vagas-na-gringa.html como um artifact novo, sem mudar o código, com:
   - ícone "briefcase"
   - descrição: "Painel pessoal de vagas internacionais e projetos freelance, ranqueados pelo meu currículo."
   - capabilities exatamente assim:
     {"db": {"rules": [{"path": "", "read": "owner", "write": "owner"}]},
      "user": {},
      "mcp": {"servers": [{"server": "Claude Code Remote", "tools": ["fire_trigger"]}]}}
   Se o conector "Claude Code Remote" tiver outro nome de exibição na minha conta, use o nome certo e me avise.

3. Crie uma tarefa agendada chamada "Busca de vagas na gringa", de segunda a sexta às 7:43 no horário de São Paulo (CRON_TZ=America/Sao_Paulo 43 7 * * 1-5), com notificação push. O prompt da tarefa é todo o texto do TAREFA.md que vem depois da linha "---", trocando cada {{URL_DO_PAINEL}} pelo link do artifact que você acabou de publicar.

4. Com a ferramenta ArtifactData, grave no banco do painel o documento collection "sistema", doc_id "agenda", com {"triggerId": "<id da tarefa criada>", "horario": "seg–sex às 7:43"}. É isso que faz os botões do painel funcionarem.

5. Confira com um "list" da collection "sistema" que o documento foi gravado, fixe o painel na minha barra lateral e me diga em poucas linhas o que fazer agora.
```

---

## Depois de instalar

1. Abra o painel (fica fixado na barra lateral do claude.ai).
2. Suba seu currículo em PDF, DOCX ou TXT. Pode ser o PDF exportado do LinkedIn.
3. Ajuste os cargos, países, modalidade, contrato, nível e inglês.
4. Clique em **Buscar vagas novas**. Na primeira vez, o claude.ai pede para você autorizar o painel a iniciar a busca: aceite.
5. Em alguns minutos aparecem as vagas, a revisão do currículo e a ideia de projeto para o GitHub.
