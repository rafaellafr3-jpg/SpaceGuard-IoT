// ==========================
// SpaceGuard IoT
// Temperatura + Luminosidade + Vibração
// ==========================

// Vibração
int Led = 12;
int Tilt = 3;
int Estado;

// Temperatura
int ledTemp = 2;

// Luminosidade
int ledLuz = 11;

void setup()
{
  pinMode(A0, INPUT); // TMP36
  pinMode(A1, INPUT); // LDR

  pinMode(ledTemp, OUTPUT);
  pinMode(ledLuz, OUTPUT);

  pinMode(Led, OUTPUT);
  pinMode(Tilt, INPUT);

  Serial.begin(9600);
}

void loop()
{
  // ==========================
  // TEMPERATURA
  // ==========================

  float temperatura =
  (-40 + 0.488155 * (analogRead(A0) - 20));

  if (temperatura > 30)
  {
    digitalWrite(ledTemp, HIGH);
    Serial.println("ALERTA: TEMPERATURA ALTA");
  }
  else
  {
    digitalWrite(ledTemp, LOW);
  }

  // ==========================
  // LUMINOSIDADE
  // ==========================

  int luminosidade = analogRead(A1);

  if (luminosidade > 550)
  {
    digitalWrite(ledLuz, HIGH);
    Serial.println("ALERTA: LUMINOSIDADE ALTA");
  }

  if (luminosidade < 450)
  {
    digitalWrite(ledLuz, LOW);
  }

  // ==========================
  // VIBRAÇÃO / INCLINAÇÃO
  // ==========================

  Estado = digitalRead(Tilt);

  if (Estado == LOW)
  {
    digitalWrite(Led, HIGH);
    Serial.println("ALERTA: VIBRACAO DETECTADA");
  }
  else
  {
    digitalWrite(Led, LOW);
  }

  // ==========================
  // MONITOR SERIAL
  // ==========================

  Serial.print("Temperatura: ");
  Serial.print(temperatura);
  Serial.print(" C | ");

  Serial.print("Luminosidade: ");
  Serial.print(luminosidade);
  Serial.print(" | ");

  Serial.print("Tilt: ");
  Serial.println(Estado);

  delay(500);
}
