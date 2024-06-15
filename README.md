# The Bug Hunting

<details>
<summary><strong>🧑‍💻 O que deverá ser desenvolvido</strong></summary><br />

Neste exercício, você vai praticar os seus conhecimentos em Python e a habilidade de debugar código.

Para isso, você vai receber algumas pequenas aplicações em Python que possuem alguns erros no código que impedem que ele funcione corretamente. Seu trabalho será identificar e corrigir esses erros!

<br />

</details>
  
<details>
  <summary><strong>:memo: Habilidades a serem trabalhadas</strong></summary><br />

Neste exercício, verificamos se você é capaz de:

- Identificar erros em código Python
- Corrigir erros em código Python
- Utilizar a ferramenta de debug integrada ao VS Code
- Escrever código Python que passa em testes de integração

</details>

<br/>

# Orientações
  
<details>

   <summary><strong>‼ Antes de começar a desenvolver </strong></summary><br />

1. Instale as dependências

- Siga os passos do tópico [**🏕️ Ambiente Virtual**]

</details>

<details>
  <summary><strong>🏕️ Ambiente Virtual</strong></summary>
  O Python oferece um recurso chamado de ambiente virtual, onde permite sua máquina rodar sem conflitos, diferentes tipos de projetos com diferentes versões de bibliotecas.

  1. **Criar o ambiente virtual**

  ```bash
  python3 -m venv .venv
  ```

  2. **Ativar o ambiente virtual**

  ```bash
  source .venv/bin/activate
  ```

  3. **Instalar as dependências no ambiente virtual**

  ```bash
  python3 -m pip install -r dev-requirements.txt
  ```

  Com o seu ambiente virtual ativo, as dependências serão instaladas neste ambiente.
  Quando precisar desativar o ambiente virtual, execute o comando `deactivate`. Lembre-se de ativar novamente quando voltar a trabalhar no exercício.

  O arquivo `dev-requirements.txt` contém todas as dependências que serão utilizadas no exercício.

  Se o VS Code não reconhecer as dependências instaladas no ambiente virtual criado, será necessário informar o caminho do interpretador Python. Para isso, abra o VS Code e pressione `Ctrl + Shift + P` (no Mac, `Cmd + Shift + P`) e digite `Python: Select Interpreter`. Selecione o interpretador que possui o caminho `./.venv/bin/python` no nome.
</details>

# Exercícios

📍 **Dica importante:** Os exercícios envolvem a alteração de códigos existentes para que bugs sejam corrigidos, mas não esperamos que você faça grandes alterações.

👎 Você não deve alterar assinaturas de funções (como o nome da função ou os parâmetros que ela recebe), nem removê-las. Você também não deve alterar os testes, apenas o código que está sendo testado.

👍 Você pode adicionar uma nova função, alterar uma condicional, remover uma linha, etc.

## 1. Identifique e corrija os erros no arquivo `src/word_finder.py`

No arquivo `src/word_finder.py` há um código que deveria retornar uma lista de linhas de um arquivo que contém uma determinada palavra. Porém, há 2 erros no código que impedem que ele funcione corretamente.

Seu objetivo é identificar e corrigir os erros no código.

<details>

<summary> Como o código deveria funcionar </code>
</summary><br/>

A aplicação do arquivo `src/word_finder.py` deve ser executada da seguinte forma:

```bash
python3 src/word_finder.py
```

Ao executar o comando acima, a aplicação deveria retornar uma lista de linhas de um arquivo que contém uma determinada palavra. No código atual, a palavra que está sendo buscada é `python` e o arquivo que está sendo lido é o `data/word_finder.txt`.

Nesse caso, a saída esperada é a seguinte:

```txt
[1, 2, 3, 4, 6, 8]
```

</details>

## 2. Identifique e corrija os erros no arquivo `src/spotify.py`

No arquivo `src/spotify.py` há um código que deveria processar as músicas do arquivo `data/spotify.csv` e retornar a análise solicitada na linha de comando.

Porém, há 2 erros no código que impedem que ele funcione corretamente.

Seu objetivo é identificar e corrigir os erros no código.

<details>

<summary> Como o código deveria funcionar </code>
</summary><br/>

As possíveis análises são:

- `1`: retorna as músicas mais instrumentais;
- `2`: retorna as músicas mais dançantes;
- `3`: retorna as músicas mais enérgicas.

A aplicação do arquivo `src/spotify.py` deve ser executada da seguinte forma:

```bash
python3 src/spotify.py 1
```

Ao executar o comando acima, a aplicação deveria retornar a lista das 10 músicas "mais instrumentais", mas você pode escolher qualquer uma das análises disponíveis (`1`, `2` ou `3`).

No nosso caso, a saída esperada é:

```txt
Top 10 músicas mais instrumentais:
 1 - 'Cornfield Chase' de Hans Zimmer
 2 - 'Day One (Interstellar Theme)' de Hans Zimmer
 3 - 'Chevaliers De Sangreal - From The Da Vinci Code Original Motion Picture Soundtrack' de Hans Zimmer
 4 - 'Experience' de Ludovico Einaudi
 5 - 'The Tree' de Ludovico Einaudi
 6 - 'Temple White' de Ludovico Einaudi
 7 - 'Natural Light' de Ludovico Einaudi
 8 - 'First Step' de Hans Zimmer
 9 - 'Veridis Quo' de Daft Punk
10 - 'Goldberg Variations, BWV 988: Aria' de Johann Sebastian Bach
```

</details>

---