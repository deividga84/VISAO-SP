# API de dados do launcher

Os manifestos servem ao atualizador de `com.xyron.game`. Os arquivos de jogo ficam em `data-full/files` e `data-lite/files` e são armazenados no Git LFS. O launcher consulta os manifestos em `raw.githubusercontent.com` e baixa os objetos LFS em `media.githubusercontent.com`. A exceção `playvicio.txt` é um arquivo vazio regular no Git (o LFS não publica objeto zero-byte) e, por isso, seu URL explícito nos manifestos aponta para `raw.githubusercontent.com`.

`client_config-{full,lite}.json` informa a versão 3, igual ao APK fornecido, e aponta para o manifesto da variante. `files-{full,lite}.json` contém nome, caminho relativo e tamanho de cada arquivo; o marcador vazio usa URL explícita. `update_sources.json` é a configuração embutida na versão atualizada do launcher.

Cada variante tem 379 entradas e 1.909.364.387 bytes. Os arquivos Full e Lite são idênticos nesta publicação; os manifestos e endpoints são separados para permitir atualização independente no futuro. O app grava arquivos em `getExternalFilesDir(null)`, normalmente `/storage/emulated/0/Android/data/com.xyron.game/files`, e aplica a filtragem original por GPU.
