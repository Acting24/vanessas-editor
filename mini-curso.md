# 🎓 Mini Curso:

Bem-vindo! Este curso foi desenhado para transformar você de iniciante a **power user** em 6 módulos progressivos. Cada módulo leva de 10 a 20 minutos. Recomendo **digitar tudo manualmente** (não copie e cole) para treinar memória muscular.

---

## 📋 Antes de Começar

Abra o editor e clique no botão **❓ Ajuda** (ou pressione `F1`) para ter o guia de atalhos sempre à mão.

---

## 🟢 MÓDULO 1 — Primeiros Passos (10 min)

**Objetivo:** Familiarizar-se com a interface e salvar seu primeiro arquivo.

### Passo 1.1 — Limpe o editor
Clique no campo de texto à esquerda e pressione `Ctrl + A` (selecionar tudo) e depois `Delete` para limpar.

### Passo 1.2 — Dê um nome ao arquivo
No canto superior direito, no campo "Arquivo:", digite:
```
meu_primeiro_documento
```

### Passo 1.3 — Digite seu primeiro conteúdo
No editor, digite exatamente isto (respeitando as quebras de linha):

```markdown
# Meu Primeiro Documento

Olá! Este é meu primeiro arquivo criado no NeonDownright.

## Sobre mim
- Nome: [Seu nome aqui]
- Curso: Álgebra Linear
- Data: 11/11/2026
```

### Passo 1.4 — Observe a mágica
Olhe para o painel da **direita**. Você verá o texto renderizado com:
- Título grande e colorido em neon
- Subtítulo com linha decorativa
- Lista com marcadores

### Passo 1.5 — Salve o arquivo
Pressione `Ctrl + S` ou clique em **💾 Salvar .md**. Um arquivo chamado `meu_primeiro_documento.md` será baixado.

✅ **Desafio do Módulo 1:** Feche o editor, abra o arquivo `.md` baixado em um editor de texto simples (Bloco de Notas) e veja o código Markdown puro.

---

## 🟡 MÓDULO 2 — Markdown Essencial (20 min)

**Objetivo:** Dominar a formatação de texto profissional.

### Passo 2.1 — Limpe o editor e digite:

```markdown
# Guia de Markdown

## Formatação de Texto

Este é um texto em **negrito** e este em *itálico*.
Também posso combinar ***negrito e itálico***.
E usar `código inline` para destacar comandos.

## Listas

### Lista não ordenada
- Vetores
- Matrizes
- Determinantes

### Lista ordenada
1. Primeiro conceito
2. Segundo conceito
3. Terceiro conceito

## Citações

> "A matemática é a rainha das ciências."
> — Carl Friedrich Gauss

## Tabelas

| Operação | Notação | Propriedade |
|----------|---------|-------------|
| Soma     | A + B   | Comutativa  |
| Produto  | A · B   | Associativa |
```

### Passo 2.2 — Experimente as variações
Adicione ao final do documento:

```markdown
## Links e Imagens

Visite o [GitHub](https://github.com) para mais projetos.

## Checklists (Tarefas)

- [x] Instalar o editor
- [x] Aprender Markdown básico
- [ ] Dominar LaTeX
- [ ] Criar gráficos interativos
```

✅ **Desafio do Módulo 2:** Crie uma tabela com 4 linhas e 3 colunas sobre "Tipos de Matrizes" (Identidade, Nula, Transposta, Inversa).

---

## 🟠 MÓDULO 3 — LaTeX para Matemática (25 min)

**Objetivo:** Escrever fórmulas matemáticas profissionais.

### Passo 3.1 — Limpe e digite:

```markdown
# Fórmulas de Álgebra Linear

## Equações Inline

A equação da reta é $y = mx + b$, onde $m$ é o coeficiente angular.

## Equações em Bloco (centralizadas)

A fórmula de Bhaskara:

$$
x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}
$$

## Matrizes

### Matriz 2x2

$$
A = \begin{pmatrix} 1 & 2 \\ 3 & 4 \end{pmatrix}
$$

### Matriz Identidade 3x3

$$
I_3 = \begin{bmatrix} 1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 1 \end{bmatrix}
$$

## Somatórios e Integrais

$$
\sum_{i=1}^{n} i = \frac{n(n+1)}{2}
$$

$$
\int_{0}^{1} x^2 \, dx = \frac{1}{3}
$$
```

### Passo 3.2 — Use o botão ▦ Matriz
Clique no botão **▦ Matriz** na barra superior. Quando pedir:
- Linhas: `2`
- Colunas: `3`
- Tipo: `bmatrix`

Uma matriz será inserida automaticamente no cursor.

✅ **Desafio do Módulo 3:** Escreva a definição de determinante de uma matriz 2x2 usando LaTeX:
$$\det(A) = ad - bc$$

---

## 🔴 MÓDULO 4 — Gráficos Interativos (25 min)

**Objetivo:** Criar visualizações de funções matemáticas com JSON.

### Passo 4.1 — Limpe e digite:

```markdown
# Gráficos de Funções

## Função Quadrática

```graph
{
  "xAxis": {"domain": [-5, 5]},
  "yAxis": {"domain": [-2, 10]},
  "title": "f(x) = x²",
  "data": [
    {"fn": "x^2", "color": "#00f3ff"}
  ]
}
```

## Funções Trigonométricas

```graph
{
  "xAxis": {"domain": [-6.28, 6.28]},
  "yAxis": {"domain": [-1.5, 1.5]},
  "title": "Seno e Cosseno",
  "data": [
    {"fn": "sin(x)", "color": "#00f3ff"},
    {"fn": "cos(x)", "color": "#ff00ff"}
  ]
}
```
```

