# 🔥 Fire Doom Effect

Um projeto em **JavaScript** que recria o famoso **efeito de fogo do jogo Doom (1993)**, utilizando apenas **HTML, CSS e Canvas API**.  
Feito para praticar **estrutura de dados, algoritmos e renderização gráfica** em tempo real no navegador.

---

## 🚀 Demonstração

O código gera uma matriz de pixels que simulam chamas se movendo de baixo para cima, com base em uma paleta de cores que varia do preto ao branco, passando por tons de vermelho, laranja e amarelo como no efeito original do Doom.
[VEJA FUNCIONANDO!](https://jadsoncerqueira.github.io/fogo-dom/)

---

## 🧠 Conceitos praticados

- Estruturas de dados com **arrays bidimensionais**
- Manipulação de pixels via **Canvas API**
- **Algoritmos de propagação e decaimento**
- Atualização contínua com **`requestAnimationFrame()`**
- Uso de **paletas de cores indexadas**
- Renderização eficiente em **tempo real**

---

## 🧩 Estrutura do Projeto

```
📁 Fire-Doom
├── index.html
```

O arquivo `index.html` contém todo o código: estrutura HTML, estilos e o script principal.

---

## ⚙️ Como funciona

1. **Inicialização da estrutura de fogo**  
   Cria-se um array (`fireArray`) representando cada pixel da tela, inicialmente com valor `0` (sem fogo).

2. **Criação da fonte de fogo**  
   A última linha do array recebe o valor máximo (`36`), correspondente à cor mais quente da paleta.

3. **Propagação do fogo**  
   Cada pixel acima é atualizado com base no pixel logo abaixo, sofrendo um pequeno **decaimento aleatório**, o que cria o efeito de movimento das chamas.

4. **Renderização**  
   O canvas é redesenhado quadro a quadro, convertendo o valor de cada pixel em uma cor RGB da paleta `fireColorsPalette`.

---

## 🎨 Paleta de Cores

A paleta é composta por 37 níveis, indo do preto ao branco, simulando o gradiente de calor:

```js
const fireColorsPalette = [
  {"r":7,"g":7,"b":7},
  {"r":31,"g":7,"b":7},
  ...
  {"r":255,"g":255,"b":255}
]
```

---

## 🕹️ Tecnologias usadas

- **HTML5**
- **CSS3**
- **JavaScript Puro (Vanilla JS)**
- **Canvas API**

---

## 💡 Aprendizados

Durante o desenvolvimento, pratiquei:

- Lógica de **simulação visual com base em dados**
- Uso de **arrays unidimensionais** para simular grids 2D
- Controle de **taxa de atualização de frames**
- Conceitos de **decay**, **propagação** e **gradiente de cores**

---

## 🧰 Melhorias futuras

- Controlar intensidade e velocidade das chamas
- Adicionar gradiente dinâmico de cores
- Permitir interação com o mouse (ex: soprar o fogo 😄)
- Converter para **TypeScript** ou **React Canvas**

---

## 🧑‍💻 Autor

**Jadson Cerqueira**  
Desenvolvedor Full Stack  
[LinkedIn](https://www.linkedin.com/in/jadsoncerqueira/) | [GitHub](https://github.com/jadsoncerqueira)

---

## 📜 Licença

Este projeto é de código aberto e pode ser usado livremente para fins de estudo e experimentação.

---

🔥 *“O fogo do Doom nunca apaga — ele só é otimizado frame a frame.”*
