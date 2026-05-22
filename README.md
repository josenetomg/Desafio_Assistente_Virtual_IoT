# Assistente Virtual IoT com Redes Neurais para Automação Residencial

<p align="center">
  <img src="https://img.shields.io/badge/Projeto-DIO_IoT_Challenge-orange?style=for-the-badge" alt="DIO Project">
  <img src="https://img.shields.io/badge/IA-Redes_Neurais_/_NLP-blue?style=for-the-badge" alt="Neural Networks">
  <img src="https://img.shields.io/badge/Hardware-Arduino_e_IoT-green?style=for-the-badge" alt="Arduino IoT">
</p>

## 📌 Sobre o Projeto

Este repositório foi desenvolvido para o desafio de projeto focado em **Internet das Coisas (IoT)** e **Inteligência Artificial** da **Digital Innovation One (DIO)**. O objetivo central é o desenvolvimento de uma arquitetura completa de **Assistente Virtual para Automação Residencial (Smart Home)**, integrando processamento de linguagem e controle de hardware em tempo real.

O sistema utiliza **Redes Neurais** para a interpretação e classificação de comandos de voz, convertendo a linguagem natural humana em gatilhos lógicos que controlam periféricos físicos gerenciados por microcontroladores **Arduino**.

---

## 🏗️ Arquitetura do Sistema e Fluxo de Dados

A solução opera através da integração de três camadas principais:

Para este repositório, que conecta duas das suas maiores especialidades — **Inteligência Artificial (Redes Neurais)** e **Hardware/Sistemas Embarcados (Arduino e Automação)** —, a descrição precisa destacar a arquitetura da solução. O leitor do seu portfólio deve entender de imediato como a IA processa a voz e como o hardware executa a ação no mundo físico.

Aqui está o código Markdown estruturado de forma técnica e profissional para atualizar o README.md do seu repositório:

---

```markdown
# Assistente Virtual IoT com Redes Neurais para Automação Residencial

<p align="center">
  <img src="https://img.shields.io/badge/Projeto-DIO_IoT_Challenge-orange?style=for-the-badge" alt="DIO Project">
  <img src="https://img.shields.io/badge/IA-Redes_Neurais_/_NLP-blue?style=for-the-badge" alt="Neural Networks">
  <img src="https://img.shields.io/badge/Hardware-Arduino_e_IoT-green?style=for-the-badge" alt="Arduino IoT">
</p>

## 📌 Sobre o Projeto

Este repositório foi desenvolvido para o desafio de projeto focado em **Internet das Coisas (IoT)** e **Inteligência Artificial** da **Digital Innovation One (DIO)**. O objetivo central é o desenvolvimento de uma arquitetura completa de **Assistente Virtual para Automação Residencial (Smart Home)**, integrando processamento de linguagem e controle de hardware em tempo real.

O sistema utiliza **Redes Neurais** para a interpretação e classificação de comandos de voz, convertendo a linguagem natural humana em gatilhos lógicos que controlam periféricos físicos gerenciados por microcontroladores **Arduino**.

---

## 🏗️ Arquitetura do Sistema e Fluxo de Dados

A solução opera através da integração de três camadas principais:


```

[ Comando de Voz ]
│
▼
┌───────────────────────────────────┐
│   Camada de IA & Processamento    │ -> Processamento de Linguagem Natural (NLP)
│   (Classificação via Redes Neurais)│    Reconhecimento de Intenções (Intent Parsing)
└───────────────────────────────────┘
│
▼  [ Sinal Lógico / Serial ou Wi-Fi ]
┌───────────────────────────────────┐
│        Camada de Controle         │ -> Microcontrolador Arduino (ATmega328P / ESP8266)
│         (Firmware/Lógica)         │    Mapeamento de Pinos e Relés
└───────────────────────────────────┘
│
▼
┌───────────────────────────────────┐
│  Camada de Atuação (World Physics)│ -> Lâmpadas, Motores, Sirenes, Cargas de Potência
└───────────────────────────────────┘

```

---

## ⚙️ Componentes e Atuadores Mapeados

O firmware e o circuito foram projetados para gerenciar elementos críticos de uma casa inteligente através de uma matriz de atuadores:

*   **Iluminação Inteligente:** Controle de acionamento de lâmpadas utilizando módulos relé isolados para isolamento da rede elétrica residencial.
*   **Controle de Acesso e Motores:** Simulação de abertura de portões eletrônicos ou persianas automatizadas através do controle de motores (DC, de Passo ou Servo).
*   **Módulo de Segurança e Alarme:** Disparo autônomo de alertas sonoros de alta potência (sirenes e buzzers) acionados por comandos de voz de emergência ou gatilhos de sensores de presença.

---

## 🛠️ Tecnologias e Conceitos Aplicados

*   **Inteligência Artificial:** Modelagem de Redes Neurais Artificiais (RNAs) para extração de características de áudio ou texto e classificação de intenções de comandos.
*   **Sistemas Embarcados & IoT:** Programação em C/C++ para ecossistema Arduino, gerência de GPIOs (portas de entrada e saída) e protocolos de comunicação (Serial, I2C, SPI ou Wi-Fi/MQTT).
*   **Eletrônica de Potência Básica:** Chaveamento de cargas AC/DC usando transistores e relés acoplados ao microcontrolador.

---

<p align="center">
  Desenvolvido por <a href="https://github.com/josenetomg">José Joaquim Brandão Neto</a> — Projetando a convergência entre IA avançada e o controle de hardware físico.
</p>

```

