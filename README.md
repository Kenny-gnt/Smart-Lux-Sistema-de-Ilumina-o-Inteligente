# Smart-Lux-Sistema-de-Ilumina-o-Inteligente

O Smart Lux é um sistema de iluminação automatizado desenvolvido para otimizar o bem-estar de aves em ambientes controlados, reduzindo o consumo de energia elétrica de maneira eficiente e inteligente. O projeto utiliza sensores de luminosidade, temperatura e distância para acionar a iluminação apenas quando as condições ideais são atendidas, garantindo conforto para os animais e promovendo o uso responsável de energia.
----------------------------------------------------------
COMO FUNCIONA 

O sistema é composto por:
- Sensor LDR → Detecta o nível de luminosidade do ambiente;

- Sensor de temperatura (TMP36) → Mede a temperatura local;

- Sensor ultrassônico (HC-SR04) → Identifica a presença de aves ou pessoas próximas;

- LED → Representa a lâmpada controlada automaticamente pelo sistema.


A lâmpada é acionada somente quando:
- O nível de luz ambiente é baixo (LDR abaixo de 400),

- A temperatura está inferior a 25 °C,

- E há presença detectada a até 150 cm de distância.

Dessa forma, o Smart Lux mantém a iluminação ligada apenas quando realmente necessária, equilibrando bem-estar animal e eficiência energética.
----------------------------------------------------------
TECNOLOGIAS UTILIZADAS

- Arduino UNO

- LDR (sensor de luz)

- Sensor de temperatura TMP36

- Sensor ultrassônico HC-SR04

- Linguagem C/C++ (Arduino IDE)
- 
- Python (pandas)
----------------------------------------------------------
ORIENTAÇÃO DE EXECUÇÃO

1. Monte o circuito no Arduino UNO, conectando:

- LDR na entrada analógica A0;

- Sensor de temperatura TMP36 na A1;

- Sensor ultrassônico HC-SR04 nos pinos 5 (TRIG) e 4 (ECHO);

- LED no pino 2.

2. Envie o código para a placa utilizando a Arduino IDE.
Após o upload, abra o Monitor Serial para acompanhar as leituras dos sensores.


3. Salve as leituras exibidas no Monitor Serial em um arquivo chamado coleta_de_dados.csv.
 Esse arquivo armazenará todas as informações captadas pelos sensores (LDR, temperatura, distância e estado da lâmpada).


4. Coloque o arquivo coleta_de_dados.csv na mesma pasta do script analise_Smart_Lux.py.
   
5. Abra o terminal e, caso necessário, instale o pandas:

 pip install pandas
 

6. Execute o script Python com o comando:

 python analise_Smart_Lux.py
 

7. O programa exibirá no terminal:

- As primeiras leituras coletadas;

- As médias de luminosidade, temperatura e distância;

- A porcentagem de tempo em que a lâmpada ficou ligada;

- E a estimativa de economia de energia obtida.

 8. Analise os resultados e, se necessário, ajuste os sensores para otimizar o desempenho e a eficiência do sistema.





