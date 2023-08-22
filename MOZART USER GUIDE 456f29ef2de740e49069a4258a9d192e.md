# MOZART USER GUIDE

[MOZART 개요](MOZART%20USER%20GUIDE%20456f29ef2de740e49069a4258a9d192e.md)

- **INSTALLATION**
    
    
    [                                                   SYSTEM REQUIREMENTS](MOZART%20USER%20GUIDE%20456f29ef2de740e49069a4258a9d192e/SYSTEM%20REQUIREMENTS%2042b598adef744aec80e0b2c408696d44.md)
    
    [                                                   MOZART Client 설치](MOZART%20USER%20GUIDE%20456f29ef2de740e49069a4258a9d192e/MOZART%20Client%20%E1%84%89%E1%85%A5%E1%86%AF%E1%84%8E%E1%85%B5%20028971ea4876457a97ab29e9d3aa85d2.md)
    
    [                                      MOZART Client 설치(MOZART .NET)](MOZART%20USER%20GUIDE%20456f29ef2de740e49069a4258a9d192e/MOZART%20Client%20%E1%84%89%E1%85%A5%E1%86%AF%E1%84%8E%E1%85%B5(MOZART%20NET)%20840a70aed15b41ab9c2f6ee7ab542ced.md)
    
    [                                      MOZART Server 설치](MOZART%20USER%20GUIDE%20456f29ef2de740e49069a4258a9d192e/MOZART%20Server%20%E1%84%89%E1%85%A5%E1%86%AF%E1%84%8E%E1%85%B5%2050d990553c6141da849684e4b55d578c.md)
    
    [                                      라이선스 인증 방법](MOZART%20USER%20GUIDE%20456f29ef2de740e49069a4258a9d192e/%E1%84%85%E1%85%A1%E1%84%8B%E1%85%B5%E1%84%89%E1%85%A5%E1%86%AB%E1%84%89%E1%85%B3%20%E1%84%8B%E1%85%B5%E1%86%AB%E1%84%8C%E1%85%B3%E1%86%BC%20%E1%84%87%E1%85%A1%E1%86%BC%E1%84%87%E1%85%A5%E1%86%B8%20b1d8771d8ddf4b6f92093b02eab09132.md)
    
    [                                      MOZART 라이선스 키 요청 방법](MOZART%20USER%20GUIDE%20456f29ef2de740e49069a4258a9d192e/MOZART%20%E1%84%85%E1%85%A1%E1%84%8B%E1%85%B5%E1%84%89%E1%85%A5%E1%86%AB%E1%84%89%E1%85%B3%20%E1%84%8F%E1%85%B5%20%E1%84%8B%E1%85%AD%E1%84%8E%E1%85%A5%E1%86%BC%20%E1%84%87%E1%85%A1%E1%86%BC%E1%84%87%E1%85%A5%E1%86%B8%204524970204494d30931de1466caa8daa.md)
    
- **GETTING STARTED**
    
    [                                      Hello World Example](MOZART%20USER%20GUIDE%20456f29ef2de740e49069a4258a9d192e/Hello%20World%20Example%204f56b73e1ffb4e58a63816accfa5791b.md)
    
    [                                      Simple ETL Example](MOZART%20USER%20GUIDE%20456f29ef2de740e49069a4258a9d192e/Simple%20ETL%20Example%2016606cbdebee4516a31519c24076a493.md)
    

---

## MOZART 개요

MOZART (Manufacturing Operation Zone on Abstract Real Time) 는 제조시스템의 운영에 필요한 Plan & Schedule 을 수립하고 모니터링 할 수 있는 Application 개발에 최적화된 개발/운영 도구 및 Library 제품 전체를 의미합니다. MOZART 제품은 다음과 같이 구성됩니다.

---

### **MOZART IDE(Integrated Development Environment)**

