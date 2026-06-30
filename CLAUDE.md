# CLAUDE.md — simulador-compra-aluguer

## O que é
**RentSimulatorBlazor** — simulador de **compra vs. aluguer** de habitação. Permite comparar, ao longo do tempo, o custo de comprar casa (com crédito) face a arrendar, ajudando a decidir qual a opção financeiramente mais vantajosa.

## Stack
- **Blazor WebAssembly** (.NET) — aplicação client-side que corre inteiramente no browser.
- **PWA** (Progressive Web App) — instalável, com `service-worker` e `manifest.webmanifest` para uso offline.
- **Bootstrap** para o layout/estilos.

## Estrutura
- `wwwroot/` — conteúdo estático publicado (HTML, CSS, `_framework/`, ícones, service worker).
- `wwwroot/index.html` — ponto de entrada da app.
- `web.config` — configuração para alojamento em **IIS**.
- `.gitignore` — exclusões de build do .NET.

## Notas
- Site **estático**, sem base de dados nem backend — toda a lógica corre no cliente.
- O conteúdo em `wwwroot/_framework/` é gerado pelo build/publish do .NET; não editar à mão.
