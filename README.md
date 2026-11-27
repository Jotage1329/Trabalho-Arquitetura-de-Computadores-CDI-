# cardiodesfibrilador implantável (CDI): a moeda que salva vidas
Integrante: Jorge Henrique Dias Combé (e-mail: jorgecombe@UPE.br / Github: Jotage1329)

## Contexto e História:

Arritmia acontece quando o coração de uma pessoa bate rápido demais (taquicardia), devagar demais (bradicardia) ou de forma descompassada e irregular, podendo acarretar na morte até dos maiores atletas da humanidade. Entretanto, há um dispositivo chamado Cardiodesfibrilador implantável (CDI) que detecta anomalias no funcionamento cardíaco e, caso necessário, causa um choque no coração para reanimá-lo.

<img width="1200" height="800" alt="image" src="https://github.com/user-attachments/assets/45aaaeca-c2b4-4070-9b26-002768adca47" />

Com base no dispositivo anterior, este projeto é uma simulação no tinkercad onde o usuário pode apertar um botão e o dispositivo detecta a quantidade de pressionamentos a cada 3 segundos, e disso o dispositivo arduino retorna um led de cor verde, amarelo ou vermelho, e também aciona um piezo no caso de não receber resposta.

## Funcionadlidades:

-Detecção de batimentos cardíacos;
-Verificação do estado do usuário em tempo real;
-Acionamento de alerta em caso de parada cardíaca;

## Especificações técnicas e componentes:

<img width="894" height="529" alt="image" src="https://github.com/user-attachments/assets/bb02d441-822f-41bd-b35a-af46048dc03f" />

OBS: caso queira construir um dispositivo para ser usado na vida real com um coração de verdade, você precisaria de um MAX30102 (sensor óptico que usa luz para estimar pulso e saturação de oxigênio) ou um AD8232 (capta sinais elétricos relacionados à atividade cardíaca).

## Diagrama de Conexões:

**1-Conecte os pinos de V5 e GND do arduino com o protoboard**

<img width="1214" height="769" alt="image" src="https://github.com/user-attachments/assets/875021ff-03d7-4c94-ba98-2b411f55b4b2" />

**2-Conecte o GND e VCC do dispisitivo LCD com o protoboard. Em seguida, conecte o SDA e o SCL para o A4 e A5 do arduino, respectivamente.**

<img width="862" height="644" alt="Captura de tela 2026-11-26 233400" src="https://github.com/user-attachments/assets/21653ae0-839b-424b-b4c4-7aa0f1d60315" />

**3-Encaixe o botão no protoboard. Em seguida, conecte usando um resistor o terminal 1A à fileira inferior do GND. Para finalizar, conecte a entrada 2B ao 2 digital do arduino**

<img width="857" height="618" alt="image" src="https://github.com/user-attachments/assets/8ad1eef5-f7c6-47ca-84d7-7ec19ae263e5" />

**4-Conecte o piezo ao protoboard. Conecte o pino negativo com o GND do protoboard e o pino poisitivo à entrada 11 do arduino**

<img width="766" height="600" alt="image" src="https://github.com/user-attachments/assets/1ab94454-23bd-446c-b6c3-0507ff215309" />

**5-conecte o led vermelho ao protoboard. Em seguida, conecte o pino catódico ao GND do protoboard e o pino anótico à entrada 8 do arduino. Repita este passo para os leds seguintes, mas conectado o led amarelo à entrada 9 e o verde na entrada 10**

<img width="873" height="658" alt="image" src="https://github.com/user-attachments/assets/09840e0c-d7a5-42df-82dd-6c2258015dea" />

E, finalmente, seu projeto estará terminado

Caso queira experimentar, aqui está o link de uma versão no tinkercad simulando o circuito inteiro: https://www.tinkercad.com/things/hwMTyF93VLJ-dispositivo-simulador-de-batidas-de-coracao
