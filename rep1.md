#1과제물
#20171132 정인길

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
