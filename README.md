//
const int nappipin = 2;
const int ledpin = 13;
int napintila = 0;
void setup()
{
  pinMode(ledpin, OUTPUT);
  pinMode(nappipin, INPUT);
}

void loop()
{
napintila = digitalRead(nappipin);
  if(napintila == HIGH) {
    digitalWrite(ledpin, HIGH);
}
  else {
    digitalWrite(ledpin, LOW);
  }
