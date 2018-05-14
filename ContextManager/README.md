개요
로봇 지능 프레임워크는 변화하는 환경에 대한 상황 인식 정보를 관리 할 수 있어야 한다. 이 때 변화하는 환경을 관측하고 얻어낸 상황 정보들을 관리하는 모듈이 바로 ContextManager이다. 

ContextManger는 PerceptionManger로부터 얻어진 센서 데이터 정보를 이용하여 KnowRob과 Arbi 지식 베이스 기반으로 상황 정보를 저장 및 관리한다. 더하여  TaskManger의 요청에 따라 Swi-prolog를 이용한 복합 추론을 통해 요청된 상황 정보를 응답 기능을 수행한다.  

기능
ContextManger는 TaskManger로부터 요청받은 상황 정보들을 송신하기 위하여 저장된 저수준의 상황정보들로부터 상황 정보 서술자를 이용한 추론을 통해 고수준의 상황 정보를 TaskManager에게 전달한다.  

모델
ContextManger의 상황 서술자 목록은 다음과 같다. 
상황 서술자는 크게 각 클래스의 속성 정보를 추론해내는 속성 서술자(attribute predicate)와 클래스와 클래스 간에 관계를 나타내는 관계 정보를 추론해내기 위한 관계 서술자(relationship predicate)로 나뉜다. 
