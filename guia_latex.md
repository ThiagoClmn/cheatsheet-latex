# Apostila express de $\LaTeX$
---

# Introdução
- Use `$` no inicio e fim para escrever uma expressão na linha
> A função quadrática é `$y = x^2$`
> A função quadrática é $y = x^2$

- Use `$$` no inicio e fim para escrever uma expressão na linha abaixo centralizada
> A função quadrática é `$$y = x^2$$`
> A função quadrática é $$y = x^2$$

___Devo falar disso?_
Listas numeradas e não numeradas
Inserção de tabelas
Inserção de figuras
Divisão em capítulos e seções__

# Simbologia matemática
- Potência e índices sobrescritos
Use o circunflexo (`^`) e para expoentes:
    - Com um caractere: `r^2`, $r^2$
    - Com mais caracteres: `r^{abc}`, $r^{abc}$
    O uso das chaves para expoentes de um caractere é opcional. Caso contrário, é obrigatório
- Índices subescritos
Use o underscore (`_`)
    - Exemplo da fórmula de P.A.
        - `a_n = a_1 + r(n - 1)`
        - $a_n = a_1 + r(n - 1)$
    - Segunda lei de Newton
        - `F_{res} = ma`
        - $F_{res} = ma$
A regra do uso de chaves em exponenciação também é válida

- Frações
    - Comando `\dfrac{}{}`
    - Exemplo
        - `$\dfrac{ab}{2^x}$`
        - $\dfrac{ab}{2^x}$

**OBS.:** Ao escrever grandes expressões em fração, o interpretador a altura da linha à expressão, deixando-a espremida. Caso seja necessária adequar a altura da linha ao tamanho da expressão use `\left` e `\right` da seguinte forma:
`\left(    [Código LaTeX]    \right)`

Exemplo
`$$\left(\dfrac{7^{\ln 2}}{\exp(\dfrac{-T}{\log5})}\right)$$`
$$\left(\dfrac{7^{\ln 2}}{\exp(\dfrac{-T}{\log5})}\right)$$

# Conjuntos
Sejam _A_ e _B_ dois conjuntos e _U_ conjunto universo
- União 
    - `$A \cup B$` ; $A \cup B$
- Interseção
    - `$A \cap B$` ; $A \cap B$
- Complementar
    - `$A^c = U - A$` ; $A^c = U - A$
- Conjuntos numéricos
    - Naturais `\mathbb{N}` $\mathbb{N}$
    - Inteiros `\mathbb{Z}` $\mathbb{Z}$
    - Racionais `\mathbb{Q}` $\mathbb{Q}$
    - Reais `\mathbb{R}` $\mathbb{R}$
    - Complexos `\mathbb{C}` $\mathbb{C}$

# Cálculo

- Limite
    - ...
- Derivada
    - Notação de Lagrange
        - `$f'(x)$`
        - $f'(x)$
    - Notação de Leibniz
        - `$\left(\dfrac{df}{dx}\right)$`
        - $\left(\dfrac{df}{dx}\right)$
    - Derivada parcial
        - Símbolo $\partial$: `$\partial$`
        - `$\left(\dfrac{\partial f}{\partial x}\right)$`: $\left(\dfrac{\partial f}{\partial x}\right)$
        - `$\left(\dfrac{\partial^2 f}{\partial x^2}\right)$`: $\left(\dfrac{\partial^2 f}{\partial x^2}\right)$

- Integral
    - ...


# Geometria Analítica e Álgebra Linear
- Símbolo de vetor (`\vec{}`)
Exemplo: `\vec{u} = \vec{0}`, $\vec{u} = \vec{0}$

- Produto interno: `\vec{a} \cdot \vec{b}` $\vec{a} \cdot \vec{b}$
- Produto vetorial: `\vec{a} \times \vec{b}` $\vec{a} \times \vec{b}$

# Matriz

- Escrever os elementos da matriz entre `&` e pular linha com `\\`

- Matriz com colchetes: `bmatrix` (`\begin{bmatrix} ... \end{bmatrix}`)

`$$ A = \begin{bmatrix} 1 & 2\\ 0 & 7 \end{bmatrix} $$`

$$A = \begin{bmatrix} 1 & 2\\0 & 7 \end{bmatrix}$$

- Matriz com parênteses: `pmatrix` (`\begin{pmatrix} ... \end{pmatrix}`)

`$$
A = \begin{pmatrix}
1 & 2 \\ 0 & 7
\end{pmatrix} $$`

