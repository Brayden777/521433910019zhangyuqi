PVector center;
PVector spd;
PVector loc;
float angle=random(TWO_PI);
float angleSpd=0.1;
float rad=100;

void setup() {
  size(720, 720);
  background(#F0BE98);

  center=new PVector(width/2, height/2);
  spd=PVector.random2D();
  spd.mult(2);

  loc=new PVector();
}

void draw() {
  center.add(spd);

  angle+=angleSpd;
  loc.set(center.x+cos(angle)*rad, center.y+sin(angle)*rad);
  
  if(loc.x<0 || loc.x>width|| loc.y<0||loc.y>height){
  center.set(random(width),random(height));
}

  strokeWeight(10);
  stroke(152,random(152,240),240);
  point(loc.x, loc.y);
}
