# GAME DO ÁTOMO V4 — HTML5

Jogo educacional de Química Analítica em português, para celular e computador.

## Conteúdo
- **300 perguntas com enunciados distintos**, 30 por fase, sem exercícios de cálculo.
- 10 fases temáticas, uma questão aleatória de cada fase em cada partida.
- Alternativas embaralhadas a cada partida.
- Qualquer erro encerra a partida; reinício obrigatório na fase 1.
- Ajudas: eliminar uma alternativa errada; auditório virtual (percentuais simulados); universitário virtual (sugestão da resposta). Cada uma pode ser usada uma vez por partida.
- Breves explicações após responder; efeitos sonoros sintetizados, com opção de silenciar.
- Ranking local de vencedores salvo no `localStorage` do navegador, com nome, turma, pontuação, data e código local.
- Exportação CSV (compatível com Excel e Planilhas Google).
- Pedido de prêmio por mensagem de e-mail pré-preenchida no aplicativo de correio; o aluno escolhe o destinatário e confirma o envio.

## Rodar offline
Abra `index.html` em um navegador moderno. O banco de perguntas está incorporado ao HTML: não é necessário servidor nem conexão com a internet.

## Publicar no GitHub Pages
1. Extraia o ZIP.
2. Envie `index.html` à raiz de um repositório GitHub.
3. Em Settings > Pages, selecione Deploy from a branch, `main`, `/ (root)`.
4. Salve e aguarde o endereço publicado.

`questions.json` é uma cópia editável do banco. Se alterar esse arquivo, é necessário atualizar também o JSON incorporado ao `index.html`.

## Limitações importantes
- O ranking **não é compartilhado entre aparelhos**; cada navegador possui seus próprios dados. Apagar os dados do navegador pode apagar o ranking.
- O CSV reúne somente os vencedores registrados naquele navegador.
- O código local **não valida uma vitória contra fraudes**. O professor deve conferir os resultados antes de conceder prêmios.
- O e-mail do aluno não é salvo no ranking. O pedido abre o aplicativo de e-mail, não é enviado automaticamente. O professor precisa informar/selecionar o destinatário.
- A votação do auditório é uma **simulação**, não uma pesquisa com pessoas reais.
