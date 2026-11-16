# Adendo ao Plano de Gerenciamento de Configuração — N2-P2

**Projeto:** BBS Simulator (Dart)
**Responsável de GCS:** Bryan Bellinaso (`@BryanBellinaso`)
**Data:** 16/11/2026

Este adendo atualiza o Plano de Gerenciamento de Configuração (`Plano_Ger_Conf_DevOps_BBS_Final.pdf`, versão 1.1) com as configurações de GCS aplicadas no repositório na atividade N2-P2, conforme a Aula 1 do projeto Ongconecta. Onde este adendo e o plano divergirem, vale este adendo.

## 1. Plano de GCS como item de configuração

O plano (PDF) e este adendo estão versionados na pasta `docs/` e só mudam por Pull Request, como qualquer outro item de configuração.

## 2. Estrutura do repositório (atualiza a seção 4.3)

| Caminho | Item de configuração |
|---|---|
| `README.md` | Descrição do projeto e regras de GCS |
| `src/` | Código-fonte (`N1-E2_BBS_BryanBellinaso.dart`) |
| `docs/` | Plano de GCS e este adendo |
| `docs/evidencias/` | Evidências das configurações no GitHub |

## 3. Proteção da branch `main` (atualiza as seções 3.3 e 5.2)

- Push direto na `main` é bloqueado, inclusive para o administrador.
- Toda mudança entra por Pull Request, com no mínimo **1 aprovação**.
- Force push e exclusão da `main` são bloqueados.
- A evidência da recusa do push direto está em `docs/evidencias/`.

## 4. Par de revisão (atualiza a seção 5.2)

| Papel | Pessoa | Permissão |
|---|---|---|
| Autor / Responsável de GCS | Bryan Bellinaso (`@BryanBellinaso`) | Admin |
| Revisor (par) | Ricardo Fissmer (`@RicardoFissmer`) | Write |

## 5. Environments (atualiza a seção 3.2)

| Environment | Finalidade | Proteção |
|---|---|---|
| `staging` | Homologação antes da produção | Sem aprovação obrigatória |
| `production` | Versão usada pelos usuários finais | **Revisor obrigatório: Bryan Bellinaso (`@BryanBellinaso`)** |

Fluxo de promoção: branch `feature/*` → Pull Request aprovado pelo par → `main` → `staging` → aprovação de Bryan Bellinaso → `production`.
