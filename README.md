# 🐢 Project: Tartaruga Inteligente

Este é um motor de jogo 2D desenvolvido em **Python** utilizando o módulo **Turtle Graphics**. O projeto foi estruturado seguindo princípios de **Orientação a Objetos (POO)** para garantir modularidade e facilidade de manutenção.

---

## 🏗️ Arquitetura do Sistema

O software é dividido em componentes independentes que se comunicam no loop principal:

* **`main.py`**: O *entry point* da aplicação. Gerencia o loop de renderização, a detecção de colisões e a lógica de estado do jogo (Game Over).
* **`jogador.py`**: Classe `Jogador`. Controla a lógica de posicionamento e movimentação lateral do avatar no eixo $X$.
* **`carro.py`**: Motor de geração de obstáculos. Utiliza listas para gerenciar múltiplos objetos `Turtle` simultaneamente e controla o fluxo de spawn baseado na posição do último veículo.
* **`pista.py`**: Responsável pela renderização estática do cenário e faixas de rodagem utilizando iterações (`for loops`).
* **`pontuacao.py`**: Gerenciador de interface (UI) que atualiza o score em tempo real conforme os obstáculos são superados.

---

## 🛠️ Especificações Técnicas

* **Linguagem:** Python 3.x.
* **Biblioteca Gráfica:** `turtle`.
* **Módulos Nativos:** `time` (controle de FPS) e `random` (geração de aleatoriedade).
* **Input:** Mapeamento de teclas `Left` e `Right` via `Screen().listen()`.

---

## 🚀 Como Executar

### Em ambiente Local
1. Certifique-se de ter o Python instalado em sua máquina.
2. Mantenha todos os arquivos `.py` no mesmo diretório.
3. Execute o comando:
   ```bash
   python main.py
