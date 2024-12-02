# Chatbot da ONG Aumigo 🐾
Este é um projeto de chatbot simples e interativo desenvolvido para a ONG fictícia **Aumigo**, voltada ao resgate, cuidado e adoção de animais. O chatbot responde a perguntas sobre a ONG, adoção, voluntariado, doações e outros temas relacionados.

## Integrantes 👥
- Joao Victor Ferrari De Melo, Joao Henrique de Oliveira, Christian Martins Teixeira e Avalone Cabrera.

## 🛠️ Tecnologias utilizadas
- **Python**: Linguagem principal do projeto.
- **TensorFlow/Keras**: Treinamento e utilização de um modelo de classificação baseado em Redes Neurais.
- **NLTK**: Tokenização e lematização de textos para o processamento de linguagem natural.
- **Tkinter**: Interface gráfica para o chatbot.
- **JSON**: Armazenamento das intenções e respostas do chatbot.

## 📂 Estrutura do projeto
```
|-- intents.json # Arquivo JSON com intenções e respostas do chatbot. 
|-- bot.py # Código principal para executar o chatbot. 
|-- train.py # Código para treinar o modelo de classificação. 
|-- extract.py # Funções auxiliares para processamento e previsão. 
|-- model.keras # Modelo treinado (gerado ao rodar train.py). 
|-- words.pkl # Arquivo com palavras processadas (gerado ao rodar train.py). 
|-- classes.pkl # Arquivo com classes processadas (gerado ao rodar train.py).
```

## ⚙️ Como executar o projeto

### 1. Pré-requisitos
Certifique-se de ter instalado:
- Python 3.8+
- Gerenciador de pacotes `pip`

### 2. Instalando dependências
No terminal, dentro do diretório do projeto, execute:
```
pip install -r requirements.txt
```
Obs: Caso não tenha o arquivo requirements.txt, crie-o com os seguintes pacotes:
```
nltk
tensorflow
numpy
```

3. Treinando o modelo
Se ainda não possui o modelo treinado (model.keras), execute:

```
python train.py
```
Isso irá gerar os arquivos model.keras, words.pkl e classes.pkl.

4. Executando o chatbot
Para iniciar a interface gráfica do chatbot, execute:
```
python bot.py
```
## 🚀 Funcionalidades do chatbot

- Saudações: O chatbot inicia com mensagens de boas-vindas e está pronto para interagir.

- Informações sobre a ONG: Responde a perguntas sobre a missão e o objetivo da organização.

- Adoção de animais: Informa como proceder para adotar um animal.

- Voluntariado: Explica como se tornar voluntário.

- Doações: Lista formas de ajudar com doações.

- Relatos de animais perdidos/encontrados: Oferece suporte para essas situações.

- Respostas aleatórias: Caso não compreenda uma mensagem, sugere reformulações.

## 📌 Observações
Normalização de palavras: O projeto realiza uma normalização básica para lidar com variações comuns em português.
Respostas aleatórias: Quando existem múltiplas respostas possíveis, o bot escolhe uma aleatoriamente.
Margem de erro: O chatbot utiliza um limite de probabilidade (0.25) para evitar respostas incorretas.

## 🐾 Exemplo de interação
Usuário: Olá!
Chatbot: Olá! Eu sou o Aumigo, seu assistente da ONG. Em que posso te ajudar hoje?

Usuário: Como posso adotar um animal?
Chatbot: Que incrível que você quer adotar! Você pode visitar nossa página de adoção ou agendar uma visita para conhecer os animais disponíveis.





