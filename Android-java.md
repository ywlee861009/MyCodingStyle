# Android Java Coding Style

## 1. 주석 스타일
### 1-1. 클래스 최상단 주석

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
*         .setListener(CustomAlertDialog.listener)
*         .build()
*         .show();
* 
* @auther YWLee
*/
public class CustomAlertDialog {
  ...
}
</code></pre>
