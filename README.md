
# **Tic-Tac-Toe-Solver_202401100300045**  

## **Overview**  
This repository contains an AI-powered **Tic-Tac-Toe Solver** that uses the **Minimax Algorithm with Alpha-Beta Pruning** to make optimal moves. The AI ensures that it either wins the game or forces a draw.  

## **Features**  
✅ Implements **Minimax Algorithm** for strategic decision-making  
✅ Uses **Alpha-Beta Pruning** to enhance efficiency  
✅ Human vs. AI gameplay on a **3x3 Tic-Tac-Toe board**  
✅ Written in **Python** and executed on **Google Colab**  

## **How It Works**  
1. The Tic-Tac-Toe board is represented as a 3x3 matrix.  
2. The AI evaluates all possible moves using the **Minimax Algorithm**.  
3. **Alpha-Beta Pruning** optimizes the decision-making process by reducing unnecessary computations.  
4. The AI selects the best possible move and plays optimally.  

## **Installation & Usage**  
### **Requirements**  
- Python 3.x  
- NumPy (for matrix operations)  
- Google Colab (recommended for execution)  

### **Steps to Run**  
1. Clone the repository:  
   ```bash
   git clone https://github.com/your-repo/Tic-Tac-Toe-Solver_202401100300045.git
   ```
2. Open the `.ipynb` file in **Google Colab** or Jupyter Notebook.  
3. Run the script to start the game.  
4. The AI will analyze the board and make optimal moves.  

## **Code Snippet**  
```python
def find_best_move(board):
    best_val = -1000
    best_move = (-1, -1)
    for i in range(3):
        for j in range(3):
            if board[i][j] == ' ':
                board[i][j] = 'X'
                move_val = minimax(board, 0, False)
                board[i][j] = ' '
                if move_val > best_val:
                    best_move = (i, j)
                    best_val = move_val
    return best_move
```

## **Output Example**  
- AI analyzing moves  
- AI making an optimal move  
- Displaying the updated board  

(Screenshot of execution in Google Colab)  

## **Files in this Repository**  
📂 `Tic-Tac-Toe-Solver_202401100300045.ipynb` → Jupyter Notebook containing the code  
📂 `README.md` → This file with project details  
📂 `report.pdf` → Detailed project report (as per submission guidelines)  

## **References & Credits**  
- **Minimax Algorithm**: Game Theory for AI  
- **Alpha-Beta Pruning**: Optimization Technique  
- **Python AI Implementation in Tic-Tac-Toe**  

---

