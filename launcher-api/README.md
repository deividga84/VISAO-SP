# API de dados do launcher

Os manifestos servem ao atualizador de `com.xyron.game`. Os arquivos de jogo ficam em `data-full/files` e `data-lite/files` e são armazenados no Git LFS. O launcher consulta os manifestos em `raw.githubusercontent.com` e baixa objetos LFS em `media.githubusercontent.com`. A exceção `playvicio.txt` é um arquivo vazio regular no Git (não há objeto LFS zero-byte); seu URL explícito usa `raw.githubusercontent.com`.

O arquivo `SAMP/server.ini` das variantes aponta para `179.198.105.167:7584`. O launcher consulta o mesmo endereço por protocolo SA-MP sobre UDP para exibir status; isso configura o cliente e não hospeda nem abre a porta do servidor.

`client_config-{full,lite}.json` informa a versão 3, igual ao APK fornecido, e aponta para o manifesto da variante. `files-{full,lite}.json` contém nome, caminho relativo e tamanho; o marcador vazio usa URL explícita. `update_sources.json` é a configuração embutida no launcher.

Cada variante tem 379 entradas e 1.909.364.387 bytes. Full e Lite são idênticos nesta publicação; manifestos e endpoints são separados para atualização futura independente. O app grava em `getExternalFilesDir(null)` e mantém a filtragem original por GPU.
