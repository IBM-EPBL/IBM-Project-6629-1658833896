int GasSensorVal = 0;
int sensorState = 0;
int temp = 0;

void setup()
{
  pinMode(A0, INPUT);
  pinMode(A1, INPUT);
  pinMode(A3, INPUT);
  pinMode(12, OUTPUT);
  pinMode(2, OUTPUT);
  pinMode(12, OUTPUT);
  Serial.begin(9600);

}

void loop()
{
  GasSensorVal = analogRead(A0);
  if (GasSensorVal > 150) {
    digitalWrite(12, HIGH);
    digitalWrite(2, HIGH);
    Serial.println("Detect");
    delay(1000); 
    Serial.println("Not Detect");
    digitalWrite(12, LOW);
    digitalWrite(2, LOW);
  } else {
    digitalWrite(12, LOW);
  }
  {
    if ( sensorState == HIGH) {
    digitalWrite(13, HIGH);
    Serial.println("Sensor activated!");
  } else {
    digitalWrite(13, LOW);
  }
  delay(10); 
}
   {
   temp = analogRead(temp);
   temp = temp * 0.48828125;
   Serial.print("TEMPERATURE = ");
   Serial.print(temp); 
   Serial.print("*C");
   Serial.println();
   delay(1000); 
}
}
