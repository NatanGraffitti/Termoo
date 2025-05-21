import random
import unicodedata

#listas com a letra A        
lista_palavras_a5 = ["amigo", "andar", "antes", "arroz", "anexo", "altar", "abrir", "amplo", "aceno", "apito", "acima", "aviso", "aliar", "astro", "agua", "ardor", "areia", "autos", "acres", "assar"]
lista_palavras_a6 = ["amavel", "amparo", "apagar", "abrigo", "alento", "abismo", "aliado", "andar", "atento", "arruar", "argola", "alegre", "armado", "aviao", "abrir", "anelar", "atirar", "aceita", "almoço"]
lista_palavras_a7 = ["amarelo", "abrigar", "amassar", "alegria", "andarao", "atuante", "aliados", "aumento", "ansioso", "ameaças", "apontar", "abrange", "armados", "abertos", "alugado", "avançar", "aviador", "aflitos", "assinar", "alugara"]
#listas com a letra E        
lista_palavras_e5 = ["estar", "entra", "exato", "etapa", "elite", "exame", "enche", "errar", "eixos", "ecoar", "expor", "exige", "etnia", "enfim", "epico", "extra", "edema", "exito", "ervas", "egito"]
lista_palavras_e6 = ["esquema", "enlace", "empate", "ensino", "enviar", "estrela", "elevar", "esfera", "entrar", "emenda", "encher", "exigir", "espera", "editar", "exalar", "errado", "esgoto", "estilo", "exibir", "elegir"]
lista_palavras_e7 = ["escrever", "entrada", "ensinar", "enxugar", "esforço", "errante", "enxoval", "enfeite", "eleitor", "emprego", "excesso", "eleiçao", "encontro", "elegido", "emitido", "estudar", "enchera", "engajar", "espelho", "estimar"]
#listas com a letra I        
lista_palavras_i5 = ["ideia", "idolo", "ileso", "impor", "infra", "indio", "inato", "idoso", "imune", "intua", "insta", "isola", "igual", "irado", "impio", "inicio", "intra", "iris", "item", "imune"]
lista_palavras_i6 = ["ideias", "inicio", "idolos", "infame", "irmaos", "imovel", "inveja", "imensa", "impeto", "iguala", "imitar", "isento", "intuir", "idiota", "isolar", "ignora", "iludir", "insumo", "imundo"]
lista_palavras_i7 = ["idiomas", "iniciar", "inverno", "ilusao", "imagina", "impressa", "inedito", "imagens", "invadir", "igualar", "idadear", "irmaos", "imuniza", "ignorar", "ilustre", "invejar", "infeliz", "incitar", "impostos", "insumos"]
#listas com a letra O        
lista_palavras_o5 = ["olhos", "obter", "ordem", "ondas", "outro", "obvio", "ossos", "opaco", "orçar", "ouvir", "ostra", "oxida", "opera", "outra", "orgao", "otimo", "onças", "ofere", "olhar", "orbes"]
lista_palavras_o6 = ["observar", "oferta", "olhado", "orgulho", "ouvido", "outras", "obrigar", "opcoes", "olhara", "opuser", "ombros", "ornato", "orques", "oficio", "obtido", "ousado", "ondas", "oposto", "obstaculo", "otario"]
lista_palavras_o7 = ["objetos", "ocultar", "olhares", "ofertas", "obtiver", "oficial", "ouvidos", "orgulho", "oscilou", "ostenta", "oponham", "ouvinte", "orvalho", "obrigar", "omelete", "orienta", "obrador", "obstina", "odiaram", "oxigena"]
#listas com a letra U        
lista_palavras_u5 = ["unido", "unico", "usina", "urina", "uvaso", "ultra", "usado", "urgir", "urros", "usura", "ungir", "urubu", "ufano", "umido", "ubere", "unhas", "urban", "usura", "uteis", "ursos"]
lista_palavras_u6 = ["uganda", "urgente", "unidos", "usinas", "utopia", "urgida", "urinar", "usavel", "urros", "uivado", "usando", "unidas", "umbigo", "ungido", "urgido", "ultimo", "urubus", "unirem", "uivava", "unisse"]
lista_palavras_u7 = ["univoco", "utiliza", "urgente", "unificar", "usando", "uruguai", "ultraje", "urgindo", "usaveis", "ungidos", "usando", "usufrui", "usurpar", "uranio", "unidade", "urgidos", "uivando", "uniforme", "utilizo", "usassem"]

