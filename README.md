# Cerberus x
- 20190726 교육시간에 배운 내용을 정리
<br><br>
## 생각나는대로 적기
* import mojo : 기본 라이브러리
* class [이름] Extend App : app의 기능을 상속시켜주는 것
'''
클래스와 인스턴스, 인터페이스, 추상객 <br>
* 인터페이스 : 클래스에 필요한(정의된) 요소들
* 추상객체 : 클래스와 인터페이스의 중간단계. 반반?인얘 (대략 이렇게 생겻어! 설명도 애매하고 그림도애매쓰....)
(나중에 제대로 정리해서 수정 바람)
'''

## short notation
* boolean ?
* integer %
* float #
* string $

## 너무 헷깔리는 Declarations (class App)
* OnCreate - must call SetUpdateRate
<br> [SetUpdateRate 숫자]를 반드시 넣어야함. 숫자는 초당 루프 수.
* OnUpdate - can use mojo input commands <br>
* OnRender - can use mojo drawing commands

> OnUpdate는 업데이트 타이머가 체크 표시를 할 때 호출되며 게임 로직 코드가 실행되어야 하는 위치입니다. 업데이트 타이머는 SetUpdateRate 기능을 사용하여 설정됩니다.

> OnRender는 응용 프로그램이 자체적으로 렌더링될 때 호출됩니다. 업데이트 타이머를 체크하는 경우 OnUpdate 후에도 가능한 한 빨리 호출되지만 일반적으로 응용 프로그램을 새로 고쳐야 하는 경우 언제든지 OnRender가 호출될 수 있습니다.

> OnUpdate는 일반적으로 개체 및 게임 상태를 업데이트하는 데 사용되며 OnRender는 그래픽을 그리는 데 사용됩니다

>> 1 -> (2->3) : 괄호는 반복된다.

* 게임에서 무한 루프는 기본이다!


## Graphics
### Draw
* DrawPoint x, y : x, y에 점을 찍는다.
* DrawImage [이름], x, y
* DrawText "hello", x, y
### Function
* Function SetColor : Int ( r:Float, g:Float, b:Float ) : 현재 색상 설정


## ~문들
* if else
'''python
If 조건
    진술
ElseIf 조건
    진술
Else
    진술
EndIF
'''

* Select(switch)
'''python
Select Expression
Case Expression [, Expression...]
    진술
Default
    진술
End
'''

* while
'''python
While Expression
    진술
Wend
'''

* Repeat
'''python
Repeat
    진술
Until Expression  [or Forever]
'''

* For
'''python
For [ Local ] IndexVariable = FirstValue To | Until LastValue [ Step StepValue ]
     Statements...
Next
'''

* (Exit == break) && continue