$$ A = \begin{pmatrix}
1 & 2 \\ 0 & 7
\end{pmatrix} $$

- Matriz com barra vertical simples: `vmatrix` (`\begin{vmatrix} ... \end{vmatrix}`)
    - Determinante (`$\det$`)

`\det A = \begin{vmatrix} 1 & 2\\0 & 7 \end{vmatrix} `

$$ \det A = \begin{vmatrix}
1 & 2\\0 & 7
\end{vmatrix} $$


# Letras Gregas

|Letra | Símbolo |
|------|-------- |
Alfa `\alfa` | $\alpha$
Beta `\beta` | $\beta$
Gama `\gama` | $\gamma$
Delta `\delta` | $\delta$
Epsilon `\epsilon` | $\epsilon$
Zeta `\zeta` | $\zeta$
Eta `\eta` | $\eta$
Theta `\theta` | $\theta$
Iota `\iota` | $\iota$
Kappa `\kappa` | $\kappa$
Lambda `\lambda` | $\lambda$
Mu `\mu` | $\mu$
Nu `\nu` | $\nu$
Xi `\xi` | $\xi$
Omicron `\omicron` | $\omicron$
Pi `\pi` | $\pi$
Rho `\rho` | $\rho$
Sigma `\sigma` | $\sigma$
Tau `\tau` | $\tau$
Upsilon `\upsilon` | $\upsilon$
Phi `\phi` | $\phi$
Chi `\chi` | $\chi$
Psi `\psi` | $\psi$
Omega `\omega` | $\omega$

Para usar a versão maiúscula, basta escrever o comando com letra maiúscula

_Exemplos:_

| Letra  | Símbolo |
|------  |-------- |
|`\delta`| $\delta$|
|`\Delta`| $\Delta$|
|`\omega`| $\omega$|
|`\Omega`| $\Omega$|


# Uso de fontes
Existem duas formas de manipular o tamanho e tipo de fonte do documento $\LaTeX$
- Afetando o documento todo
- Afetando uma parte do documento

## Mudanças gerais
Para estabelecer um tipo de fonte e tamanho padrão para todo o documento, isso é feito no preâmbulo, isto é, a parte de configurações do documento, ela vêm antes mesmo do corpo do texto propriamente dito

`\documentclass[12pt]{report}`

## Mudanças locais
OBS.: Uso do `\small` ou `\Small` e `\large` ou `\Large`
|Comandos|
|--|
|`\Huge`|
|`\huge`|
|`\LARGE`|
|`\Large`|
|`\large`|
|`\normalsize` (padrão)|
|`\small`|
|`\footnotesize` (rodapé)|
|`\scriptsize`|
|`\tiny`|

Um guia (em inglês) com todos os tamanhos de fonte disponíveis pode ser encontrado [aqui](https://en.wikibooks.org/wiki/LaTeX/Text_Formatting#Sizing_text)

| Comando | Resultado|
|----|----|
|`{\Huge Texto}` | ${\Huge Texto}$
|`{\huge Texto}` | ${\huge Texto}$
|`{\LARGE Texto}` | ${\LARGE Texto}$
|`{\Large Texto}` | ${\Large Texto}$
|`{\large Texto}` | ${\large Texto}$
|`{\normalsize Texto}` | ${\normalsize Texto}$
|`{\small Texto}` | ${\small Texto}$
|`{\footnotesize Texto }`| ${\footnotesize Texto}$
|`{\scriptsize Texto }`| ${\scriptsize Texto}$
|`{\tiny Texto}` | ${\tiny Texto}$

# **Bônus** :star:
## Links de compiladores de $\LaTeX$

* Overleaf [:leaves: Homepage](https://www.overleaf.com/)
* Notion: recurso de escrita no bloco `code`
* [$\LaTeX$ equation editor](https://latexeditor.lagrida.com/)
* [$\LaTeX$ codecogs](https://latex.codecogs.com/eqneditor/editor.php)

## Referências e fontes de estudo
Santos, Reginaldo J.. Introdução ao LaTeX. Departamento de Matemática-ICEx. Universidade Federal de Minas Gerais. 2002.
Disponível [aqui](https://regijs.github.io/apostilas.html)

Oetiker, Tobias; Partl, Hubert; Hyna, Irene; Schlegl, Elisabeth. Introdução ao LaTeX 2e - Ou LaTeX 2e em 105 minutos. Departamento de Engenharia Elétrica, Instituto Federal Suíço de Tecnologia. 2001.
Disponível [aqui](https://www.ime.usp.br/~polli/pdf/lshortBR-4.14.zip)
