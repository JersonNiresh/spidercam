const int M11 = 2;
const int M12 = 3;
const int M21 = 4;
const int M22 = 5;

const int M31 = 6;
const int M32 = 7;
const int M41 = 8;
const int M42 = 9;
int a = 200;
int b = 100;
void setup() {
  // put your setup code here, to run once:
  Serial.begin(9600);
  pinMode(M11,OUTPUT);
  pinMode(M12,OUTPUT);
  pinMode(M21,OUTPUT);
  pinMode(M22,OUTPUT);
  pinMode(M31,OUTPUT);
  pinMode(M32,OUTPUT);
  pinMode(M41,OUTPUT);
  pinMode(M42,OUTPUT);
  pinMode(10,OUTPUT);
  pinMode(11,OUTPUT);
  
  pinMode(14,INPUT_PULLUP);
  pinMode(15,INPUT_PULLUP);
  pinMode(16,INPUT_PULLUP);
  pinMode(17,INPUT_PULLUP);
  pinMode(18,INPUT_PULLUP);
  pinMode(19,INPUT_PULLUP);
  
  digitalWrite(M11,LOW);
  digitalWrite(M12,LOW);
  digitalWrite(M21,LOW);
  digitalWrite(M22,LOW);
  digitalWrite(M31,LOW);
  digitalWrite(M32,LOW);
  digitalWrite(M41,LOW);
  digitalWrite(M42,LOW);
  
}