#INICIO - print que explica as regras do game:
print("Bem-vindo ao jogo!")
print("REGRAS")
print("1 - Você pode escolher o nível de dificuldade de 5, 6, ou 7 caracteres.")
print("2 - A quantidade de caracteres será a quantidade de chances.")
print("3 - Ao errar, mostra quais letras estão na posição correta.")
print("4 - Pode usar Ç, mas não acentos.")
print("5 - O jogo termina ao fim das tentativas.")
print("Boa sorte!\n")

# Função que verifica se a entrada é válida
def obter_input(prompt, valid_inputs):
    while True:
        valor = input(prompt).lower()
        if valor in valid_inputs:
            return valor
        print(f"Entrada inválida. Por favor, insira um valor válido ({', '.join(valid_inputs)}).")

# Solicitando entradas
quantidade_letras = obter_input("Digite com quantas letras você deseja que a palavra tenha (5, 6 ou 7): ", ['5', '6', '7'])
letra_inicial = obter_input("Digite a vogal inicial da palavra (a, e, i, o, u): ", ['a', 'e', 'i', 'o', 'u'])

# Função que seleciona a palavra
def escolher_palavra(letra, tamanho):
    listas = {
        'a': [lista_palavras_a5, lista_palavras_a6, lista_palavras_a7],
        'e': [lista_palavras_e5, lista_palavras_e6, lista_palavras_e7],
        'i': [lista_palavras_i5, lista_palavras_i6, lista_palavras_i7],
        'o': [lista_palavras_o5, lista_palavras_o6, lista_palavras_o7],
        'u': [lista_palavras_u5, lista_palavras_u6, lista_palavras_u7]
    }
    indices = {'5': 0, '6': 1, '7': 2}
    return random.choice(listas[letra][indices[tamanho]])

# Função que verifica a tentativa
def verificar_tentativa(palavra, tentativa):
    resultado = ""
    for i in range(len(palavra)):
        if tentativa[i] == palavra[i]:
            resultado += tentativa[i]  # letra correta na posição correta
        elif tentativa[i] in palavra:
            resultado += tentativa[i].upper()  # letra correta, mas posição errada
        else:
            resultado += "_"
    return resultado

# Função para remover acentos
def remover_acentos(texto):
    return ''.join(c for c in unicodedata.normalize('NFD', texto) if unicodedata.category(c) != 'Mn')

# Seleção de palavra
palavra = escolher_palavra(letra_inicial, quantidade_letras)

# Definir tentativas
tentativas_maximas = 5
tentativas = 0

# Loop principal do jogo
while tentativas < tentativas_maximas:
    tentativa = input(f"Tentativa {tentativas + 1}: ").lower()
    tentativa = remover_acentos(tentativa)

    if len(tentativa) != len(palavra):
        print(f"A palavra deve ter exatamente {len(palavra)} letras. Tente novamente.")
        continue

    if tentativa[0] != letra_inicial:
        print(f"A palavra deve começar com a letra '{letra_inicial}'. Tente novamente.")
        continue

    if tentativa == palavra:
        print(f"Parabéns! Você acertou: {palavra}")
        break
    else:
        resultado = verificar_tentativa(palavra, tentativa)
        print(f"Letras corretas e na posição certa: {resultado}")
    
    tentativas += 1
else:
    print(f"Fim de jogo! A palavra era: {palavra}")
