# Bridge-LED-lighting-with-button-on-22-program to lighting three LEDs the components used are: arduino LEDs jumper wires bleadboads pushbutton codeL4 csa
int led1 = 8;
int led2 = 9;
int led3 = 10;
int button = 2;

int buttonState = 0;

void setup() {
  pinMode(led1, OUTPUT);
  pinMode(led2, OUTPUT);
  pinMode(led3, OUTPUT);
  pinMode(button, INPUT);
}

void loop() {
  buttonState = digitalRead(button);

  if (buttonState == HIGH) {
    digitalWrite(led1, HIGH);
    digitalWrite(led2, HIGH);
    digitalWrite(led3, HIGH);
  } else {
    digitalWrite(led1, LOW);
    digitalWrite(led2, LOW);
    digitalWrite(led3, LOW);
  }r
}
