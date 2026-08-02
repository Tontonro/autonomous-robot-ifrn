# 🤖 Robô Autônomo OBR — Projeto Integrador IFRN Santa Cruz

[![Instituição](https://img.shields.io/badge/IFRN-Campus%20Santa%20Cruz-green.svg)](portal.ifrn.edu.br)
[![Competição](https://img.shields.io/badge/OBR-N%C3%ADvel%202%20%7C%20N%C3%ADvel%205-blue.svg)](https://www.obr.org.br/)
[![Plataforma](https://img.shields.io/badge/Hardware-Arduino%20MEGA%202560-00979D.svg)](https://www.arduino.cc/)
[![Simulador](https://img.shields.io/badge/Virtual-sBotics%20(C%23)-purple.svg)](https://sbotics.net/)
[![Linguagem](https://img.shields.io/badge/Linguagem-C%2B%2B%20%2F%20C%23-orange.svg)]()
[![Licença](https://img.shields.io/badge/Licen%C3%A7a-MIT-yellow.svg)](LICENSE)

> **Códigos, Simulações e Referência Técnica para Desenvolvimento de Robôs Autônomos voltados à Olimpíada Brasileira de Robótica (OBR)**  
> *Trabalho do Projeto Integrador do Curso Técnico de Nível Médio em Informática (Forma Integrada) do Instituto Federal do Rio Grande do Norte (IFRN) – Campus Santa Cruz.*

---

## 💡 Visão Geral e Objetivo

A robótica educacional promove o pensamento computacional, o raciocínio lógico e o trabalho em equipe. No âmbito nacional, a **Olimpíada Brasileira de Robótica (OBR)** é o principal evento da área, desafiando estudantes a construir e programar robôs autônomos capazes de realizar missões de resgate em ambientes simulados de desastre.

Contudo, equipes iniciantes do IFRN Campus Santa Cruz frequentemente enfrentavam a ausência de documentação técnica aberta, padronizada e validada. Esse cenário gerava ciclos de tentativa e erro, desperdício de recursos e retrabalho.

Este repositório centraliza uma **solução completa, replicável e de baixo custo (< R$ 600,00)** baseada na plataforma **Arduino MEGA 2560**, contemplando:
1. **Modalidade Prática Presencial (Nível 2):** Robô físico com seguimento de linha via algoritmo PID, desvio de obstáculos ultrassônico, transposição de rampa e garra robotizada em impressão 3D para resgate de vítimas.
2. **Modalidade Prática Virtual (Nível 2):** Modelo equivalente implementado e testado no simulador **sBotics** em C#.
3. **Modalidade Teórica (Nível 5):** Caderno preparatório com fundamentação teórica em eletrônica digital, microcontroladores, lógica de programação e banco de questões resolvidas e comentadas conforme a BNCC e diretrizes do CNE/CEB.

Estima-se que esta base de conhecimento proporcione uma **redução de até 60% no tempo de desenvolvimento** de novas equipes do IFRN Campus Santa Cruz.

---

## ✨ Destaques do Projeto

- 🎯 **Controle PID Discreto:** Algoritmo implementado em C++ para ajuste suave de trajetória sobre a linha.
- 🧱 **Arquitetura Modular de Baixo Custo:** Custo total do hardware mantido abaixo de R$ 600,00, priorizando componentes acessíveis e reaproveitáveis na instituição.
- 🤖 **Atuação Mecânica sob Medida:** Garra leve manufaturada via impressão 3D e acionada por servomotor.
- 💻 **Dupla Validação (Física e Simulada):** Portabilidade do algoritmo do ambiente real para o simulador oficial **sBotics**.
- 📖 **Documentação Aberta (Cultura Maker):** Esquemáticos, código-fonte comentado, guia de calibração e caderno de estudos teóricos integrados.

---

## 👥 Equipe e Orientação

### ✍️ Autores (Discentes)
* 👨‍💻 [**Antonny Adryan de Andrade**](http://lattes.cnpq.br/3764943485025248)
* 👨‍💻 [**Cícero Bento Dantas Fernandes**](http://lattes.cnpq.br/9661989505513469)
* 👨‍💻 [**Gervásio Filho Souza de Lima**](http://lattes.cnpq.br/8523883028703687)
* 👨‍💻 [**Jácio Mauê do Nascimento Silva**](http://lattes.cnpq.br/1822484917550390)

### 👨‍🏫 Orientadores
* 🏫 [**Prof. Gutemberg Santos Santiago**](http://lattes.cnpq.br/1423358177316450) — *Orientador Principal*
* 🏫 [**Prof. Karlo Sérgio Medeiros Leopoldino**](http://lattes.cnpq.br/1397392760629073) — *Coorientador*

**Instituição:** Instituto Federal de Educação, Ciência e Tecnologia do Rio Grande do Norte (IFRN) — Campus Santa Cruz  
**Curso:** Técnico de Nível Médio em Informática na Forma Integrada   

---

## 📈 Metodologia e Gestão Ágil (Scrum)

O projeto adotou uma abordagem **ágil e incremental**, dividida em **Sprints quinzenais**, permitindo a sobreposição e validação rápida do hardware, da simulação virtual e da preparação teórica.

### Backlog de Incrementos

| Incremento | Escopo / Entregáveis Principais |
| :--- | :--- |
| **Inc. 1** | Seguimento de linha básico com matriz de 5 sensores IR e leitura de encoders. |
| **Inc. 2** | Integração do desvio de obstáculos (HC-SR04) + controle PID em rampas. |
| **Inc. 3** | Mecanismo de resgate com garra 3D e servomotor para captura de vítimas. |
| **Inc. 4** | Integração total do robô físico (meta $< 	ext{4min 30s}$) e porte completo para sBotics. |
| **Inc. 5** | Caderno de preparação teórica (20 questões resolvidas) e documentação unificada. |

### Critérios de Aceitação e Indicadores

| Tarefa | Métrica de Sucesso | Meta de Aceitação |
| :--- | :--- | :--- |
| **Seguimento de Linha** | Desvios da faixa preta por percurso | $\le 3$ desvios ($< 2$ segundos) |
| **Desvio de Obstáculo** | Taxa de desvio sem colisão | $\ge 95\%$ de sucesso |
| **Transposição de Rampa** | Subida em inclinação de 15° | $< 3$ segundos sem estancar |
| **Resgate de Vítima** | Captura e deposição das esferas | $\ge 70\%$ de sucesso |
| **Tempo Percurso Físico** | Cronometragem total da pista | $\le 4	ext{ min } 30	ext{ s}$ (máx. 5 min) |
| **Desempenho Virtual** | Taxa de conclusão no sBotics | $\ge 80\%$ de sucesso |
| **Simulado Teórico** | Acertos em prova Nível 5 (20 questões) | $\ge 70\%$ de pontuação |

---

## 🎯 Resultados Esperados e Impacto

1. **Protótipo Físico Validado:** Capaz de concluir a pista presencial da OBR em tempo inferior a 4 minutos e 30 segundos, com taxa de resgate superior a 70%.
2. **Modelo Virtual Replicável:** Taxa de sucesso $\ge 80\%$ nas missões do simulador sBotics.
3. **Redução do Custo Acadêmico:** Solução com custo de material inferior a R$ 600,00, totalmente acessível para escolas públicas e institutos federais.
4. **Transferência de Conhecimento:** Guia técnico detalhado que reduz o tempo de onboarding de futuras equipes do IFRN Campus Santa Cruz em até 60%, fomentando a Cultura Maker e a extensão em robótica.

---

## 📄 Licença

Este projeto é distribuído sob a licença **MIT**. Consulte o arquivo [LICENSE](LICENSE) para obter mais detalhes.

---

<p center="align">
  <b>IFRN Campus Santa Cruz — Curso Técnico em Informática</b><br>
  <i>Desenvolvido com foco na disseminação da Robótica Educacional e da Cultura Maker.</i>
</p>
