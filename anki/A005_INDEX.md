# A005 — Índice Anki

Data de geração: 08/10/2026
Fonte: [A005, PDF canônico](https://drive.google.com/file/d/169yinJNU07rjHoNlO2c8aMUyvk6Pajzi/view)
Status da apostila: concluída em 08/10/2026 (16/16 questões finais acertadas).

## APKG
- **Download canônico:** https://drive.google.com/file/d/1mdXHf_UK6oY_Q1Qju_fvIu6MI8u_OsaF/view?usp=drivesdk
- **Arquivo:** `A005 - Anki - 08-10-2026.apkg`
- **77 notas e 77 cartões**, distribuídos por matéria:
  - 18 → `Analista::P1::Const_Regimentos` (P1-CONST 1);
  - 45 → `Analista::P2::Proc_Regimentos` (RICD 46–64, P2-PROC 2.1 parcial);
  - 14 → `Analista::P2::ASR_Transcrição_IA` (P2-ASR 1, 1.1–1.3).
- 50 perguntas abertas/casos para recuperação livre; 27 assertivas C/E.
- 3 cartões oficiais, já reproduzidos na A005: CESPE Câmara 2002 (2 itens) e CESPE FUB 2015 (1 item). Demais cartões: autorais.
- 33 cartões do Regimento marcados `acerto_com_duvida`, reforçando a dificuldade relatada de evocar a regra sem alternativas.
- 0 cartões `erro_real` nesta execução; não houve erro reportado na bateria final.

## Seleção e abrangência
Todos os cartões possuem frente autossuficiente e verso com resposta decisiva, explicação, contraste e fonte. ASR: função e arquiteturas; P1 Constitucional: conceitos, classificações, contexto e estrutura; RICD: competência, reunião, quórum, prazos, parecer, vista, recurso, fiscalização e rotinas úteis. Não foram antecipados os arts. 95–200 do RICD nem os subitens ASR 1.4+.

## Auditoria
- Texto regimental comparado com RICD da Câmara atualizado até a Resolução nº 34/2026 (arts. 46–64);
- sem alterações de modalidade normativa em perguntas e respostas: autoridade, condição, prazo, quórum, consequência, negação e exceção;
- arquivo ZIP APKG íntegro; SQLite `PRAGMA integrity_check = ok`; colunas de esquema AnkiDroid verificadas; consulta real de leitura de cartões reproduzida com sucesso;
- 77 GUIDs distintos, 77 frentes distintas, 77 notas/77 cartões;
- três nomes completos de baralho conferidos; sem variantes históricas;
- fontes clicáveis em 77 cartões;
- `SHA-256: 7bee81abf758050f8bc377f9c3166685a417393cbdf8bd28b983696d7722b8ba`.

## Estado no AnkiDroid
O APKG foi criado e armazenado no Drive. **Não foi importado ou sincronizado automaticamente** no Anki/AnkiDroid. A planilha `Apostilas e Anki` concentra status e link.

## Correção de importação — 08/10/2026

A primeira versão do APKG tinha defeito estrutural: a tabela SQLite `cards` foi gerada com `laps`, mas o AnkiDroid exige `lapses`. A importação falhou com erro 500 (`no such column: lapses`). O mesmo arquivo do Drive foi substituído pela versão corrigida, preservando os **77 GUIDs, conteúdos e nomes de baralhos**. O teste após correção executou o SELECT que falhava na captura de tela do candidato, validou ZIP CRC e `PRAGMA integrity_check = ok`. Este teste técnico não é confirmação de importação real no aparelho.

Hash da versão inválida (apenas rastreabilidade): `c86e2ddadeeb436f16880399971404613460e2ea255f598d974cc7984f69e1e8`. Hash corrigido: `7bee81abf758050f8bc377f9c3166685a417393cbdf8bd28b983696d7722b8ba`. Rebaixar o pacote anterior a OBSOLETO; usar sempre o link canônico acima.
