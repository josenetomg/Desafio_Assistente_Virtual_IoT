# Sistema de Automação por Meio de Reconhecimento de Voz

Neste projeto o foco é direcionado para a criação de uma assistente virtual para automação residencial. 

Para que isso seja possível, vamos utilizar redes neurais para interpretação de comando de voz, Arduino, motores, lâmpadas, sirenes e outros
elementos de automação.

Inicialmente você vai precisar das seguintes instalações:

pip install SpeechRecognition

pip install + caminho

https://www.lfd.uci.edu/~gohlke/pythonlibs/#pyaudio

Também vai precisar de uma conta no TinkerCad

(https://www.tinkercad.com/dashboard), onde nosso projeto eletrônico será desenvolvido.

Ideias de projetos:
1) Ligação de atuadores (lâmpadas, motores, sirenes) por meio de controle sem fio e comando de voz;

2) Aplicação de automação em software: busca na internet, busca em listas de dados, automação de software: 
comando de voz para abrir o Excel, Navegador, Word, PowerPoint utilizando a biblioteca OS.

3) Automação envolvendo hardware físico, onde o que fizemos no TinkerCad, pode ser feito em placas eletrônicas, sensores e atuadores
reais.

Estes são alguns exemplos de projetos, mas você pode inovar e realizar uma outra forma de automação, tendo como requisito básico o comando por voz.

Código para a base do projeto:

print("testando")

import speech_recognition as sr
import os

#Função para ouvir e reconhecer a fala

def ouvir_microfone():
 #Habilita o microfone do usuário
 microfone = sr.Recognizer()

 #usando o microfone
 with sr.Microphone() as source:

 #Chama um algoritmo de reducao de ruidos no som
 microfone.adjust_for_ambient_noise(source)

 #Frase para o usuario dizer algo
 print("Diga alguma coisa: ")

 #Armazena o que foi dito numa variavel
 audio = microfone.listen(source)

 try:

 #Passa a variável para o algoritmo reconhecedor de padroes
 frase = microfone.recognize_google(audio,language='pt-BR')
 
 if "navegador" in frase:
 os.system("start Chrome.exe")
 elif "Excel" in frase:
 os.system("start Excel.exe")

 #Retorna a frase pronunciada
 print("Você disse: " + frase)

 #Se nao reconheceu o padrao de fala, exibe a mensagem
 except sr.UnkownValueError:
 print("Não entendi")

 return frase
 ouvir_microfone()