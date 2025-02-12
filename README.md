# short_circuit_task1_124ec0014
// C++ code
//
int LEDR=11;
int LEDY=8;
int LEDG=4;
int PUSH_BUTTON=12;
void setup()
{
  pinMode(LEDR, OUTPUT);
  pinMode(LEDY, OUTPUT);
  pinMode(LEDG, OUTPUT);
  pinMode(PUSH_BUTTON, INPUT);
  Serial.begin(9600);
}

void loop()
{
  int memory= digitalRead(PUSH_BUTTON);
  if (memory==0){
    digitalWrite(LEDG, HIGH);
    delay(4000);
     digitalWrite(LEDG, LOW);
    delay(2000);
    digitalWrite(LEDY, HIGH);
    delay(4000);
    digitalWrite(LEDY, LOW);
    delay(2000);
    digitalWrite(LEDR, HIGH);
    delay(4000);
    digitalWrite(LEDR, LOW);
    delay(2000);
  }
  else if(memory==1) {
    Serial.println("Please WAIT, PEDESTRIAN CROSSING");
    digitalWrite(LEDR, HIGH);
    delay(6000);
    
     digitalWrite(LEDR, LOW);
    delay(2000);
    digitalWrite(LEDY, HIGH);
    delay(4000);
    digitalWrite(LEDY, LOW);
    delay(2000);
    digitalWrite(LEDG, HIGH);
    delay(4000);
    digitalWrite(LEDG, LOW);
    delay(2000);
    
  }
  Serial.println(memory);
}
