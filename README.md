# Simulador Árvore-B remoção

Este projeto é um simulador interativo de **Árvores-B** com foco especial em **remoção com concatenação e redistribuição**, incluindo visualização quadro a quadro, destaques de operações críticas e representação gráfica em estilo *pixel art retro*.

O simulador foi desenvolvido em **HTML, CSS e JavaScript**, sem dependências externas, para fins educacionais — ideal para estudantes que precisam compreender passo a passo o funcionamento estrutural da árvore.

---
## ✨ Funcionalidades

### ✔️ Visualização Estruturada da Árvore-B
- Renderização em estilo pixel-art.
- Cada nó é mostrado com suas chaves separadas visualmente.
- Linhas conectam nós pais e filhos, facilitando entendimento da hierarquia.

### ✔️ Destaques Visuais de Eventos Críticos
O simulador marca automaticamente:
- **🔁 SPLIT** — divisão de nó durante inserção.
- **🔀 MERGE** — concatenação de nós durante remoção.
- Destaques coloridos e etiquetas aparecem nos nós afetados.

### ✔️ Passo a Passo Tipo “GIF” (Frame a Frame)
- Cada operação (inserção/remoção) gera uma **timeline de frames**.
- Controles: próximo, anterior, play/pause e reset.
- É possível acompanhar toda a operação em câmera lenta.

---
## 🎯 Objetivo Didático
O simulador permite:
- Entender Árvores-B sem depender de execução automática.
- Visualizar como o algoritmo manipula nós e chaves.
- Aprender operações fundamentais:
  - Inserção
  - Busca
  - Remoção (com concatenação e redistribuição)

---
## 📦 Conteúdos Implementados
- Construção de Árvore-B com grau mínimo `t = 2`.
- Inserção de lista inicial de **10 elementos não ordenados**.
- Geração automática do estado inicial.
- Simulação passo a passo da remoção, respeitando todas as regras:
  - Verificação prévia de filhos com menos de `t` chaves.
  - Redistribuição com irmãos.
  - Concatenação quando necessário.
  - Substituição por predecessor ou sucessor.

---
## 🧩 Estrutura do Projeto

O arquivo principal possui:
- Lógica completa de Árvores-B (classes + manipulação de nós).
- Sistema de timeline/frame.
- Interface gráfica + renderização dos nós.
- Destaques de split/merge com ícones.

O trecho final contém o sistema de renderização com SVG/linhas e destaques:
```js
renderTree(node, parentElement, highlightInfo)
```

---
## ▶️ Como Usar
1. Abra o arquivo HTML no navegador.
2. Clique em **Build** para gerar a árvore inicial.
3. Use os botões:
   - **Next / Prev** → navegar quadro a quadro.
   - **Play / Pause** → deixar animado.
   - **Reset** → reiniciar a simulação.
4. Realize inserções e remoções para visualizar mudanças.

---
## 📘 Requisitos Atendidos
Este projeto cumpre os seguintes requisitos solicitados:
- Representação animada estilo “GIF/slide”.
- Conjunto inicial de ≥10 dados não ordenados.
- Estado inicial mostrado corretamente.
- Transformações quadro a quadro durante operações.
- Destaque visual de momentos críticos (split/merge).
- Possível aprender o algoritmo apenas lendo/observando.

---
## 📌 Possíveis Extensões
Se quiser evoluir o projeto, posso adicionar:
- **Zoom e pan** da visualização.
- **Exportação de GIF real** dos frames.
- **Configuração de grau `t`** via interface.
- **Destaque animado (pulsante)** nos nós afetados.
- **Versão para Árvores B+ completa**.

---


Se quiser, posso gerar também uma versão em PDF ou DOCX deste README.

