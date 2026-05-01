# ⚙️ O Motor: Bibliotecas de Animação Front-end

> Documentação técnica das bibliotecas necessárias para criar o "Efeito R$ 25.000" no código. Baseado na curadoria de tutoriais (GSAP, Framer Motion, R3F, Lenis).

Para transformar a **Dramaturgia Visual** em código funcional sem destruir a performance (PageSpeed), o Antigravity utiliza o seguinte ecossistema de animação, escolhido a dedo dependendo da necessidade do projeto:

---

## 1. Lenis (Smooth Scroll)
A fundação de todo site premium. O scroll nativo do navegador é "seco" e varia entre mouses e trackpads.
- **O que faz:** Intercepta o scroll nativo e aplica física (easing, inércia), criando o famoso "efeito deslizante da Apple".
- **Quando usar:** Em **100% dos projetos premium**.
- **Vantagem:** É extremamente leve e feito para trabalhar perfeitamente em conjunto com o GSAP ScrollTrigger.

## 2. GSAP (GreenSock) + ScrollTrigger
O padrão ouro da indústria para animações baseadas no scroll e linhas do tempo complexas.
- **O que faz:** Controla propriedades CSS, SVG e Canvas com precisão cirúrgica. O plugin `ScrollTrigger` permite atrelar a linha do tempo da animação à posição da barra de rolagem.
- **Quando usar:** Para a narrativa de scroll principal (ex: seções pinadas que ficam presas na tela enquanto o texto sobe, imagens que dão zoom on-scroll).
- **Vantagem:** Performance absurda. É a biblioteca usada pelos sites premiados no Awwwards.

## 3. Framer Motion
A melhor biblioteca para o ecossistema React/Next.js.
- **O que faz:** Animações declarativas diretamente nos componentes React. 
- **Quando usar:** Micro-interações (hover, tap), animações de montagem da tela inicial (mount/unmount) e transições entre páginas.
- **Vantagem:** Sintaxe absurdamente simples (`<motion.div>`) e gerenciamento automático de desmontagem de componentes no React (AnimatePresence).

## 4. React Three Fiber (R3F) & Three.js
O passo além do Spline. Para quando o 3D precisa interagir matematicamente com a página.
- **Exemplo de uso (Wawa Sensei - Atmos 3D):** Fazer um modelo 3D navegar por um "Caminho Curvo" (`CatmullRomCurve3`) baseado no scroll do usuário, alterando a rotação para olhar sempre para frente.
- **Quando usar:** Quando o 3D não é apenas um fundo decorativo, mas a própria interface (pontículas interativas, shaders customizados, objetos que reagem à luz e ao mouse nativamente).
- **Bibliotecas auxiliares:** `Drei` (helpers) e `Lamina` (shaders fáceis).

## 5. CSS Nativo / Vanilla JS
Muitos Shorts enviados focam nisso: a melhor biblioteca às vezes é não usar nenhuma.
- **O que faz:** Animações simples usando `transition`, `keyframes` ou `IntersectionObserver`.
- **Quando usar:** Quando a performance for crítica (mobile) ou para efeitos extremamente simples (fade-in ao entrar na tela).

---

## 🛠️ O Stack do Motor (Como combiná-las)

A stack definitiva do Antigravity para um projeto Next.js animado será:

1. **Next.js** (Framework)
2. **Tailwind CSS** (Estilização base)
3. **Lenis** (Para o Smooth Scroll global)
4. **Framer Motion** (Para micro-interações nos botões e cards)
5. **GSAP ScrollTrigger** (Para a grande narrativa de scroll e Efeito Parallax)
6. **R3F** (Apenas se o projeto exigir 3D renderizado via código)
