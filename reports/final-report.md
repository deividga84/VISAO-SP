# Relatório final — Data Especial 10k v1.0

## Fonte analisada

Arquivo: `DataEspecial10kv1.0✨(ComPostes&TodasGPUS)-SampMobile.7z`

- Tamanho compactado: **858.732.614 bytes** (aprox. 819 MiB)
- Tamanho descompactado: **1.909.364.387 bytes** (aprox. 1,78 GiB)
- Arquivos extraídos: **379**
- Pastas extraídas: **38**
- Integridade: **extração concluída sem erros pelo 7-Zip**
- Criptografia: **não**

## Estrutura instalada

O conteúdo extraído de `com.sampmobile.game/files` foi usado para substituir completamente os diretórios:

```text
data-full/files/
data-lite/files/
├── AZVoice/
├── SAMP/
├── anim/
├── audio/
├── data/
├── fonts/
├── models/
└── texdb/
```

## Verificação da substituição

- `data-full/files`: **379 arquivos**, idênticos ao conteúdo extraído do 7z.
- `data-lite/files`: **379 arquivos**, idênticos ao conteúdo extraído do 7z.
- Os dois diretórios são idênticos entre si.
- A substituição removeu os arquivos antigos dos diretórios ativos; eles não foram misturados nem duplicados.
- Os arquivos antigos foram preservados somente em backups locais fora dos diretórios ativos, para reversão:
  - `special-archive-analysis/backups-before-replacement-20260926-1317/data-full-files-original`
  - `special-archive-analysis/backups-before-replacement-20260926-1317/data-lite-files-original`

## Componentes relevantes

O pacote contém a organização típica do GTA/SAMP Mobile, além de componentes adicionais ou modificados:

- `AZVoice/`
- `texdb/vicio/`
- `texdb/Optimize_Fps.img`
- `texdb/Optimize_Lag.img`
- `texdb/patch_medium.img`
- `data/fixLagRockstarMobile.dat`
- Assets de `cutscene`
- Configurações e logs adicionais em `SAMP/`

## Publicação no GitHub

Destino solicitado: `deividga84/VISAO-SP`.

A publicação será feita preservando a estrutura de pastas e usando Git LFS quando necessário para os arquivos grandes. Nenhum arquivo será publicado fora desse repositório.
