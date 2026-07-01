# SOLPPE Toolkit

Toolkit de suporte para Windows com instaladores, reparos, configurações de rede, drivers de impressora e utilitários de atendimento.

## Downloads

Os executáveis oficiais são publicados em [Releases](https://github.com/Nata-Felix/SOLPPE-Toolkit/releases):

- `SOLPPE_toolkit.exe`: aplicativo principal.
- `SOLPPE_updater.exe`: atualizador automático validado por SHA-256.

## Estrutura

- `gui/ToolkitAllGui.cs`: interface e orquestração do toolkit.
- `gui/SolppeUpdater.cs`: atualizador automático.
- `toolkit_all.ps1`: ações de suporte executadas pelo aplicativo.
- `instalar.ps1`: instalação do Crystal Reports e dependências.
- Release `v1.0`: dependências utilizadas pelas ações do toolkit.
- Release `drivers-impressoras-v1`: catálogo e pacotes de drivers.

## Compilação

No Windows, execute:

```powershell
powershell -NoProfile -ExecutionPolicy Bypass -File .\gui\build.ps1
```

O build gera `SOLPPE_toolkit.exe` e `SOLPPE_updater.exe` na raiz do repositório.

Os executáveis e pacotes exclusivos do instalador TekFarma permanecem separados no repositório original.
