# Proyecto

void setup () {  
 
   pinMode(12,OUTPUT);
   pinMode(2,INPUT_PULLUP);
   pinMode(3,INPUT_PULLUP);
}

void loop() {
 int state =digitalRead(2);
 int boton = digitalRead(3); 
 if(state == LOW) {
    tone(12,34.65);
    delay(200);
    noTone(12);
    delay(100);
     tone(12,38.89);
    delay(200);
    noTone(12);
    delay(200);
     
 }
else {
    noTone(12);
}
 if(boton == LOW) {
    tone(12,1046.50);
    delay(200);
   
   
 }
else {
    noTone(12);
 }

}


