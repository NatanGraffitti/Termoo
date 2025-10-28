# Termoo - Jogo de Adivinhação de Palavras 

O Termoo é um jogo de adivinhação em que o jogador precisa descobrir uma palavra com um número específico de letras (5, 6 ou 7). 
A palavra começa com uma vogal determinada pelo jogador e é escolhida aleatoriamente entre várias listas de palavras.

Regras:

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

# Objetivo: 
Acertar a palavra antes de esgotar as tentativas!

Versão necessária:
Python>=3.6

1. Código Explicado:

O jogo começa com a explicação das regras.
O jogador escolhe a quantidade de letras da palavra (5, 6 ou 7) e a vogal inicial.
O código seleciona uma palavra aleatória da lista de palavras com base nas escolhas feitas pelo jogador.
O jogador tem até 5 tentativas para adivinhar a palavra.
Após cada tentativa, o código informa se o jogador acertou letras ou se acertou algumas letras, mas em posições erradas.
O jogo termina quando o jogador acerta a palavra ou esgota as tentativas.

2. Python e requirements.txt:

O código usa apenas bibliotecas padrão, sendo assim apenas é necessária a versão do Python dita no inicio.

3. Como rodar o código:

# Para rodar o código no seu terminal, basta seguir as etapas abaixo:
- Salve o código Python em um arquivo chamado, por exemplo, termoo.py
Crie o ambiente virtual (opcional, mas recomendado):
Se preferir, você pode criar um ambiente virtual para rodar o jogo sem afetar o sistema global de pacotes Python:
- python -m venv venv
Ative o ambiente virtual:
No Windows:
- venv\Scripts\activate

No Linux/macOS:
- source venv/bin/activate

Rodar o código:
Para rodar o jogo, execute o seguinte comando no terminal (onde o arquivo termoo.py está localizado):
- python termoo.py


