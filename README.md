# BBS Simulator (Dart)

Aplicação de console em Dart que simula uma antiga BBS (Bulletin Board System), com mensagens organizadas nas áreas GERAL, GAMES, TECNOLOGIA e DOWNLOADS.

Disciplina: Gerenciamento, Configuração e Processos de Software (Prof. Luiz Camargo)
Autor: Bryan Bellinaso

## Estrutura do repositório

| Caminho | Conteúdo |
|---|---|
| `src/` | Código-fonte (`N1-E2_BBS_BryanBellinaso.dart`) |
| `docs/` | Plano de Gerenciamento de Configuração (item de configuração) e adendo N2-P2 |
| `docs/evidencias/` | Evidências das configurações de GCS no GitHub |

## Gestão de Configuração

- A branch `main` é protegida: o push direto é recusado e toda mudança entra por Pull Request com 1 aprovação.
- Par de revisão: Ricardo Fissmer (`@RicardoFissmer`), com acesso de escrita (Write).
- Environments: `staging` e `production`. O `production` exige aprovação de Bryan Bellinaso (`@BryanBellinaso`) como revisor obrigatório.
- Evidência da recusa do push direto: pasta [docs/evidencias](docs/evidencias)

## Como executar

```
dart run src/N1-E2_BBS_BryanBellinaso.dart
```

Também é possível colar o código no [DartPad](https://dartpad.dev).
