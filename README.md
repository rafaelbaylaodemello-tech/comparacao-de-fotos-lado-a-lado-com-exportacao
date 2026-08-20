# Comparação de fotos lado a lado com exportação

Visualizador para comparar duas fotos de paciente (antes/depois) lado a lado ou
em cima/baixo, com zoom, pan, divisória ajustável e exportação em PNG. Recriação
da tela **"Comparar fotos"** do Clinicorp usando os componentes e tokens do
**CliniDS2** (Design System da Clinicorp), em **light mode**.

## Funcionalidades

- **Lado a lado / Cima e baixo** — alternância de layout via componente **Tabs** do CliniDS2.
- **Inverter** — troca as fotos A/B de posição.
- **Redefinir** — volta zoom, pan e divisória ao estado inicial.
- **Zoom sincronizado** — aplica zoom/pan simultâneo nos dois painéis.
- **Divisória arrastável** — ajusta a proporção entre os frames.
- **Zoom (scroll)** e **pan (arrastar)** por painel.
- **Exportar** — compõe a comparação atual em um PNG.
- Arrastar uma imagem sobre um frame substitui a foto (para teste). Nenhuma
  imagem é enviada a servidores — todo o processamento é local no navegador.

## Design System

- **CliniDS2** — tokens semânticos (cores, tipografia, raio, sombra), light mode.
- Fonte **Roboto** em toda a interface.
- Componente **Tabs** extraído do Figma do CliniDS2 (node `17375:199556`):
  track `muted` raio 10px, trigger raio 8px, ativo em pílula branca com sombra `sm`.
- Ícones **Lucide** (utilitários).

## Uso

Abra o `index.html` em um navegador moderno. Não requer build nem dependências
locais (Tailwind e Lucide via CDN).

## Stack

HTML + Tailwind (Play CDN) + Lucide. Sem back-end.
