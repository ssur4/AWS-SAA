---
tags:
  - AWS
---

- ==투명하고 변경 불가능하며 암호화 방식==으로 ==검증 가능한 트랜잭션 로그를 제공==하는 ==완전관리형 원장 데이터베이스==이다.
- ==애플리케이션 데이터의 모든 변경 사항을 추적==하고, 
  ==시간 경과에 따른 완전하고 검증 가능한 변경 기록을 유지==할 수 있습니다.


#### **주요 특징**

- ==**변경 불가능한 저널**==
	- Amazon QLDB는 추가 전용 저널을 사용하여 ==모든 데이터 변경 사항을 정확하고 순차적으로 기록==한다.
	- ==이 저널은 데이터를 덮어쓰거나 삭제할 수 없으므로== ==저장된 변경 기록이 삭제되거나 수정되지 않음을 보장==한다.

- ==**암호화 검증**==
	- QLDB는 ==암호화를 사용하여 데이터 변경 기록의 무결성을 확인할 수 있는 다이제스트를 생성==한다.
	- 이를 통해 ==데이터의 변경 이력이 의도치 않게 수정되지 않았음을 검증==할 수 있다.

- ==**서버리스 아키텍처**==
	- QLDB는 ==완전관리형 서버리스 서비스==이다.
		- 인스턴스나 용량을 프로비저닝할 필요가 없다.
	- ==인프라 관리 없이 애플리케이션의 수요에 따라 자동으로 확장==됩니다.

- ==**SQL 호환 쿼리**==
	- QLDB는 ==PartiQL==이라는 ==SQL 호환 쿼리 언어를 지원==한다.
	- 관계형, 반구조화 및 중첩된 데이터에 대한 SQL 호환 액세스를 제공한다.


#### **사용 사례**

- **금융 거래 기록**
	- 신용 및 직불 거래와 같은 모든 금융 거래의 완전하고 정확한 레코드를 생성하여 데이터의 무결성을 보장한다.

- **공급망 추적**
	- 각 거래 이력을 기록하고, 제조에서 판매까지의 모든 배치의 세부 정보를 제공하여, 
	  공급망의 투명성을 높인다.

- **청구 기록 유지**
	- 청구의 전체 수명을 추적하고 암호화 방식으로 데이터 무결성을 확인하여, 
	  데이터 입력 오류 및 조작으로부터 애플리케이션의 복원력을 유지한다.