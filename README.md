<h2 align="center"> Termoo - Jogo de Adivinhação de Palavras </h2>

<h4 align="center"> Versão necessária Python>=3.6 </h4>
O Termoo é um jogo de adivinhação em que o jogador precisa descobrir uma palavra com um número específico de letras (5, 6 ou 7). 
A palavra começa com uma vogal determinada pelo jogador e é escolhida aleatoriamente entre várias listas de palavras.

<h4 align="center"> Regras: </h4>

O jogador escolhe o número de letras da palavra (5, 6 ou 7).
O jogador também escolhe a vogal inicial da palavra (A, E, I, O, U).
O objetivo é adivinhar a palavra em um número limitado de tentativas (máximo de 5 tentativas).
Ao tentar uma palavra, o sistema informa se alguma letra está correta e na posição certa (letra minúscula) ou se está na palavra,
mas na posição errada (letra maiúscula).
Se o jogador acertar a palavra, ele ganha! Se as tentativas acabarem, o jogo revela a palavra correta.

Exemplo de Interação:
O jogador escolhe uma palavra de 6 letras começando com a letra "a".
O sistema escolhe aleatoriamente a palavra "amparo".
O jogador tenta "amigo" e recebe a dica "a_m__".
O jogador tenta "amparo" e acerta!

---
<h4 align="center"> Objetivo: </h4>

Acertar a palavra antes de esgotar as tentativas!

Código Explicado:
O jogo começa com a explicação das regras.
O jogador escolhe a quantidade de letras da palavra (5, 6 ou 7) e a vogal inicial.
O código seleciona uma palavra aleatória da lista de palavras com base nas escolhas feitas pelo jogador.
O jogador tem até 5 tentativas para adivinhar a palavra.
Após cada tentativa, o código informa se o jogador acertou letras ou se acertou algumas letras, mas em posições erradas.
O jogo termina quando o jogador acerta a palavra ou esgota as tentativas.

Python e requirements.txt:
O código usa apenas bibliotecas padrão, sendo assim apenas é necessária a versão do Python dita no inicio.

---
<h4 align="center"> Para rodar o código no seu terminal, basta seguir as etapas abaixo: </h4>

Salve o código Python em um arquivo chamado, por exemplo, termoo.py

Crie o ambiente virtual (opcional, mas recomendado):

Se preferir, você pode criar um ambiente virtual para rodar o jogo sem afetar o sistema global de pacotes Python:

- python -m venv venv

Ative o ambiente virtual:
No Windows:
- venv\Scripts\activate

No Linux/macOS:
- source venv/bin/activate

Funcionamento:
Para rodar o jogo, execute o seguinte comando no terminal (onde o arquivo termoo.py está localizado):
<h5 align="center"> python termoo.py </h5>


---





---

<h2 align="center"> Termoo - Word Guessing Game </h2>

<h4 align="center"> Required Version Python >= 3.6 </h4>
Termoo is a word guessing game where the player must discover a word with a specific number of letters (5, 6, or 7).
The word starts with a vowel chosen by the player and is randomly selected from several word lists.

---
<h4 align="center"> Rules: </h4>
The player chooses the number of letters in the word (5, 6, or 7).
The player also chooses the starting vowel of the word (A, E, I, O, U).
The goal is to guess the word within a limited number of attempts (a maximum of 5).
After each attempt, the system informs the player if any letter is correct and in the right position (lowercase letter), or if the letter exists in the word but is in the wrong position (uppercase letter).
If the player guesses the correct word, they win! If all attempts are used up, the game reveals the correct word.

Example of Interaction:
The player chooses a 6-letter word starting with the letter “A.”
The system randomly selects the word “amparo.”
The player tries “amigo” and receives the hint “a_m__.”
The player then tries “amparo” and wins!

---
<h4 align="center"> Objective: </h4>
Guess the word before running out of attempts!

Code Explanation:
The game starts by explaining the rules.
The player chooses the number of letters (5, 6, or 7) and the initial vowel.
The code randomly selects a word from a predefined list based on the player's choices.
The player has up to 5 attempts to guess the word.
After each attempt, the program indicates whether letters are correct or misplaced.
The game ends when the player guesses the word or runs out of attempts.
Python and requirements.txt:
The code only uses standard Python libraries, so you only need the specified Python version to run the game.

---
<h4 align="center"> To run the code in your terminal, follow these steps: </h4>

Save the Python code in a file named, for example, termoo.py.

(Optional but recommended) Create a virtual environment to run the game without affecting global Python packages:

- python -m venv venv
Activate the virtual environment:

On Windows:
- venv\Scripts\activate

On Linux/macOS:
- source venv/bin/activate

Running the Game:
To start the game, run the following command in your terminal (in the same folder as termoo.py):

<h5 align="center"> python termoo.py </h5>

