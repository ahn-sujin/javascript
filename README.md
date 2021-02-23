# JAVASCRIPT
javascript study

## About
* javascript 공부를 기록하는 저장소입니다. 

## Contact
:envelope: asj9674@gmail.com 

# JAVASCRIPT에 관하여 

## 1. 데이터타입 - 문자열과 숫자 

### 1-1. 데이터타입 종류 
* Boolean 
* Null
* Undefined
* Number (숫자)
* String (문자열)
* Symbol

### 1-2. String(문자열)
* 문자는 ""('')사용 
* .length  문자열의 갯수를 알려줌 
* .toUpperCase( ) 대문자 알파벳으로 변경 
* .indexOf( ) 문자의 위치를 찾아줌 
* .trim( ) 공백을 없애줌  

## 2. 변수와 대입 연산자 
* x(변수) =(대입연산자)  1 ;
* 대입연산자 : 좌항과 우항을 결합해서 우항의 값을 만들어 낸다.  
* 1(상수)=2;    -> 성립되지 않는 수식 
* varibale(변수)  vs  constant(상수) 
* 실행 = enter  / 실행유보 = shift + enter 
* 변수 사용할 때 앞에 'var' 붙여서 사용 할 것 ex) var name ="sujin" ;
* 변수 사용의 이유: 방대한 자료 속 특정한 문자를 변수를 이용하여 정확하고 빠르게 바꿀 수 있다.

## 3. 제어할 태그 선택하기 
* javascript select tag by css selector


  :  element = document .querySelector(selectors);


  ex) var el = document .querySelector(".myclass");
      

* javascript element style


 : var x = document .getElementById("myH1").style;
      

* javascript style background-color


  : document.body.style.backgroundColor="red";
      

## 4. 프로그램, 프로그래맹, 프로그래머 
* HTML: 프로그래밍 언어(X), 시간에 순서에 구애 받지 않는다 
* JAVASCRIPT : 프로그래밍 언어(0), 사용자와의 상호작용, 시간의 순서에 따라 실행
* 프로그램 : 순서 
* 프로그래밍 : 순서를 만드는 행위 -> 반복적인 일을 하지 않아도 됨
* 프로그래머: 순서를 만드는 사람 

## 5. 조건문 
* 조건문: 조건에 따라 다른 순서의 기능들이 실행 되도록 함 -> 복잡한 일을 해결

## 6. 비교 연산자와 블리언 
### 6-1. === (비교 연산자)
   ex) 1 === 1   : true    /  1===2  : false

### 6-2. true / false (블리언) 
   html '<'  은  '&lt;' 로 표현한다 

## 7. 조건문 
<pre>
<code>
document .write("1");
if (true){
      document.write("2");
}    else  {
     document.write("3");
}
document.write("4");	
</code>
</pre>


===> if (  true or false  ) {  A  } else { B  }   
* if 절의 값이 true 일 때, else 조건문(B) 이 생략 되고, 
* if 절의 값이 false 일 때, if 조건문(A) 이 생략 된다. 

## 8. 조건문의 활용 
* javascript element get value


  : document.querySelector('selector' ).value;
  
## 9. 리팩토링 중복의 제거 
* 리팩토링: 비효울적인 코드를 효율적으로 만들어 가독성을 높이고 유지보수가 쉽도록 코드를 개선 

### 9-1. this: 이벤트가 속해 있는 자신을 가르킴 (따로 id, class명을 설정하지 않아도 됨)
<pre>
<code>
<input id="night_day" type="button" value="night" onclick="
    if(document.querySelector('#night_day').value ==='night'){
    document.querySelector('body').style.backgroundColor='black';
    document.querySelector('body').style.color='white';
    document.querySelector('#night_day').value='day';
    } else {
    document.querySelector('body').style.backgroundColor='white';
    document.querySelector('body').style.color='black';
    document.querySelector('#night_day').value='night';
    }
">
</code>
</pre>

<pre>
<code>
 <input  type="button" value="night" onclick="
    if(this.value ==='night'){
    document.querySelector('body').style.backgroundColor='black';
    document.querySelector('body').style.color='white';
    this.value='day';
    } else {
    document.querySelector('body').style.backgroundColor='white';
    document.querySelector('body').style.color='black';
    this.value='night';
    }
 ">
</code>
</pre>

* 코딩을 잘하는 tip : 중복되는 코드 제거!

### 9-2. 중복되는 코드 이름 설정 
<pre>
<code>
<input  type="button" value="night" onclick="
    if(this.value ==='night'){
    document.querySelector('body').style.backgroundColor='black';
    document.querySelector('body').style.color='white';
    this.value='day';
    }
    ">
</code>
</pre>

<pre>
<code>
 <input  type="button" value="night" onclick="
   var target = document.querySelector('body');	
    if(this.value ==='night'){
    target.style.backgroundColor='black';
    target.style.color='white';
    this.value='day';
    }
    ">
</code>
</pre>

## 10. 배열(Array)
*  [ "값1", "값2" ]

  index 0 = 값1
  
  index 1 = 값2

* javascript array count 

  : var fruits = ["Banana" , "Orange" , "Apple", "Mango"]; fruits.length;
  
* javascript array add data

  : var fruits = ["Banana" , "Orange" , "Apple", "Mango"]; fruits.push("Kiwi");
  
## 11. 반복문(Loop)
* 반복문: 순서대로 흐르는 순서문의 흐름을 제어 
* while(ture / false ){     코드   } 

  : ( ) 안에 값이 false가 될 때까지 { } 안에 코드 들이 실행 됨, ( ) 안에 값이 false가 되면 
  
*  while문 :  바깥에 코드가 실행됨. (반복문 종료)
*  var i  = 0; : 실행 코드가 몇번 실행 됐는지 적는 코드  



  
  
  





  


              














 
