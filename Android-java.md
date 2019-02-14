# Android Java Coding Style

## 1. 주석 스타일
### 1-1. class 최상단 주석
#### A. 자동으로 만들어지는 주석은 사용하지 않는다.
<pre><code>
/**
* Created by YWLee 2019-01-01
*/
public class CustomAlertDialog {
  ...
}
</code></pre>

#### B. 다음과 같은 포맷으로 주석을 활용한다.
<pre><code>
/**
* (기능,역할 - 필수)
* (사용 방법 - 선택)
* 
* @auther (작성자)
*/
public class CustomAlertDialog {
  ...
}
</code></pre>

##### Example
<pre><code>
/**
* 커스텀 얼럿 다이얼로그 생성
* 사용법 :
*   new CustomAlertDialog.Builder(Context)
*         .withMessage(String)
*         .withTitle(String)
*         .buttonType(CustomAlertDialog.TWO_BUTTON)
*         .setSubmitListener(CustomAlertDialog.listener)
*         .build()
*         .show();
* 
* @auther YWLee
*/
public class CustomAlertDialog {
  ...
}
</code></pre>


### 1-2. method 상단 주석
#### A. method 에는 다음과 같은 포맷으로 주석을 단다.

<pre><code>
/**
* (기능,역할 - 필수)
*
* @param seq 회원의 순서
*
* @return seq 를 계산하여 회원의 이름을 리턴함
*/
public String getClientName4Seq(int seq) {
  ...
}
</code></pre>


<hr />


## 2. Method 코딩 스타일
### 2-1. Method Parameters
#### A. Parameter 가 3개 이상일 경우 라인을 구분하여 코딩한다.
##### Ex a. 1 parameters
<pre><code>
/**
* ...함수 주석
*/
public void testFunc(String a) {
  //...
}
</code></pre>
##### Ex b. 3 parameters
<pre><code>
/**
* ...함수 주석
*/
public void testFunc(String a,
                  String b,
                  int c) {
  //...
}
</code></pre>

### 2-1. call method
#### A. 마찬가지로, method 호출 시 Parameter 가 3개 이상인 경우 다음과 같이 호출한다.
<pre><code>
String test1 = "test1";
int test2 = 2;
float test3 = 3.2f;

callMethod(test1,
          test2,
          test3);
</code></pre>







<pre><code>
</code></pre>
