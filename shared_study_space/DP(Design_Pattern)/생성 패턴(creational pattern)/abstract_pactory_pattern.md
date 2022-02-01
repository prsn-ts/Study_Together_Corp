# 디자인패턴/ 생성 패턴(Creational Pattern)

## 추상 팩토리(Abstract Pactory)

### 1. 추상 팩토리 패턴이란?
- 서로 연관이 있는 객체들을 묶어서 팩토리 클래스로 만들고 이 팩토리 클래스들을 조건에 따라 생성하기 위해 다시 팩토리를 만들어(추상의 개념) 객체를 생성하는 패턴
<br>

### 2. 구성 요소
- AbstractFactory: 팩토리 클래스의 공통 인터페이스
- ConcreteFactory: 구체적인 팩토리 클래스로 AbstractFactory 클래스의 추상 메소드를 오버라이드하여 구체적인 객체를 생성
- AbstractProduct: 제품의 공통 인터페이스
- ConcreteProduct: 구체적인 팩토리 클래스에서 생성되는 구체적인 제품
<br>

### 3. 사용 예시
