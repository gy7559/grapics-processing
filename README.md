# Report 2-2
## 안동대학교 윤효원

...
PFont f;
void setup(){
  size(800,300);
  textSize(60);
  f=createFont("궁서",64);
  textFont(f);
  text(0,0,255);
}
int i, dir=1, sp=1;
void draw(){
  fill(0);
  background(200,10,0);
  text("안동대 컴공 사랑합니다" , i, 170);
  if(i>width-684) dir=-1;
  if(i<0) dir=1;
  i= i+dir*sp;
  if(keyPressed) sp = key-'0';
}
...
