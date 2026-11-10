# 🚌 Senta Aí

> **Monitoramento em tempo real de ocupação e fluxo de passageiros no transporte público.**

Bem-vindo à organização oficial do **Senta Aí**! Nossa missão é otimizar o transporte urbano utilizando IoT e processamento em tempo real, fornecendo estatísticas exatas de lotação de cada ônibus da malha para operadores e passageiros.

---

## 🏗️ Como Funciona

Nosso ecossistema combina hardware embarcado de baixo custo com uma arquitetura de backend de alta performance:

* **Coleta na Ponta (IoT):** Módulos **ESP32** instalados nos veículos gerenciam e processam os dados dos sensores.
* **Contagem de Fluxo:**
  * **Catracas:** Contabilizam o embarque exato de passageiros.
  * **Portas:** Sensores dedicados identificam o fluxo de entrada, saída e re-entradas.
* **Comunicação por MQTT:** Os microcontroladores transmitem os dados de telemetria em tempo real utilizando o protocolo **MQTT**, garantindo alta eficiência, leveza e baixa latência.
* **Ingestão e Processamento (Backend Java):** Uma API robusta em **Java** consome os tópicos MQTT, processando os eventos e mantendo o estado atualizado de lotação de cada ônibus.

---

## ⚙️ Tecnologias Utilizadas

* **Embarcado (IoT):** C/C++ (Arduino/ESP-IDF), ESP32, Sensores de Contagem de Pessoas.
* **Mensageria & Comunicação:** Protocolo MQTT para transmissão de telemetria dos veículos.
* **Backend:** Java, APIs e clientes de mensageria para ingestão e gerenciamento de estado da frota.

---

## 📦 Repositórios Principais

* [`senta-ai-firmware`](https://github.com/SentaAI/senta-ai-firmware) — Código para os microcontroladores ESP32 (gestão de sensores nas portas, catracas e publicação MQTT).
* [`senta-ai-backend`](https://github.com/SentaAI/senta-ai-backend) — API em Java responsável por assinar os tópicos MQTT, processar e gerenciar os dados da frota.
* [`senta-ai-frontend`](https://github.com/SentaAI/senta-ai-frontend) — Front-End desenvolvido em React, dando um contexto geral da solução.
* [`senta-ai-docs`](https://github.com/SentaAI/senta-ai-docs) — Documentação de arquitetura, tópicos e protocolos.

---

<div align="center">
  <sub>Desenvolvido com ☕ e IoT pela equipe Senta Aí.</sub>
</div>
