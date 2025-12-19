# 💧 BlueFlow

Projeto desenvolvido para a disciplina Performance em Sistemas Ciberfísicos, com foco em IoT, sistemas embarcados e integração web, utilizando ESP32 para monitoramento de consumo de água em tempo real.

O sistema permite o monitoramento remoto da vazão e do histórico de consumo de água, além da detecção automática de vazamentos. Para isso, utiliza um sensor de fluxo conectado ao ESP32, com envio dos dados para a nuvem via Firebase e visualização por meio de uma interface web interativa.

---

## 🚀 Objetivo e Funcionalidades

O BlueFlow tem como objetivo monitorar o consumo de água em tempo real, oferecendo dados precisos, acesso remoto e alertas automáticos, com o intuito de auxiliar na economia de água e na identificação de desperdícios. Para isso, o sistema oferece as seguintes funcionalidades:
- Monitoramento da vazão atual (L/min)
- Armazenamento do histórico de consumo (hora, semana e mês)
- Cálculo da vazão média
- Identificação do pico de vazão
- Indicação do mês com maior consumo
- Detecção automática de vazamentos
- Visualização dos dados em interface web responsiva

---

## 🧠 Arquitetura do Sistema

A arquitetura do BlueFlow é baseada na integração entre hardware, software em nuvem e interface web, permitindo o monitoramento contínuo e remoto do consumo de água.

**1. Sensor de Fluxo (YF-S201):**  
Mede o volume de água por meio da geração de pulsos proporcionais à vazão.

**2. Microcontrolador ESP32:**  
Atua como o núcleo do sistema, sendo responsável por processar os pulsos enviados pelo sensor de fluxo, calcular a vazão e o consumo total de água, identificar padrões anormais de consumo para a detecção de vazamentos e realizar o envio dos dados via conexão Wi-Fi.

**3. Firebase Realtime Database:**  
Armazena os dados de consumo em tempo real, permitindo acesso remoto às informações.

**4. Interface Web:**  
Exibe gráficos, métricas, histórico de consumo e alertas de vazamento de forma intuitiva.

---

## 🛠️ Tecnologias Utilizadas

O desenvolvimento do BlueFlow envolveu a integração de diferentes tecnologias de hardware e software, essenciais para o funcionamento do sistema.

- **Hardware:**  
  - ESP32 DevKit V1
  - Sensor de fluxo de água YF-S201
  - Protoboard
  - Jumpers
  - Mangueira de jardim
  - Adaptadores de mangueira
  - Cabo micro USB

- **Software e Plataformas:**
  - Firebase Realtime Database
  - Wokwi (ambiente de simulação)

- **Linguagens:**
  - C++
  - JavaScript
  - HTML
  - CSS

- **Bibliotecas:**
  - `WiFi.h`
  - `FirebaseESP32.h`
  - `Ticker.h`
  - `Wire.h`
  - `time.h`

---

## 🧪 Testes Realizados

Os testes foram conduzidos com o objetivo de validar o funcionamento correto do sistema, garantindo a confiabilidade dos dados coletados e a estabilidade da comunicação entre os componentes.

- Testes isolados do sensor de fluxo em ambiente de simulação (Wokwi)
- Validação da lógica de cálculo da vazão e do consumo total
- Testes da detecção automática de vazamentos com padrões contínuos de consumo
- Testes de comunicação Wi-Fi entre o ESP32 e o Firebase
- Testes de estabilidade, reconexão de rede e envio contínuo de dados
- Verificação da exibição correta das informações na interface web

---

## 👥 Integrantes da Equipe

Este projeto foi desenvolvido por:
- Arthur Rodrigues Pansera
- Jean Inácio Praes
- João Gabriel de Lima Coltre
- Stefany Carlos de Oliveira