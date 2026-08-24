# EvoLift

**Evolua todos os dias.**

EvoLift é um aplicativo de treino offline-first: todos os dados de
treino, histórico e evolução do usuário ficam armazenados no próprio
aparelho, sem exigir conta ou conexão com a internet. Criar uma conta é
opcional e serve apenas para sincronizar dados entre aparelhos, quando o
usuário quiser.

Site: **https://deyvidsantos-commits.github.io/Evolift-Home/**

## Proposta

A maioria dos apps de treino trata o acesso à internet e a criação de
conta como pré-requisito. O EvoLift inverte essa prioridade: o app
funciona por completo no modo offline, e a nuvem é um recurso adicional,
não uma dependência.

## Principais recursos

- **Funciona 100% offline** — treinos, histórico, progresso e dados
  corporais ficam sempre no dispositivo.
- **Compatibilidade de equipamento** — o usuário cadastra o que tem
  disponível no seu espaço de treino, e o app identifica automaticamente
  quais exercícios são compatíveis.
- **Evolução acompanhada de verdade** — cargas, recordes pessoais e
  histórico completo de cada treino já realizado.
- **Conta opcional** — sincronização manual entre aparelhos via e-mail e
  senha, sem exigir conexão constante nem coleta além do necessário.

## Privacidade

O EvoLift foi desenhado com privacidade como padrão, não como exceção:
dados sensíveis (fotos corporais, medidas) nunca saem do dispositivo,
mesmo com uma conta ativa. Detalhes completos e o mecanismo de exclusão
de conta e dados:

- [Política de Privacidade](https://deyvidsantos-commits.github.io/Evolift-Home/privacy/)
- [Excluir conta e dados](https://deyvidsantos-commits.github.io/Evolift-Home/delete-account/)

## Tecnologia

Desenvolvido em Flutter, com persistência local em SQLite (via Drift) e
sincronização opcional na nuvem via Supabase (autenticação e banco de
dados). Foco atual em Android, com testes em iOS.

## Responsável

Deyvid Santos — deyvid.santos@gmail.com
