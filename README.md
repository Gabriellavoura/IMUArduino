# Codigo Arduino para IMU MPU9250 
Código utilizado para captar os dados fornecidos pela IMU MPU 9250 e realizar o envio através de um dispositivo NODEMcu para um banco de dados do tipo Firebase


# Requirements
* FirebaseArduino.h
* SPI.h
* ESP8266.h
* Wire.h
* Arduino UNO.
* NodeMCU
* IMU MPU 9250

# Como utilizar

Execute primeiramente o código absoluteMagnetoCalib para realizar a calibração da IMU, mexa o dispositivo em movimentos no formato do número 8 até a calibração estar concluída.

No código principal existe a variável relacionada com a declividade da cidade em que o dispositivo está sendo usado em relação a terra, por isso é necessário trocar o valor dessa variável de acordo com o valor real. No próprio código tem um comentário que explica como encontra esse valor. 


# Filtro

O código principal possui dois filtros o de Madgwick e o de Mahony, utilize o que mais se encaixar em sua aplicação, basta apenas comentar o que não utilizar no código e tirar o comentário do que será usado.
