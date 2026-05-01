# 🚀 GUIA MESTRE — Sites Animados de Alto Nível
> Consolidação de 5 vídeos sobre sites e landing pages épicas
> Atualizado em: 2026-05-01

---

## 📚 BASE DE CONHECIMENTO (3 Vídeos)

| # | Vídeo | Canal | Foco Principal |
|---|-------|-------|---------------|
| 1 | [Criar Sites Animados Nunca Foi Tão Rápido](https://www.youtube.com/watch?v=jNIXAjLxv44) | Gustavo Campelo | Figma MCP + Claude Code + Spline |
| 2 | [Antigravity + Nano Banana 2 = R$25.000](https://www.youtube.com/watch?v=HrMVakatQHk) | Enzo Barbatto | Nano Banana + Kling + Scroll Video |
| 3 | [5 Segredos Para Sites Incríveis](https://www.youtube.com/watch?v=ZmLx28d1bkE) | Gustavo Campelo | 5 Pilares do Design Premium |
| 4 | [Landing Page com IA Sem Parecer IA](https://www.youtube.com/watch?v=TZ-JiwmZenM) | Tom Melo | Gravyx + Fuga do estilo genérico + Micro-interações |
| 5 | [Criar landing pages ÉPICAS com IA](https://www.youtube.com/watch?v=rLZsqDW_SP8) | Arthur Marquez | Prompt Engineering: Dramaturgia Visual |

---

## 🏗️ STACK COMPLETO

### Geração de Assets com IA
- **Gravyx** → Imagens e assets com estilo realista/fotográfico (evita o "visual IA genérico")
- **Nano Banana 2** → Imagens de produto premium com IA
- **Kling 3.0** → Image-to-Video (cria animação a partir da imagem)
- **Flow** → Exportação de vídeo animado (cuidado com gradientes em 1080p)

### Design
- **Figma** → Layout base do site
- **MCP (Model Context Protocol)** → Conecta Figma ao VS Code
- **Firecrawl** → Faz scraping de site de referência para a IA usar

### Programação com IA
- **Antigravity** → Nosso motor principal para geração de código e estrutura. Age como "Diretor Criativo" (Dramaturgia Visual) antes de codar.
- **Claude Code / Cursor** → Ferramentas base de IA para desenvolvimento
- **Aura.Build** → Geração do esqueleto e layout visual para ser refinado no Antigravity

### Elementos 3D
- **Spline** → Objetos 3D interativos sem precisar de Three.js

### Otimização
- **FFMPEG** → Compressão de vídeo para web
- **Handbrake** → Alternativa GUI ao FFMPEG
- **Squoosh.app** → Compressão de imagens para WebP

---

## 🎯 OS 5 SEGREDOS DO SITE INCRÍVEL

1. **Hierarquia Visual** — guiar o olhar do usuário com tipografia e espaçamento
2. **Scroll-Triggered Animations** — elementos que reagem ao scroll
3. **Micro-Interações** — hover effects, transições suaves nos botões
4. **Workflow Figma → IA → Código** — design profissional como base
5. **Otimização de Assets** — WebP + WebM + compressão

---

## ⚙️ WORKFLOW DEFINITIVO DE PROJETO (Framework Dramaturgia Visual)

```
╔════════════════════════════════════════════════╗
║          FASE 0 — BRIEFING (DIREÇÃO DE ARTE)   ║
╠════════════════════════════════════════════════╣
║  • Antigravity atua como Diretor Criativo      ║
║  • Definir: Sensação, Público, Energia e CTA   ║
║  • Usar referências reais (repo awesome-design)║
║  • Mapear a Dramaturgia Visual (tensão/alívio) ║
╔════════════════════════════════════════════════╗
║          FASE 1 — REFERÊNCIA E ASSETS          ║
╠════════════════════════════════════════════════╣
║  • Definir referência visual (Figma ou URL)    ║
║  • Firecrawl para scraping do site referência  ║
║  • Nano Banana 2 → gerar imagens de produto    ║
║  • Kling 3.0 → animar a imagem (vídeo 3D)      ║
╠════════════════════════════════════════════════╣
║          FASE 2 — DESIGN NO FIGMA              ║
╠════════════════════════════════════════════════╣
║  • Layout completo: tipografia, cores, espaços ║
║  • Definir hierarquia visual (5 Segredos #1)   ║
║  • Mapear animações desejadas                  ║
╠════════════════════════════════════════════════╣
║          FASE 3 — CÓDIGO COM IA                ║
╠════════════════════════════════════════════════╣
║  • Conectar Figma via MCP ao VS Code           ║
║  • Antigravity/Claude Code gera código base    ║
║  • Implementar scroll-triggered video          ║
║  • Adicionar micro-interações (hover effects)  ║
╠════════════════════════════════════════════════╣
║          FASE 4 — ELEMENTOS 3D                 ║
╠════════════════════════════════════════════════╣
║  • Criar objetos 3D no Spline                  ║
║  • Exportar como embed                         ║
║  • Integrar ao site                            ║
╠════════════════════════════════════════════════╣
║          FASE 5 — PERFORMANCE                  ║
╠════════════════════════════════════════════════╣
║  • FFMPEG: converter vídeos para WebM          ║
║  • Squoosh: converter imagens para WebP        ║
║  • Testar PageSpeed Insights                   ║
║  • Ajustar animações se score < 70             ║
╚════════════════════════════════════════════════╝
```

---

## 🎬 TÉCNICA: SCROLL-TRIGGERED VIDEO (Efeito Apple)

```javascript
// Hero Section com vídeo sincronizado ao scroll
const video = document.querySelector('#hero-video');
const section = document.querySelector('#hero-section');

window.addEventListener('scroll', () => {
  const rect = section.getBoundingClientRect();
  const scrollProgress = Math.max(0, Math.min(1,
    -rect.top / (rect.height - window.innerHeight)
  ));
  if (video.duration) {
    video.currentTime = scrollProgress * video.duration;
  }
});
```

---

## ⚡ OTIMIZAÇÃO DE MÍDIAS

### Converter MP4 → WebM com FFMPEG
```bash
# Conversão básica para web (qualidade alta)
ffmpeg -i input.mp4 -c:v libvpx-vp9 -crf 30 -b:v 0 -an output.webm

# Versão leve (scroll-triggered, sem áudio)
ffmpeg -i input.mp4 -c:v libvpx-vp9 -crf 40 -b:v 0 -vf scale=1920:-1 -an output.webm
```

### Formatos por tipo de conteúdo
| Tipo | Formato | Meta de Tamanho |
|------|---------|----------------|
| Imagem de produto | WebP | < 200KB |
| Vídeo hero (scroll) | WebM | < 5MB |
| Vídeo background | WebM | < 10MB |
| Fonte | WOFF2 | < 50KB |

---

## ⚠️ REGRAS DE PERFORMANCE (Anti-PageSpeed-Killer)

```
✅ USE animações apenas nos elementos acima da dobra
✅ USE scroll-triggered com requestAnimationFrame
✅ SEMPRE comprima vídeos antes de subir (WebM < 5MB)
✅ TESTE com PageSpeed Insights antes de entregar
❌ EVITE animar TODOS os elementos da página
❌ EVITE vídeos MP4 sem compressão
❌ EVITE gradientes em vídeo exportado (use CSS)
❌ NUNCA suba PNG/JPG sem converter para WebP
```

---

## ✅ CHECKLIST DE PROJETO

**Planejamento**
- [ ] Definir referência visual
- [ ] Mapear seções e animações desejadas
- [ ] Gerar assets com Nano Banana 2 (se produto físico)

**Desenvolvimento**
- [ ] Design no Figma + conectar MCP
- [ ] Gerar código base com Antigravity/Claude Code
- [ ] Implementar hierarquia visual (5 Segredos #1)
- [ ] Implementar scroll-triggered animations
- [ ] Adicionar micro-interações (hover, transições)
- [ ] Integrar elementos 3D (Spline)

**Performance**
- [ ] Converter imagens → WebP (Squoosh)
- [ ] Converter vídeos → WebM (FFMPEG)
- [ ] Testar PageSpeed Insights (meta: > 70 mobile)
- [ ] Ajustar animações se necessário

---

## 🔗 RECURSOS SALVOS

- **Vídeo 1:** https://youtu.be/jNIXAjLxv44
- **Vídeo 2:** https://youtu.be/HrMVakatQHk
- **Vídeo 3:** https://youtu.be/ZmLx28d1bkE
- **Vídeo 4 (Tom Melo):** https://youtu.be/TZ-JiwmZenM
- **Vídeo 5 (Arthur Marquez):** https://youtu.be/rLZsqDW_SP8
- **Repo Identidade Visual:** https://github.com/arthurmarquez/awesome-design-md
- **Gravyx (Imagens):** https://gravyx.com.br/
- **Squoosh (WebP):** https://squoosh.app
- **Spline 3D:** https://spline.design
