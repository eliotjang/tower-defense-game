## 프로젝트 소개

대학생 두 명이서 협력하여 2개월간 Unity 엔진을 사용하여 제작한 타워 디펜스 장르의 게임

## 스크린샷

![](https://eliotjang.github.io/assets/images/defense-game/TD-demo.png) 

## 게임 로직 구현

- 클리어시 다음 스테이지 이동 및 금화 획득
  - [WaveSpawner.cs](https://github.com/eliotjang/tower-defense-game/blob/eliot/Assets/Scripts/WaveSpawner.cs)
- 일반 및 보스 몬스터 소환 및 이동 경로
  - [Enemy.cs](https://github.com/eliotjang/tower-defense-game/blob/eliot/Assets/Scripts/Enemy.cs)
  - [WalkInCircles.cs](https://github.com/eliotjang/tower-defense-game/blob/eliot/Assets/Scripts/WalkInCircles.cs)
  - [WayPoints.cs](https://github.com/eliotjang/tower-defense-game/blob/eliot/Assets/Scripts/Waypoints.cs)
- 타워 포탄 발사 및 몬스터 포탄 유도
  - [Tower.cs](https://github.com/eliotjang/tower-defense-game/blob/eliot/Assets/Scripts/Tower.cs)
  - [Bullet.cs](https://github.com/eliotjang/tower-defense-game/blob/eliot/Assets/Scripts/Bullet.cs)
- 확률형 스킬 구매 및 스킬 이펙트 및 데미지 처리
  - [DamageWithSkill.cs](https://github.com/eliotjang/tower-defense-game/blob/eliot/Assets/Scripts/Skills/DamageWithSkill.cs)
  - [RandomSkilRate.cs](https://github.com/eliotjang/tower-defense-game/blob/eliot/Assets/Scripts/Skills/RandomSkillRate.cs)
  - [SkillEffect.cs](https://github.com/eliotjang/tower-defense-game/blob/eliot/Assets/Scripts/Skills/SkillEffect.cs)
- 시각적으로 간단한 UI/UX
  - [LiveUI.cs](https://github.com/eliotjang/tower-defense-game/blob/eliot/Assets/Scripts/UI/LivesUI.cs)
  - [Money.cs](https://github.com/eliotjang/tower-defense-game/blob/eliot/Assets/Scripts/UI/MoneyUI.cs)
  - [TextFadeIn.cs](https://github.com/eliotjang/tower-defense-game/blob/eliot/Assets/Scripts/UI/TextFadeIn.cs)

## 게임 규칙 및 플레이 방법

- 한 라운드당 몬스터는 20마리이다.
	- 라이프는 40으로 설정한다. 
	- 필드의 몬스터의 개수만큼 라이프는 감소해서 보여진다.
	- 열 라운드마다 몬스터와 함께 필드보스가 등장한다. (몬스터 20마리 + 필드보스 1마리)
- 한 라운드당 시간제한은 30초이다. 단, 필드의 몬스터가 없으면 바로 다음 라운드로 진행된다.
	- 라운드가 끝나기 전까지 필드보스를 잡지 않아도 패배하지 않는다.
	- 일반 몬스터는 한 바퀴를 돌 때마다 방어력이 1씩 오른다.
	- 초기 골드는 0골드이고 스킬을 구매하는 비용은 1500골드이다.
	- 스킬을 판매시, 1000골드를 획득할 수 있다.
- 라운드 시작전, 스킬의 구매와 환불은 골드가 소모되지 않는다. 단, 최대 2번까지 가능하다.
- 일반 몬스터를 잡으면 1골드를, 필드 보스를 잡으면 1000골드를 획득할 수 있다.
- 스킬의 최대 개수는 4개이다.
- 스킬의 등급은 F~S등급까지 존재한다.
- 스킬을 구매할 때 등급은 랜덤으로 정해진다.

## 기술 스택 및 학습 내용

### 언어 및 기술 스택
- C#
- Unity
- Unity Collaboration

### 학습 내용
- 게임 개발 과정의 A to Z
- Unity 게임 제작 기초
- 코드 리뷰를 통한 구현 능력 향상
- 팀원과의 협업 도구 활용

## 참고자료

- [워크래프트3 : 리포지드 유즈맵 랜덤능력타워디펜스](https://myiro.tistory.com/247)