### Passo 4.2 — Entenda a estrutura JSON
Cada gráfico tem:
- `xAxis.domain`: intervalo do eixo X `[min, max]`
- `yAxis.domain`: intervalo do eixo Y `[min, max]`
- `title`: título do gráfico
- `data`: array de funções com `fn` (fórmula) e `color` (cor)

### Passo 4.3 — Funções disponíveis
Você pode usar: `sin`, `cos`, `tan`, `sqrt`, `abs`, `log`, `exp`, `pi`, `e`, e o operador `^` para potência.

✅ **Desafio do Módulo 4:** Crie um gráfico com 3 funções:
1. $f(x) = \sin(x)$ em ciano (`#00f3ff`)
2. $g(x) = \cos(x)$ em rosa (`#ff00ff`)
3. $h(x) = \sin(x) \cdot \cos(x)$ em verde (`#0aff00`)

Dica: no JSON, use `"fn": "sin(x) * cos(x)"`.

---

## 🟣 MÓDULO 5 — Modo Vim (30 min)

**Objetivo:** Editar texto sem usar o mouse.

### Passo 5.1 — Ative o Modo Vim
Clique no botão **⌨️ Modo Vim**. Você verá `[ NORMAL ]` aparecer no canto inferior direito.

### Passo 5.2 — Navegação básica
Digite este texto:
```
Linha 1: Aprendendo Vim
Linha 2: Navegação com hjkl
Linha 3: h = esquerda, l = direita
Linha 4: j = baixo, k = cima
```

Agora, **sem usar o mouse ou setas**, pressione:
- `h` várias vezes (vai para esquerda)
- `l` várias vezes (vai para direita)
- `j` (desce uma linha)
- `k` (sobe uma linha)

### Passo 5.3 — Modos de edição
- Pressione `i` → entra no modo `INSERT` (cursor vira linha)
- Digite algo
- Pressione `Esc` → volta ao modo `NORMAL` (cursor vira bloco)

### Passo 5.4 — Operações em linhas
Posicione o cursor na "Linha 2" e:
- Digite `dd` → a linha é deletada
- Pressione `p` → a linha é colada abaixo
- Digite `yy` → a linha é copiada
- Pressione `p` novamente → a linha é duplicada

### Passo 5.5 — Desfazer e refazer
- Pressione `u` → desfaz a última ação
- Pressione `Ctrl + r` → refaz

✅ **Desafio do Módulo 5:** Escreva 5 linhas sobre "Vetores". Use `dd` para apagar a linha 3, `yy` + `p` para duplicar a linha 1, e `u` para desfazer. Tudo sem tocar no mouse!

---

## ⚫ MÓDULO 6 — Workflow Profissional (20 min)

**Objetivo:** Criar um documento completo e exportá-lo.

### Passo 6.1 — Crie um documento final
Limpe o editor e crie um resumo completo sobre um tema de Álgebra Linear. Use TUDO que aprendeu:

```markdown
# Resumo: Espaços Vetoriais

## Definição
Um **espaço vetorial** $V$ sobre um corpo $\mathbb{R}$ é um conjunto com duas operações.

## Axiomas Fundamentais

$$
\vec{u} + \vec{v} = \vec{v} + \vec{u} \quad \text{(Comutatividade)}
$$

## Exemplo: $\mathbb{R}^2$

O espaço $\mathbb{R}^2$ pode ser representado pela matriz:

$$
\begin{bmatrix} x \\ y \end{bmatrix}
$$

## Visualização

```graph
{
  "xAxis": {"domain": [-5, 5]},
  "yAxis": {"domain": [-5, 5]},
  "title": "Vetor no R²",
  "data": [
    {"fn": "x", "color": "#00f3ff"},
    {"fn": "-x", "color": "#ff00ff"}
  ]
}
```

## Tarefas de Estudo

- [x] Entender definição
- [x] Estudar exemplos
- [ ] Resolver exercícios
- [ ] Revisar antes da prova
```

### Passo 6.2 — Exporte em 3 formatos
1. **💾 Salvar .md** → para editar depois
2. **🌐 Exportar .html** → para compartilhar como página web
3. **🖨️ PDF** → para imprimir ou enviar como documento formal

### Passo 6.3 — Teste o Drag & Drop
Arraste o arquivo `.md` que você acabou de salvar de volta para o editor. Ele será recarregado automaticamente!

✅ **Desafio Final:** Exporte seu documento como HTML, abra o arquivo no navegador e envie para um amigo. Ele verá um documento profissional com fórmulas matemáticas renderizadas!

---

## 🏆 Certificado de Conclusão

Ao completar os 6 módulos, você desenvolveu:

| Habilidade | Nível |
|------------|-------|
| Markdown | ⭐⭐⭐⭐⭐ |
| LaTeX / Matemática | ⭐⭐⭐⭐ |
| Visualização de Dados | ⭐⭐⭐⭐ |
| Edição Eficiente (Vim) | ⭐⭐⭐ |
| Exportação Profissional | ⭐⭐⭐⭐⭐ |

---

## 📚 Próximos Passos

1. **Pratique diariamente:** Use o editor para suas anotações de estudo.
2. **Explore o código:** Abra o arquivo HTML do editor em um editor de código e tente modificar uma cor ou adicionar um botão.
3. **Crie templates:** Salve documentos modelo que você reutiliza frequentemente.
4. **Compartilhe:** Exporte seus resumos em HTML e compartilhe com colegas.

**Lembre-se:** A maestria vem da prática consistente. 15 minutos por dia usando o editor valem mais que 3 horas uma vez por semana. 🚀

Bom estudo!