void loop() {
  Serial.print(digitalRead(14));Serial.print(",");
  Serial.print(digitalRead(15));Serial.print(",");
  Serial.print(digitalRead(16));Serial.print(",");
  Serial.print(digitalRead(17));Serial.print(",");
  Serial.print(digitalRead(18));Serial.print(",");
  Serial.print(digitalRead(19));Serial.println(",");
  int button1 = digitalRead(14);
  int button2 = digitalRead(15);
  int button3 = digitalRead(16);
  int button4 = digitalRead(17);
  int dir1 =digitalRead(18);
  int dir2 =digitalRead(19);
  
  if (dir1 == LOW && button1 == LOW)
  {
    analogWrite(10,b);
    analogWrite(11,b);
    digitalWrite(M11,HIGH);
    digitalWrite(M12,LOW);
    delay(a);
    digitalWrite(M11,LOW);
    digitalWrite(M12,LOW);
  }
  else if (dir1 == LOW && button2 == LOW)
  {analogWrite(10,b);
    analogWrite(11,b);
    digitalWrite(M21,HIGH);
    digitalWrite(M22,LOW);
    delay(a);
    digitalWrite(M21,LOW);
    digitalWrite(M22,LOW);
  }
  else if (dir1 == LOW && button3 == LOW)
  {analogWrite(10,b);
    analogWrite(11,b);
    digitalWrite(M31,HIGH);
    digitalWrite(M32,LOW);
    delay(a);
    digitalWrite(M31,LOW);
    digitalWrite(M32,LOW);
  }
  else if (dir1 == LOW && button4 == LOW)
  {analogWrite(10,b);
    analogWrite(11,b);
    digitalWrite(M41,HIGH);
    digitalWrite(M42,LOW);
    delay(a);
    digitalWrite(M41,LOW);
    digitalWrite(M42,LOW);
  }
  
  else if (dir2 == LOW && button1 == LOW)
  {analogWrite(10,b);
    analogWrite(11,b);
    digitalWrite(M11,LOW);
    digitalWrite(M12,HIGH);
    delay(a);
    digitalWrite(M11,LOW);
    digitalWrite(M12,LOW);
  }
  else if (dir2 == LOW && button2 == LOW)
  {analogWrite(10,b);
    analogWrite(11,b);
    digitalWrite(M21,LOW);
    digitalWrite(M22,HIGH);
    delay(a);
    digitalWrite(M21,LOW);
    digitalWrite(M22,LOW);
  }
  else if (dir2 == LOW && button3 == LOW)
  {analogWrite(10,b);
    analogWrite(11,b);
    digitalWrite(M31,LOW);
    digitalWrite(M32,HIGH);
    delay(a);
    digitalWrite(M31,LOW);
    digitalWrite(M32,LOW);
  }
  else if (dir2 == LOW && button4 == LOW)
  {analogWrite(10,b);
    analogWrite(11,b);
    digitalWrite(M41,LOW);
    digitalWrite(M42,HIGH);
    delay(a);
    digitalWrite(M41,LOW);
    digitalWrite(M42,LOW);
  }




  
  if (button1 == LOW && button2 == HIGH && button3 == HIGH && button4 == HIGH && dir1 == HIGH && dir2 == HIGH)
  {
    one();
  }
  else if (button1 == HIGH && button2 == LOW && button3 == LOW && button4 == LOW && dir1 == HIGH && dir2 == HIGH)
  {
    two();
  }
  else if (button1 == HIGH && button2 == LOW && button3 == HIGH && button4 == HIGH && dir1 == HIGH && dir2 == HIGH)
  {
    three();
  }
  else if (button1 == LOW && button2 == HIGH && button3 == LOW && button4 == LOW && dir1 == HIGH && dir2 == HIGH)
  {
    four();
  }

  else if (button1 == HIGH && button2 == HIGH && button3 == HIGH && button4 == LOW && dir1 == HIGH && dir2 == HIGH)
  {
    five();
  }
  else if (button1 == LOW && button2 == LOW && button3 == LOW && button4 == HIGH && dir1 == HIGH && dir2 == HIGH)
  {
    six();
  }
  else if (button1 == HIGH && button2 == HIGH && button3 == LOW && button4 == HIGH && dir1 == HIGH && dir2 == HIGH)
  {
    seven();
  }
  else if (button1 == LOW && button2 == LOW && button3 == HIGH && button4 == LOW && dir1 == HIGH && dir2 == HIGH)
  {
    eight();
  }
  
  else
  {
    stop1();
  }
}
int one()
{
  analogWrite(11,200);
  analogWrite(10,b);
  digitalWrite(M11,HIGH);
  digitalWrite(M12,LOW);
  digitalWrite(M21,HIGH);
  digitalWrite(M22,LOW);
  digitalWrite(M31,LOW);
  digitalWrite(M32,HIGH);
  digitalWrite(M41,HIGH);
  digitalWrite(M42,LOW);
}
int two()
{
  analogWrite(10,b);
  analogWrite(11,200);
  digitalWrite(M11,LOW);
  digitalWrite(M12,HIGH);
  digitalWrite(M21,LOW);
  digitalWrite(M22,HIGH);
  digitalWrite(M31,HIGH);
  digitalWrite(M32,LOW);
  digitalWrite(M41,LOW);
  digitalWrite(M42,HIGH);
}
int three()
{
  analogWrite(10,b);
  analogWrite(11,200);
  digitalWrite(M11,LOW);
  digitalWrite(M12,HIGH);
  digitalWrite(M21,LOW);
  digitalWrite(M22,HIGH);
  digitalWrite(M31,LOW);
  digitalWrite(M32,HIGH);
  digitalWrite(M41,HIGH);
  digitalWrite(M42,LOW);
}
int four()
{
  analogWrite(10,b);
  analogWrite(11,200);
  digitalWrite(M11,HIGH);
  digitalWrite(M12,LOW);
  digitalWrite(M21,HIGH);
  digitalWrite(M22,LOW);
  digitalWrite(M31,HIGH);
  digitalWrite(M32,LOW);
  digitalWrite(M41,LOW);
  digitalWrite(M42,HIGH);
}

int five()
{
  analogWrite(10,200);
  analogWrite(11,b);
  digitalWrite(M11,HIGH);
  digitalWrite(M12,LOW);
  digitalWrite(M21,LOW);
  digitalWrite(M22,HIGH);
  digitalWrite(M31,HIGH);
  digitalWrite(M32,LOW);
  digitalWrite(M41,HIGH);
  digitalWrite(M42,LOW);
}
int six()
{
  analogWrite(10,200);
