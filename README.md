# Receitas-INF1A-02

Versão aprimorada do site da atividade prática de Biologia da turma INF1A, baseada no `Receitas-INF1A` e preparada para uso real durante a aula.

## Recursos

### Para alunos
- Escolha rápida do grupo.
- Visualização dos integrantes por número de chamada.
- Edição das receitas somente quando permitida.
- Perfil com nome, número, função e grupo.
- Avisos do professor.
- Status da atividade em tempo real ao abrir a página.
- Indicador de atividade finalizada/bloqueada.
- Interface responsiva para celular.
- Tema claro/escuro.

### Para o professor
- Dashboard de modo aula.
- Visão dos 6 grupos em uma única tela.
- Contagem de grupos por status.
- Status: não iniciado, em andamento, em revisão e finalizado.
- Relógio padrão de Brasília/São Paulo (`America/Sao_Paulo`).
- Publicação e limpeza de avisos para toda a turma.
- Organização de alunos por grupo e número de chamada.
- Criação de grupos.
- Upload de foto do trabalho para cada grupo.
- Histórico das alterações do grupo.
- Finalização que bloqueia as receitas do grupo.
- Reabertura de edição pelo professor.
- Exclusão de contas de alunos.

### Segurança e banco
- Novos recursos ficam protegidos por funções SQL `security definer` com verificação de papel do usuário.
- Histórico de atividade com RLS.
- Storage separado para fotos dos trabalhos.
- Receitas finalizadas não podem ser alteradas pelo fluxo de edição.

## Efeitos visuais

- Identidade visual inspirada em Biologia.
- Barra de progresso da rolagem.
- Elementos com entrada suave conforme aparecem na tela.
- Hover e profundidade nos cards.
- Fundo com detalhes orgânicos sutis.
- Animação decorativa do DNA.
- Suporte a `prefers-reduced-motion`.
- Layout responsivo para celular e desktop.

## Banco de dados

Os grupos e receitas continuam no Supabase. As novas ferramentas de aula usam a migração:

`supabase/migrations/20260920000000_classroom_tools.sql`

Depois de aplicar a migration no projeto Supabase, o dashboard e os recursos de status/histórico/fotos ficam disponíveis.

## Publicação

O projeto é estático e pode ser publicado pelo GitHub Pages usando a branch `main`.

`https://guilherme-augusto-inf.github.io/Receitas-INF1A-02/`
