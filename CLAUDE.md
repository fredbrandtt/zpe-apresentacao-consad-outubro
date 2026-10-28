# CLAUDE.md

Deck da **10ª Reunião Ordinária do CONSAD** (Investe Maranhão e ZPE Maranhão), 29/10/2026, on-line. Parte da ZPE na ordem do dia do Ofício Circular nº 11/2026 (`fontes/`): item II (Missão China e CDRU com a NexSolar) e item III (comprovação de 10% das obras ao CZPE e carteira de projetos).

Feito a partir do template `slides/deck-relatorio` do design system ZPE (skill `zpe-maranhao-design`). Valem as regras do README do template: palco fixo 1920×1080 escalado pela largura, zona segura `150px 168px 190px`, grão em toda superfície, vídeos secundários sem autoplay. HTML, CSS e JS inline em `index.html`; os componentes novos ficam no fim do CSS, no bloco "COMPONENTES DO CONSAD DE OUTUBRO".

## Dados

- **`AGENDA`** (script no fim do `index.html`) é a fonte única da Missão China: monta o slide de roteiro e as contagens de cidades e agendas (`data-conta`). `ok: false` = agenda prevista sem confirmação da delegação; fica fora do slide e das contagens. `via: true` (no card ou no item) = deslocamento, que aparece no slide mas não conta como agenda. Todas confirmadas em 28/10.
- Conteúdo da missão: `../2026-10_missao-china-cobertura/` (`ROTEIRO_CONSOLIDADO.md`, matéria v2, `finals/fotos-imprensa/`). Empresas privadas aparecem só pelo setor (orientação da presidente).
- **Fotos:** só as marcadas com `selecao_` em `materiais/` (escolha da delegação), copiadas para `assets/fotos/` com nome descritivo; hoje são 40, todas em uso. Cada foto vai para o slide da visita (murais de Nansha, Gaolan e Shenzhen; registro de Foshan). Foto de local incerto, se voltar a aparecer, vai para um mural no fim da missão. Toda foto abre ampliada com clique (lightbox no fim do script).
- CECPS (Hengqin): dados de imprensa pesquisados em 28/10 (fontes no rodapé do slide). Quatro fotos da seleção num mural pequeno na coluna da direita.
- Gaolan (Zhuhai, 21/10): a reunião entrou no slide de Gaolan porque a presidente disse que foi "na ZPE da China"; o INDICE da cobertura lembra que o CECPS foi no mesmo dia, com as mesmas roupas.
- NexSolar (empresa do projeto H2X) e CZPE: áudio da presidência em `fontes/` (com transcrição). A CDRU vale pelo contrato, assinado em 16/10 (o áudio diz 23/10); remuneração em `fontes/Projecao_Receita_ZPE_H2X.xlsx`. Carteira: Relatório Gerencial dos Entregáveis (posição de setembro).

## Comandos

```
npm install
npm run verificar        # 5 janelas: texto cortado, console, 404 (SHOTS=1 grava .shots/)
npm run pdf              # deck.pdf, uma página por slide
```
