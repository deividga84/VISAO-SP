# API de dados do launcher

Os manifestos abaixo servem ao atualizador de `com.xyron.game`. Os arquivos de jogo ficam nos diretórios `data-full/files` e `data-lite/files` e são armazenados pelo Git LFS. O launcher consulta os manifestos em `raw.githubusercontent.com` e baixa os objetos reais do LFS em `media.githubusercontent.com`.

`client_config-{full,lite}.json` informa a versão 3 (igual ao APK fornecido, portanto sem solicitar uma atualização de APK) e aponta para o manifesto da variante. `files-{full,lite}.json` contém nome, caminho relativo e tamanho de cada arquivo. `update_sources.json` é a configuração embutida na versão atualizada do launcher.

A versão atual tem 379 entradas por variante. Os arquivos Full e Lite são idênticos nesta publicação; os manifestos e endpoints são mantidos separados para permitir atualizações futuras. O app grava os downloads em `getExternalFilesDir(null)`, normalmente `/storage/emulated/0/Android/data/com.xyron.game/files`, respeitando a filtragem existente por GPU.
