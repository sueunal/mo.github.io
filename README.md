# JAVA Programing


### 생성자 this()와 this.의 차이

```
class ConstructExample{
   int x ;
  ConstructExample(String a){
      :: this(1); ::    <- 생성자 안에서 자기 자신이 아닌 (int B)를 매개변수로 가지는 생성자를 호출함
      System.out.println("생성자 호출입니다");
   }
   ConstructExample(int B){
       System.out.println("A");
   }
   public void setX(int x){this.x = x;}
   public int getX(){
      return x;
   }

   public static void main(String[] args){
      ConstructExample a = new ConstructExample("H");
      int n = a.getX();
      System.out.println(n);
   }
}


```
  
  ### 앞서 코드에 보이는 것 처럼 this()는 클래스 안에서 생성자를 호출한다.
  
 
 



