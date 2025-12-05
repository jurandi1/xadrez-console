# ♟️ Xadrez em C# — Console Chess Game

Um jogo completo de **Xadrez desenvolvido em C#**, executado no console e construído do zero para fins didáticos e prática da linguagem.

Este projeto implementa **todas as regras oficiais do xadrez**, incluindo roque, promoção, en passant, capturas, verificação de xeque e xequemate, movimentação válida e controle de turnos.

---


![xadrez_demo](https://github.com/user-attachments/assets/1610a9b6-1776-4168-85af-f259f58de21d)


## 📌 Funcionalidades

### ✔️ Regras implementadas
- Movimentação de todas as peças  
- Controle de movimentos válidos  
- Capturas de peças  
- Exibição das posições possíveis no tabuleiro  
- Detecção de **xeque**  
- Detecção de **xequemate**  
- Tratamento de erros com exceções personalizadas  
- Colocação inicial das peças conforme regras oficiais  
- Jogada especial **Roque pequeno e grande**  
- Jogada especial **En Passant**  
- Jogada especial **Promoção de Peão**  

---

## 🎮 Como jogar

Ao iniciar o programa, você verá o tabuleiro e o status da partida:

1. Digite a **posição de origem** da peça (ex: `e2`).  
2. O programa destacará todos os **movimentos possíveis**.  
3. Digite a **posição de destino** (ex: `e4`).  
4. O jogo executa a jogada e alterna o turno automaticamente.  

Caso uma jogada seja inválida, o programa exibirá uma mensagem explicativa.

---

## 🧠 Estrutura do projeto

O jogo foi construído com uma arquitetura modular para garantir clareza e fácil manutenção:
```
📁 xadrez-console
├── Program.cs
├── tela/
| └── Tela.cs
├── tabuleiro/
| ├── Tabuleiro.cs
| ├── Posicao.cs
| ├── Peca.cs
| └── TabuleiroException.cs
└── xadrez/
├── PartidaDeXadrez.cs
├── Rei.cs
├── Dama.cs
├── Torre.cs
├── Bispo.cs
├── Cavalo.cs
└── Peao.cs
```
---

## 🚀 Execução

### **Requisitos**
- .NET 6 ou superior  
- Windows, Linux ou macOS  
- Terminal habilitado para UTF-8  

### **Rodando o projeto**
```bash
git clone https://github.com/jurandi1/xadrez-console.git
cd xadrez-console
dotnet run
