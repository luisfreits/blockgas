# BlockGas - Monitoramento de Gás com ESP32 e Telegram

Este projeto serve para detectar vazamentos de gás usando um sensor conectado a um ESP32. Quando detecta gás, ele toca um alarme e manda um aviso pelo Telegram. Você pode configurar tudo de forma fácil pelo computador, usando uma página na internet.

---

## O que o projeto faz

* **Detecta gás** usando um sensor simples.
* **Toca um alarme** quando detecta gás.
* **Manda mensagem no Telegram** avisando sobre o vazamento.
* **Permite configurar pelo computador** usando um cabo USB e uma página web.
* **Guarda as configurações** (como Wi-Fi e Telegram) mesmo se desligar da tomada.
* **Tem opção de resetar tudo** e começar do zero pela página web.
* **Mostra mensagens de status** na tela do computador para acompanhar o que está acontecendo.

---

## O que você precisa

* **Peças:**
  * ESP32 (placa eletrônica)
  * Sensor de gás (exemplo: MQ-2)
  * Buzzer (faz o som do alarme)
* **No computador:**
  * Arduino IDE (programa para enviar o código para o ESP32)
  * Algumas bibliotecas (programas extras para o ESP32 funcionar com Wi-Fi e Telegram)
* **No navegador:**
  * Uma página web simples (HTML + JavaScript) para conversar com o ESP32 pelo cabo USB

---

## Como funciona

* O ESP32 liga e tenta conectar no Wi-Fi usando as informações que já estão salvas.
* Se não tiver nada salvo, ele espera você enviar pelo computador:
  * Para configurar: `0;nome_do_wifi;senha_do_wifi;id_do_telegram`
  * Para resetar tudo: `1`
* Se detectar gás, toca o alarme e manda mensagem no Telegram.
* Tudo o que acontece aparece na tela do computador em tempo real.

---

## Melhorias que podem ser feitas

* Melhorar a conexão com o Wi-Fi para não cair.
* Permitir mais de um sensor ou mais de um usuário.
* Deixar a página web mais bonita e mostrar histórico dos alertas.

---

## Quem fez

* Heitor — https://github.com/heitor0846
* Luís Freits — https://github.com/luisfreits