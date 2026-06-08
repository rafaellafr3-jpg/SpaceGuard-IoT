# SpaceGuard IoT

## Sistema Inteligente de Monitoramento de Cápsula Espacial

Projeto desenvolvido para a Global Solution FIAP 2026 com o objetivo de simular um sistema embarcado baseado em Internet das Coisas (IoT) para monitoramento das condições internas de uma cápsula espacial.

---

#  Objetivo

Desenvolver uma solução capaz de monitorar em tempo real variáveis importantes para a segurança de uma missão espacial experimental.

O sistema realiza o monitoramento de:

*  Temperatura
*  Luminosidade
*  Vibração / Inclinação
* 
Quando uma condição crítica é detectada, o sistema gera alertas visuais através de LEDs.

---

#  Conexão com a Indústria Espacial

Missões espaciais dependem de sistemas de monitoramento contínuo para garantir a segurança dos astronautas e o correto funcionamento dos módulos da nave.

O projeto SpaceGuard IoT simula esse cenário utilizando sensores conectados a um microcontrolador Arduino, permitindo a coleta e análise de dados em tempo real.

---

#  ODS Relacionados

O projeto está alinhado com os Objetivos de Desenvolvimento Sustentável (ODS) da ONU:

* ODS 9 – Indústria, Inovação e Infraestrutura
* ODS 11 – Cidades e Comunidades Sustentáveis
* ODS 13 – Ação Contra a Mudança Global do Clima

---

#  Componentes Utilizados

* Arduino Uno
* Protoboard
* Sensor TMP36
* Fotorresistor (LDR)
* Sensor de Inclinação
* LEDs
* Resistores
* Cabos Jumpers

---

#  Funcionamento do Sistema

## Sensor de Temperatura

O sensor TMP36 monitora a temperatura interna da cápsula.

* Temperatura acima de 30°C
* LED de alerta ativado

---

## Sensor de Luminosidade

O sensor LDR monitora a intensidade luminosa do ambiente.

* Luminosidade elevada
* LED de alerta ativado

---

## Sensor de Vibração

O sensor de inclinação simula vibrações, impactos ou turbulências.

* Vibração detectada
* LED de alerta ativado

---

#  Tecnologias Utilizadas

* Arduino IDE (C/C++)
* Tinkercad
* GitHub

---

#  Resultados

O sistema foi capaz de:

✅ Monitorar temperatura em tempo real

✅ Monitorar luminosidade em tempo real

✅ Detectar vibrações simuladas

✅ Gerar alertas visuais automáticos

✅ Exibir informações através do Monitor Serial

---

#  Melhorias Futuras

* Integração com display LCD
* Dashboard web para monitoramento remoto
* Conexão Wi-Fi utilizando ESP32
* Armazenamento em nuvem
* Aplicativo móvel para alertas

---

#  Demonstração

Link do vídeo:

https://youtu.be/0BC5_GxHoek

---

#  Simulação

Link do projeto Tinkercad:

(https://www.tinkercad.com/things/5IrDt5BvKUH-grand-tumelo/editel?returnTo=https%3A%2F%2Fwww.tinkercad.com%2Fdashboard%2Fdesigns%2Fall&sharecode=ALlH94MFyL8DQSYSGRoXTZlfmdm5soQHObffyvxLaBc)

---

#  Integrantes

### Rafaella Ferreira de Moraes

RM: 571030

### Aneliza Rondina Bonafé

RM: 572977

---

#  Disciplina

Global Solution 2026 – 1º Semestre

FIAP – Ciência da Computação

Projeto desenvolvido para aplicação dos conceitos de Internet das Coisas (IoT), Sistemas Embarcados e Monitoramento Inteligente aplicado à Indústria Espacial.
