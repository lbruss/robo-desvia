![GitHub License](https://img.shields.io/github/license/lbruss/robo-desvia?style=flat)

# Robô desvia obstáculos
Projeto de um robô que consegue desviar de obstáculos usando sensores de chave fim de curso.

---

#  Projeto: Robô Desvia de Obstáculos

Este projeto reúne **experimentos e simulações** realizados durante as aulas, com o uso do **Tinkercad**.  
Todas as montagens foram **simuladas virtualmente**, sem o uso de materiais físicos.

O objetivo principal foi **compreender o controle de motores** e desenvolver um **robô capaz de desviar de obstáculos**.

---

##  Controle de Sentido de Motores

O primeiro experimento teve como foco entender **como inverter e controlar o sentido de rotação de motores DC**.

<img width="946" height="529" alt="Controle de Motores" src="https://github.com/user-attachments/assets/c8f6f546-99ab-465e-b3a3-2214af00527c" />

### Materiais Simulados

<img width="1084" height="347" alt="Materiais" src="https://github.com/user-attachments/assets/f9509297-3ecd-4624-be07-f80d6a743328" />

---

##  Desafio: Sistema com Sensores de Fim de Curso

<img width="1003" height="548" alt="Desafio" src="https://github.com/user-attachments/assets/e9fe97c5-3464-4ce6-bb01-821486582285" />

###  Observações
- O **sensor de fim de curso** não está disponível no Tinkercad.  
  → Foi substituído por um **interruptor deslizante**.  
- O experimento foi **apenas simulado**, sem o uso de componentes reais.  

###  Materiais Utilizados
<img width="1408" height="269" alt="Materiais Desafio" src="https://github.com/user-attachments/assets/dca90640-d231-4d86-8561-3242b71bbc5c" />

### Robô BUG ver 2.0

<img width="1172" height="603" alt="Captura de tela 2025-10-09 140914" src="https://github.com/user-attachments/assets/7a6976a0-87c5-4f69-b2bc-923021026c75" />

**A imagem acima é uma versão corrigida do do Robô no Tinkercad**
---

##  Etapa 1 – Montagem do Robô

Durante a aula, recebemos kits contendo:

1. **3 rodas** (incluindo 1 boba);  
2. **1 placa controladora**;  
3. **8 baterias**, entre outros componentes.  

Durante a montagem, tivemos dificuldades para encaixar as rodas, mas conseguimos resolver.  
As baterias foram instaladas, e a próxima etapa foi **realizar as conexões elétricas**.

---

##  Soldagem dos Fios

Esta etapa consistiu em **soldar e conectar** os fios entre as **baterias, motores, sensores de fim de curso** e a **chave geral**.

###  Preparação Inicial
- O **fio negativo** de uma bateria estava curto → foi adicionado um **extensor**.  
- Os **sensores de fim de curso** foram fixados na parte superior da placa, um em cada canto.

---

###  Lado Esquerdo
1. Soldar o **positivo da bateria esquerda** no **motor esquerdo**.  
2. Soldar um **fio do motor esquerdo** até o **Comum (C)** do **sensor direito**.  
3. Estender o **fio negativo da bateria esquerda** até o **T1** do **sensor direito**.

###  Lado Direito
1. Soldar o **negativo da bateria direita** no **motor direito**.  
2. Soldar um **fio do motor direito** até o **Comum (C)** do **sensor esquerdo**.  
3. Soldar o **positivo da bateria direita** no **T2** do **sensor direito**.

---

###  Conexões Entre Sensores
- Ligar **T1 ↔ T1** e **T2 ↔ T2** entre os sensores.  
- Unir o **positivo da bateria esquerda** com o **negativo da bateria direita**.

---

## Resumo das Ligações

| Lado | Conexões Principais |
|------|---------------------|
| **Esquerdo** | + da bateria → motor / – da bateria → T1 do sensor direito |
| **Direito** | – da bateria → motor / + da bateria → T2 do sensor direito |
| **Sensores** | Interligados (T1↔T1 e T2↔T2) |
| **Baterias** | + esquerda ↔ – direita |
| **Chave geral** | Controla o circuito entre motor direito e sensor esquerdo |

---

## Montagem Final e Correções

Durante os testes finais, foi necessário **refazer toda a fiação**, pois os motores não estavam funcionando corretamente.

### Etapas de Soldagem Final
1. **Motores e Sensores**
   - Fios soldados nos pinos A dos motores → Comuns dos sensores.  
   - **+ da bateria esquerda** → pino do meio do sensor esquerdo.  
   - **– da bateria direita** → pino direito do sensor direito.  
   - Interligações entre sensores (direito ↔ esquerdo) nos pinos laterais e centrais.

2. **Motores (Pino B)**
   - Fios curtos soldados em cada motor (pino B).  
   - Conexão de alimentação unindo **4 fios** (negativo esquerdo, positivo direito e fios dos motores).

### Testes
- **1º teste:** apenas uma roda funcionou.  
- **Correção:** fios do **motor esquerdo** invertidos.  
- **Resultado:** funcionamento completo após correção.

---

## Resultado Final

O **Robô Desvia** foi concluído com sucesso!  
O sistema de sensores e motores respondeu corretamente, permitindo que o carrinho **detectasse e desviasse de obstáculos**.

O projeto proporcionou um excelente aprendizado sobre:
- Controle de motores DC  
- Sensores de fim de curso  
- Conexões elétricas e soldagem  
- Montagem lógica de um circuito funcional  

---

 **Conclusão:**  
> A simulação no **Tinkercad** demonstrou, de forma prática, como sensores e motores podem ser integrados para criar um robô autônomo simples, eficiente e educativo.


---

## Autor
Bruss Loza
