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
<img width="1536" height="1024" alt="file_000000009b54722f8b37d3998bcf0dfe" src="https://github.com/user-attachments/assets/a4d7cad1-b4bc-4e43-92cf-9054fb21aee2" />
