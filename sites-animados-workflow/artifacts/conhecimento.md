# Criar Sites Animados com IA — Workflow Completo

> **Fonte:** YouTube — [Criar Sites Animados Nunca Foi Tão Rápido](https://www.youtube.com/watch?v=jNIXAjLxv44)  
> **Canal:** Gustavo Campelo - Desenvolvedor  
> **Duração:** 27:51 | **Views:** ~15.900

---

## Resumo do Vídeo

O vídeo ensina como utilizar ferramentas de **Inteligência Artificial** e fluxos de trabalho modernos para criar sites com **animações de alto nível em tempo recorde**, focando na ponte entre design (Figma) e código funcional. O autor demonstra um workflow que permite criar sites profissionais valendo R$25.000 de forma muito mais rápida.

---

## 🔧 Ferramentas e Tecnologias Ensinadas

### 1. Claude Code / Claude Design (IA Copiloto Principal)
- Ferramenta de IA usada para **transformar designs em código funcional**
- Dado um layout no Figma, o Claude escreve o código HTML/CSS/JS automaticamente
- Foco em escrever prompts detalhados para gerar animações de qualidade

### 2. Figma com MCP (Model Context Protocol)
- Técnica de **conectar o Figma diretamente ao VS Code via MCP**
- Permite que a IA "leia" o design no Figma e gere o código correspondente
- Workflow: Design no Figma → Claude lê via MCP → Código gerado automaticamente
- Este é o diferencial principal do método ensinado

### 3. Spline (Elementos 3D Interativos)
- Ferramenta para criar e integrar **elementos 3D em sites web**
- Permite animações 3D interativas sem conhecimento profundo de Three.js
- Integra facilmente como embed ou componente no site

### 4. Google Antigravity
- Citado como ferramenta para criar **animações complexas e experiências 3D** de forma simplificada
- Facilita o desenvolvimento de experiências de alta qualidade

### 5. Nano Banana 2 / Stitch / Vibe Code
- Metodologias ou ferramentas específicas do autor para elevar a qualidade dos projetos
- Mencionadas como parte do stack para "sites de R$25.000"

---

## 🎯 Workflow Completo Ensinado

```
1. DESIGN NO FIGMA
   └── Criar o layout completo do site no Figma
   └── Definir tipografia, cores, espaçamentos, animações desejadas

2. CONECTAR FIGMA AO CLAUDE (via MCP)
   └── Configurar o MCP do Figma no VS Code
   └── Claude consegue "ver" o design em tempo real

3. GERAÇÃO DE CÓDIGO COM IA
   └── Prompts detalhados para Claude Code
   └── Claude gera HTML, CSS e JavaScript baseado no design
   └── Incluir instruções sobre animações desejadas

4. INTEGRAÇÃO DE ELEMENTOS 3D (Spline)
   └── Criar objetos 3D no Spline
   └── Exportar como embed para o site
   └── Integrar com as animações CSS/JS

5. OTIMIZAÇÃO DE PERFORMANCE
   └── Converter imagens para WebP
   └── Converter vídeos para WebM
   └── Comprimir vídeos com Handbrake
   └── Testar velocidade de carregamento
```

---

## ⚡ Boas Práticas de Performance (Dicas dos Comentários)

| Elemento | Formato Recomendado | Ferramenta |
|----------|--------------------|-----------:|
| Imagens  | **WebP**           | Squoosh, TinyPNG |
| Vídeos   | **WebM**           | Handbrake |
| Fontes   | WOFF2              | Google Fonts |
| Ícones   | SVG                | Feather Icons, Lucide |

- **WebP** carrega mais rápido que PNG/JPG e tem boa compatibilidade
- **WebM** é mais leve que MP4 e funciona melhor para vídeos de background
- **Handbrake** é a ferramenta gratuita recomendada para compressão de vídeo

---

## 📚 Recursos e Links

- **Comunidade WebHub:** https://gustavocampelo.com.br/comunidade-webhub/
- **Webinar Gratuito (toda terça 20h):** https://gustavocampelo.com.br/webinario-cadastro/
- **Hospedagem Hostinger** (cupom: `GUSTAVOCAMPELO`)
- **Spline 3D:** https://spline.design
- **Figma:** https://figma.com

---

## 💡 Principais Aprendizados

1. **IA como copiloto, não substituto** — o desenvolvedor ainda precisa saber o que quer e guiar a IA com bons prompts
2. **Figma MCP é o diferencial** — conectar design diretamente ao editor de código elimina re-trabalho
3. **Spline democratiza o 3D** — não é preciso saber Three.js para ter elementos 3D interativos
4. **Performance é obrigatória** — sites com animações pesadas precisam de mídia otimizada (WebP/WebM)
5. **Workflow iterativo** — design → código → ajuste → animação → otimização

---

## 🏷️ Tags
`sites-animados` `figma-mcp` `claude-code` `spline-3d` `frontend` `animacao-web` `ia-desenvolvimento` `webdesign` `performance-web` `webp` `webm`
