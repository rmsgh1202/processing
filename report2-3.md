PFont f;
void setup(){
  size(1600, 800);
  f = createFont("굴림",64);
  textFont(f);
  textSize(128);
}
int i, dir=1, sp=1;
void draw(){
  fill(0);
  background(255);
  text("안동대 컴공 사랑합니다.", i, 450);
  if(i>width-128/2*1) dir=-1;
  if(i<0) dir=1;
  i = i+dir*sp;
  if(keyPressed){
    sp = key-'0';
  }
}
