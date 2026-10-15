# API de dados do launcher

Os manifestos servem ao atualizador de `com.xyron.game`. Os arquivos de jogo ficam em `data-full/files` e `data-lite/files` e são armazenados no Git LFS. O launcher consulta os manifestos em `raw.githubusercontent.com` e baixa objetos LFS em `media.githubusercontent.com`.

Em 15 de outubro de 2026, o conteúdo completo de ambas as variantes foi substituído pelos 303 arquivos do pacote Android `MAPA DO GTA 5 MODIFICADO PARA GTA SA POWER`. A subpasta `com.rockstargames.gtasa/files` do pacote foi mapeada para a raiz de cada variante; os demais arquivos foram mantidos em seus caminhos relativos. Os manifestos Full e Lite têm 303 entradas cada e somam 2.261.500.523 bytes. O `.7z` de origem está em `download/MAPA_DO_GTA_5_MODIFICADO_PARA_GTA_SA_POWER_vr_ANDROID_By_4KLRZN_YT.7z`.

`client_config-{full,lite}.json` informa a versão 3, igual ao APK fornecido, e aponta para o manifesto da variante. `files-{full,lite}.json` contém nome, caminho relativo e tamanho de cada arquivo servido. `update_sources.json` é a configuração embutida no launcher. O manifesto legado `download/files.json` aponta para os arquivos da variante Full.

Como o pacote substituto não contém a pasta `SAMP/`, as novas variantes e seus manifestos não incluem `SAMP/server.ini` nem os demais arquivos antigos específicos do SA-MP.
