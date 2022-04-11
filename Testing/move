#include "SoftwareSerial.h"
#include "DFRobotDFPlayerMini.h"

SoftwareSerial mySoftwareSerial(1, 3); // RX, TX
DFRobotDFPlayerMini myDFPlayer;

void setup() {
  mySoftwareSerial.begin(9600);
  myDFPlayer.begin(mySoftwareSerial);

  myDFPlayer.volume(30);
}

void loop() {
  myDFPlayer.play(1);

  for (byte j = 0;j <= 5;j++){
    for (byte i = 1;i <= 30;i++){
      myDFPlayer.volume(i);
      delay(j*100);
    }
    for (byte i = 30;i >= 1;i--){
      myDFPlayer.volume(i);
      delay(j*100);
    }
  }
}
