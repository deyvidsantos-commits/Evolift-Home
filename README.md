# EvoLift — Home

Site público estático do aplicativo EvoLift (`com.evolift.app`), publicado
via GitHub Pages a partir da raiz deste repositório (branch `main`).

O código-fonte do aplicativo vive em um repositório separado e privado —
este repositório contém **apenas** as páginas estáticas abaixo, para poder
ser público sem expor código, documentação interna ou histórico de
desenvolvimento.

## Páginas publicadas

| Página | URL |
| --- | --- |
| Home / divulgação | https://deyvidsantos-commits.github.io/Evolift-Home/ |
| Política de Privacidade | https://deyvidsantos-commits.github.io/Evolift-Home/privacy/ |
| Excluir conta e dados | https://deyvidsantos-commits.github.io/Evolift-Home/delete-account/ |

As duas últimas são exigidas pelo Google Play para apps com criação de
conta (Política de Privacidade + URL pública de exclusão de conta/dados).

## Estrutura

```
index.html                      página inicial (divulgação do app)
privacy/index.html              Política de Privacidade
delete-account/index.html       Excluir conta e dados
assets/screenshots/*.svg        capturas de tela (placeholders — ver abaixo)
```

## Capturas de tela: placeholders a substituir

As imagens em `assets/screenshots/` (`home.svg`, `workouts.svg`,
`exercises.svg`, `progress.svg`) são placeholders gerados só para marcar
onde cada print real vai entrar — não são screenshots de verdade.

Para trocar por um print real:

1. Tire o print no aparelho/emulador (proporção 1080×2400 encaixa sem
   distorcer no molde de celular da página; outras proporções também
   funcionam, só cortam para preencher o quadro).
2. Salve como PNG ou JPG com o mesmo nome-base do placeholder que está
   substituindo (ex.: `home.png` para o print da tela Início).
3. Em `index.html`, atualize o(s) `<img src="assets/screenshots/home.svg">`
   correspondente(s) para apontar para o novo arquivo
   (`assets/screenshots/home.png`). A tela Início aparece duas vezes no
   HTML (hero + galeria) — atualize as duas ocorrências.
4. Delete o `.svg` antigo, se quiser.

## Conteúdo das páginas de privacidade

O conteúdo de `privacy/` e `delete-account/` é derivado do aviso de
privacidade técnico e factual do aplicativo
(`docs/PRIVACY_NOTICE.md`, no repositório principal) e da implementação
real da exclusão de conta (`delete_own_account()`). Responsável:
**Deyvid Santos** (deyvid.santos@gmail.com).

## Publicar mudanças

Qualquer commit na branch `main` é publicado automaticamente pelo GitHub
Pages em 1–2 minutos.