Visual Studio Package 형태로 제공되는 MOZART IDE 는 다양한 종류의 대량 Data 를 Input 으로 받아 복잡한 Logic 을 빠른 속도로 처리한 후, Output 을 생성하는 방식의 시스템 개발에 적합한 요소로 구성됩니다. 즉, Batch Data Processing 을 수행하는 시스템 개발용 도구입니다. 예로서 제조시스템의 생산계획 및 스케줄 처리, 대용량 Data 의 ETL(Extract, Transform, Load) 과 같은 응용시스템을 보다 쉽게 개발할 수 있도록 도움을 줍니다. C# 기반의 OOP 프로그램의 경우 객체기반의 개발 방식과 특성을 잘 이해하고 있어야 개발이 용이한 반면, MOZART 를 활용한 개발은 Data 와 Logic 을 분리하여 보다 직관적인 코딩이 가능하도록 구성되어 있습니다. 또한 MOZART SEEPLAN Library 의 Pegging, Simulation Module 과의 연동을 통해 제조업의 Planning, Scheduling 시스템을 효과적으로 개발할 수 있습니다.

### **MOZART Studio**

MOZART IDE 를 통해 개발된 Model 을 사용자 입장에서 조회하고 Model 의 실행조건 및 입력 Data 를 변경하여 실행시켜 볼 수 있는 최종 사용자용 MOZART 실행 환경입니다. 또한, Model 의 Logic 실행 결과를 분석할 수 있는 UI 를 개발하여 MOZART Studio 에 Embed 할 수 있어 MOZART 제품의 UI Container 역할도 함께 수행합니다.

- **MOZART Library** : MOZART Library 는 제조업의 생산계획과 생산스케줄링 시스템 구축 시 사용되며, MOZART IDE 와 통합하여 Flow 기반의 제품 개발 관리에 용이한 구조로 구성된 Library 제품입니다. MOZART Library 제품은 아래와 같은 두 가지 제품군으로 구분됩니다. 각 Library 는 IDE 와 통합되어 사용되는 전용 UI 를 포함합니다.
- **Basic Library** : 제품별 Demand 를 충족시키는 공정별 일별 생산 목표를 생성하기 위한 Backward Planning Library (Pegging Library) 와 공정/장비별 로딩 Simulation 을 통한 생산계획, 일정계획 수립용 Forward Planning Library (Loading Simulation Library) 로 구성됩니다.
- **Domain Library** : 반도체 FAB, 반도체 B/E, LCD FAB/Module, 타이어 등과 같이 특정 제조 Domain 에 특화된 Plan & Schedule 기능요소를 포함한 Library 제품입니다.

### **MOZART Management Console**

MOZART IDE 로 개발된 결과물은 Dll 형태로 MOZART Studio 및 MOZART Server 를 통해 실행 될 수 있습니다. MOZART Management Console (MMC) 은 MOZART Server 에 개발 결과를 실행시킬 수 있는 Job 을 생성하고 실행방식 (Schedule) 을 정의하며 실행을 모니터링하는 등의 Server 관리 도구입니다. 시스템의 개발 및 테스트 단계에서는 MOZART IDE 와 MOZART Studio 를 통해 작업을 수행할 수 있지만, 운영단계에서는 일정 주기나 조건에 따라 시스템이 실행되어야 하며, 실행결과의 모니터링이 중요해집니다. MMC 는 이러한 Server 를 통한 MOZART 기반 시스템 운영 업무 지원 도구입니다. MOZART (.NET Framework) 제품은 설치형 Application 형태로 제공하며, MOZART .NET 제품은 웹 브라우저를 통해 서버에 접속하는 형태로 제공됩니다.

### **MOZART Server**

MOZART Server 는 MOZART IDE 를 통해 개발된 Plan & Schedule Job 을 등록하여 조건 (Time Schedule, Condition) 에 따라 자동으로 실행시켜 주는 Server 제품입니다. 특정 사이트 내의 최종 사용자용 제품 (MOZART Studio) 의 Local License Server 역할을 병행할 수 있습니다.

ON THIS PAGE

  

 **[MOZART IDE](MOZART%20USER%20GUIDE%20456f29ef2de740e49069a4258a9d192e.md)** 

  [MOZART Studio](MOZART%20USER%20GUIDE%20456f29ef2de740e49069a4258a9d192e.md)

   **[MOZART  Management Console](MOZART%20USER%20GUIDE%20456f29ef2de740e49069a4258a9d192e.md)** 

    **[MOZART Server](MOZART%20USER%20GUIDE%20456f29ef2de740e49069a4258a9d192e.md)**