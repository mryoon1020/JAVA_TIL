# JAVA

- Work space 생성
  - File - New - JAVA Project
  
- Package
  - 좌측 파일 목록에서 SRC 우클릭 - New - Package
  - 모두 소문자로 사용
  
- Class
  - 좌측 파일 목록에서 SRC 우클릭 - New - Class(메인여부에 따라 메인 체크)
  - 첫글자는 대문자 사용
  
- Method
  - 객체 동작에 해당하는 {}
  - 첫글자는 소문자로 시작(관례상)
  
- 변수

  * 데이터를 보관하는 장소(ex, int a : 정수형 변수 a)
  * 변수선언(ex, int a =10;)

- System.out

  - 교육하며 정말 자주쓰는 명령어

  - 지정된 서식으로 화면에 보여주는 역할

  - System.out.print() : 괄호 속 내용 단순 출력, 행을 띄지 않음

  - System.out.println() : 괄호 속 내용 단순 출력, 행을 띄움, syso + ctrl + space bar 하면 바로 입력가능

  - System.out.printf() : 서식을 지정하여 출력

  - 서식 종류

    | 서식문자 | 내용                                 |
    | -------- | ------------------------------------ |
    | \n       | 새로운 줄로 이동 (Enter키랑 같음)    |
    | \t       | 다음 텝으로 이동 (Tab키와 같으)      |
    | \b       | 뒤로 한칸 이동 (Back Space키와 같음) |
    | \r       | 줄의 맨앞으로 이동(Home키와 같음)    |
    | \\\      | \출력                                |
    | \\\'     | '출력                                |
    | \\"      | "출력                                |

    

    | 서식      | 내용                        |
    | --------- | --------------------------- |
    | %b        | boolean 형식으로 출력       |
    | %d        | 정수형식으로 출력           |
    | %0        | 8진수 정수의 형식으로 출력  |
    | %x  or %X | 16진수 정수의 형식으로 출력 |
    | %f        | 소수점 형식으로 출력        |
    | %c        | 문자형식으로 출력           |
    | %s        | 문자열 형식으로 출력        |
    | %n        | 줄바꿈 기능                 |
    | %e or %E  | 지수 표현식의 형식으로 출력 |

    ``` 
    public class Ex03_02 {
    
    	public static void main(String[] args) {
    				
    		System.out.printf("%d",100,200);
    		System.out.printf("%d",200,200,400);//변수의 갯수와 상관없이 서식이
    		System.out.printf("%d",300,200,500,6000);// 입력된 만큼만 표시
    		
    		System.out.printf("\n");//줄바꿈
    		System.out.printf("%d %d",100);//오류, 서식 갯수와 출력 숫자 갯수가 반드시 일치 
    		System.out.printf("%d %d",100,200);//오류 X 100 200 출력
    		System.out.printf("\n");
    		System.out.printf("%d,%d",300,400);//오류 X ',', 300, 400 출력
    		System.out.printf("\n");
    		
    			}
    
    }
    ```

    ```
    public class Test {
    
    	public static void main(String[] args) {
    		
            int num = 202201231;
            double score = 77.7;
            
            System.out.printf("학번이 %d인 학생의 점수는 %f입니다.", num, score);
            //지정된 서식 위치에 변수가 들어가며 문자열은 그대로 프린트 됨
    
    	}
    
    }
    ```

