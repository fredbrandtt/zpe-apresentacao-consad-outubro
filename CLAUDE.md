# CLAUDE.md

Deck da **10ª Reunião Ordinária do CONSAD** (Investe Maranhão e ZPE Maranhão), 29/10/2026, on-line. Parte da ZPE na ordem do dia do Ofício Circular nº 11/2026 (`fontes/`): item II (Missão China e CDRU com a NexSolar) e item III (comprovação de 10% das obras ao CZPE e carteira de projetos).

Feito a partir do template `slides/deck-relatorio` do design system ZPE (skill `zpe-maranhao-design`). Valem as regras do README do template: palco fixo 1920×1080 escalado pela largura, zona segura `150px 168px 190px`, grão em toda superfície, vídeos secundários sem autoplay. HTML, CSS e JS inline em `index.html`; os componentes novos ficam no fim do CSS, no bloco "COMPONENTES DO CONSAD DE OUTUBRO".

## Dados

- **`AGENDA`** (script no fim do `index.html`) é a fonte única da Missão China: monta o slide de roteiro e as contagens de cidades e agendas (`data-conta`). `ok: false` = agenda prevista sem confirmação da delegação (Zhuhai, CNS, Yantian, UBTECH); fica fora do slide e das contagens. Ao confirmar, troque para `true`.
- Conteúdo da missão: `../2026-10_missao-china-cobertura/` (`ROTEIRO_CONSOLIDADO.md`, matéria v2, `finals/fotos-imprensa/`). Empresas privadas aparecem só pelo setor (orientação da presidente).
- NexSolar e CZPE: áudio da presidência em `fontes/` (com transcrição). Carteira: Relatório Gerencial dos Entregáveis (posição de setembro).

## Comandos

```
npm install
npm run verificar        # 5 janelas: texto cortado, console, 404 (SHOTS=1 grava .shots/)
npm run pdf              # deck.pdf, uma página por slide
```
