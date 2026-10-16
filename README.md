# VISAO-SP

Repositório dos dados GTA/SAMP Mobile e dos arquivos consumidos pelo launcher do servidor.

Em 15 de outubro de 2026, o conteúdo das pastas de dados foi **substituído integralmente** pelos 303 arquivos do pacote Android **MAPA DO GTA 5 MODIFICADO PARA GTA SA POWER**. A subpasta `com.rockstargames.gtasa/files` do pacote foi mapeada para a raiz de cada variante, e os demais arquivos do pacote foram mantidos em seus caminhos relativos. As variantes Full e Lite agora contêm a mesma lista de arquivos e os mesmos conteúdos.

O pacote original está disponível em [`download/MAPA_DO_GTA_5_MODIFICADO_PARA_GTA_SA_POWER_vr_ANDROID_By_4KLRZN_YT.7z`](https://media.githubusercontent.com/media/deividga84/VISAO-SP/main/download/MAPA_DO_GTA_5_MODIFICADO_PARA_GTA_SA_POWER_vr_ANDROID_By_4KLRZN_YT.7z).

**Atenção:** a substituição removeu os arquivos antigos que não faziam parte do pacote, inclusive arquivos e configurações específicos do SA-MP como `SAMP/server.ini`. O pacote recebido não contém uma pasta `SAMP/`.

## Estrutura

- `data-full/files/` — 351 ficheiros, 1.512.761.190 bytes, extraídos de `skin modificada.zip`.
- `data-lite/files/` — cópia idêntica dos mesmos 351 ficheiros.
- `download/files.json` — manifesto legado da variante Full.
- `launcher-api/` — manifestos e configuração de fontes das variantes Full e Lite.
- `atualização/` — arquivos de atualização preservados do repositório.
- `reports/` — relatórios de análises anteriores do dataset.

Os ficheiros grandes dos datasets são armazenados com Git LFS. O launcher usa os manifestos GitHub/LFS e baixa cada ficheiro diretamente do repositório.
