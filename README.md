# arduino-trafficlights
Test Arduino script to create simple traffic lights

![Breadboard and Arduino pinout](http://i.imgur.com/lv244m7.png "Breadboard and Arduino pinout")

    int red = 13;
    int amber = 12;
    int green = 11;
    
    void setup() {
      pinMode(red, OUTPUT);
      pinMode(amber, OUTPUT);
      pinMode(green, OUTPUT);
    }
    
    void loop() {
      digitalWrite(green, HIGH);
      digitalWrite(red, LOW);
      digitalWrite(amber, LOW);  
      delay(5000);
      digitalWrite(amber, HIGH);
      delay(1000);
      digitalWrite(red, HIGH);
      digitalWrite(amber, LOW);
      digitalWrite(green, LOW);  
      delay(5000);
      digitalWrite(red, LOW);  
      digitalWrite(amber, HIGH);
      delay(500);
      digitalWrite(amber, LOW);
      delay(500);
      digitalWrite(amber, HIGH);
      delay(500);
      digitalWrite(amber, LOW);
      delay(500);
      digitalWrite(amber, HIGH);
      delay(500);
      digitalWrite(amber, LOW);
      delay(500);
      digitalWrite(amber, HIGH);
      delay(500);
      digitalWrite(red, LOW);
      digitalWrite(green, HIGH);
      digitalWrite(amber, LOW);
      delay(5000);
    }
