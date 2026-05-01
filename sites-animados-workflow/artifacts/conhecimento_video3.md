# 5 Segredos Para Criar Sites Incríveis — Gustavo Campelo

> **Fonte:** YouTube — [5 Segredos Para Criar Sites Incríveis](https://www.youtube.com/watch?v=ZmLx28d1bkE)  
> **Canal:** Gustavo Campelo - Desenvolvedor  
> **Duração:** 27:45 | **Views:** ~8.962 | **Data:** 04/03/2026

---

## Resumo

Vídeo focado nos **5 pilares/segredos** que diferenciam um site padrão de um site premium de alto nível. Complementa os outros vídeos com foco em **fundamentos de design e animação** que devem estar presentes em qualquer projeto.

---

## 🔑 Os 5 Segredos (Pilares do Site Incrível)

### Segredo 1 — Hierarquia Visual
- Disposição estratégica dos elementos na tela
- O olho do usuário deve ser guiado naturalmente pelo conteúdo
- Tipografia, espaçamento e tamanhos devem criar camadas de importância

### Segredo 2 — Animações Scroll-Triggered
- Elementos surgem, se movem ou se transformam ao rolar a página
- Cria sensação de "site vivo" e engajante
- **Atenção:** Pode afetar o PageSpeed se mal implementado (ver alerta abaixo)

### Segredo 3 — Micro-Interações
- Hover effects, botões com feedback visual, transições suaves
- Detalhes que fazem o site parecer mais responsivo e premium
- Exemplos: botão que muda de cor/forma ao hover, ícones animados

### Segredo 4 — Workflow Figma → Claude Code
- Design profissional no Figma como base
- Uso de AI (Claude Code) para transformar o design em código funcional
- Conexão via MCP elimina re-trabalho manual

### Segredo 5 — Otimização de Assets
- Imagens em **WebP** (menor que PNG/JPG, mesma qualidade)
- Vídeos em **WebM** (menor que MP4, compatível com browsers modernos)
- **Ferramenta de compressão:** Flow (para exportação de vídeo)

---

## ⚠️ ALERTA IMPORTANTE — Performance vs. Estética

> **Comentário de @rplmartins (7 likes):** Cuidado com animações pesadas que derrubam o **PageSpeed** — isso pode prejudicar o SEO e a experiência do usuário.

### Estratégia de Balanceamento:
```
✅ USE animações para elementos acima da dobra (hero section)
✅ USE scroll-triggered animations com lazy loading
✅ SEMPRE otimize vídeos com FFMPEG/WebM antes de subir
❌ EVITE animações em todos os elementos da página
❌ EVITE vídeos de fundo em alta resolução sem compressão
❌ EVITE usar MP4 — prefira WebM comprimido
```

---

## 🛠️ Ferramentas Mencionadas

| Ferramenta | Uso |
|---|---|
| **Figma** | Design/layout do site |
| **Claude Code** | Geração de código com IA |
| **Flow** | Exportação de vídeo animado |
| **Hostinger** | Hospedagem (cupom: `GUSTAVOCAMPELO`) |

---

## 💬 Comentário Técnico Relevante

**@gabriellhenrique666** perguntou sobre **gradientes pixelados em exports de 1080p no Flow** — indica que gradientes em vídeos exportados podem ter problema de qualidade. Solução: usar CSS gradients ao invés de gradientes em vídeo sempre que possível.

---

## 🏷️ Tags
`5-segredos` `hierarquia-visual` `micro-interacoes` `scroll-animation` `performance` `pagespeed` `figma` `claude-code` `webp` `webm` `flow-export`
