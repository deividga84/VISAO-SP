# Relatório — ZIP anti-crash EFDS 444

- Arquivos no ZIP: **377**
- Arquivos em `ro.alyn_sampmobile.game/files`: **356**
- Tamanho de `files`: **2.36 GiB**
- Integridade do ZIP: **OK**

## Conteúdo fora de `files`

- `configs/`: 4 arquivos
- `mods/`: 1 arquivos

## Comparação com as pastas atuais

| Referência | Arquivos atuais | Caminhos comuns | Iguais | Diferentes | Só no ZIP | Só na referência |
|---|---:|---:|---:|---:|---:|---:|
| `data-full/files` | 379 | 330 | 208 | 122 | 26 | 49 |
| `data-lite/files` | 379 | 330 | 208 | 122 | 26 | 49 |

## Decisão de instalação

- O ZIP contém `ro.alyn_sampmobile.game/files`; este é o conteúdo candidato a substituir integralmente `data-full/files` e `data-lite/files`.
- O ZIP não contém `client_config.json` nem `files.json`; os arquivos existentes em `download/` serão preservados.
- As pastas `cleo/`, `mods/`, `configs/` e `servers.json` ficam fora da pasta `files`; não serão misturadas nos diretórios `data-full/files`/`data-lite/files` sem solicitação específica.
- A substituição será feita com cópia de segurança local das versões atuais.
