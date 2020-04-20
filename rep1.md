
#20171132 정인길

#1
```
  void setup(){
  size(500,500);    // 크기화면을 500x500으로 설정합니다
  stroke(0,0,255);   // 선의 색상을 파란색으로 합니다
  strokeWeight(12);  // 선의 굵기를 지정한 숫자만큼 굵게합니다
}
void draw(){
  if(mousePressed)
      line(pmouseX,pmouseY,mouseX,mouseY);   // 마우스의 좌표를 읽어옵니다
}
```


#2 
```
void setup() {
  size(700, 300);  // 크기화면을 700x300으로 설정합니다
  textSize(50);    // 글자크기를 50으로 합니다
}
int i, dir=1, sp=1;     // 변수 i,dir,sp를 선언합니다
void draw() {
  fill(0);                 //글자색을 검은색으로 채웁니다
  background(255, 0, 0);   // 배경을 빨간색으로 설정합니다
  text("20171132", i, 200);  // 출력할 글자를 입력합니다
  if (i>width) dir=-1;   // 크기가 가로의크기보다 커지면 반대쪽으로 이동하는것을 반복합니다
  if (i<0) dir=1;        // 가로의 크기가 0보다 작으면 다시 증가합니다
  i = i+dir*sp;         // 까할수있습니다.
}
void keyPressed(){
sp = key-'0';             // 키보드로부터 0~9의 숫자를 입력받아 빠르기를 조절합니다
}
```


#3

```
float x;
float y;

void setup() {
  size(640, 360);  //  크기화면을 640x360으로 설정합니다 
  noStroke();        // 테두리가 없게합니다
}

void draw() { 
  background(50);  // 배경을 어두운색으로 설정합니다
  x = lerp(x, mouseX, 0.05);  //선형 보간 함수를 사용하여 변수 x의 값에서 mouseX의 값까지 0.05값만큼 변경한 값을 반환합니다.
  y = lerp(y, mouseY, 0.05); // 선형 보간 함수를 사용하여 변수 y의 값에서 mousey의 값까지 0.05값만큼 변경한 값을 반환합니다.
  
  fill(255); // 흰색으로 채웁니다
  stroke(255); // 테두리를 흰색으로합니다.
  ellipse(x, y, 66, 66); // 원을 생성합니다
}

```


#4
```
size(200,200); //크기화면을 640x360으로 설정합니다 
rectMode(CENTER); // 사각형의 중심이 좌표가 되도록 설정합니다
rect(100,100,20,100); // 직사각형을 생성합니다
ellipse(100,70,60,60);  // 원을 생성합니다
ellipse(81,70,16,32);   //  타원을 성합니다
ellipse(119,70,16,32); 
line(90,150,80,160);     // 선을 생성합니다
line(110,150,120,160);
```



#5
```
void draw() {
  background(51); // 배경을 어두운색으로 지정합니다
  translate(mouseX, mouseY); // 기준좌표를 마우스의 좌표로 합니다
  fill(102); // 색을 채웁니다
  stroke(255); // 선의 색상을 흰색으로 합니다
  strokeWeight(2); // 선의 굵기를 지정합니다
  beginShape();  // 도형을 만듭니다
  vertex(0, -50);  
  vertex(14, -20);
  vertex(47, -15);
  vertex(23, 7);
  vertex(29, 40); //  포인트의 x,y좌표를 찍어 도형을 만들듯이 vertex를 사용하여 별모양을 만듭니다
  vertex(0, 25);
  vertex(-29, 40);
  vertex(-23, 7);
  vertex(-47, -15);
  vertex(-14, -20);
  endShape(CLOSE); // 도형만들기를 끝냅니다
}
```

[markdown]()

