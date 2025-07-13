# KAIST PintOS Week 1–3

## KAIST PintOS란?
PintOS는 교육용 운영체제 프로젝트로, 매주 주차별로 다양한 OS 개념을 C 언어로 직접 구현하며 학습합니다.  
*주차별 구현 목표는 [GitBook](https://casys-kaist.github.io/pintos-kaist/)에서 확인할 수 있습니다.*

## 해당 과정을 통해 얻은 것
- OS 핵심 개념을 깊이 이해하고, C 언어로 직접 구현해 보며 확실히 체득했습니다.  
- 40,000줄 이상의 오픈소스 코드를 읽고 구현, 디버깅할 영역을 빠르게 파악하는 능력을 기를 수 있었습니다.  
- AWS Ubuntu 환경 설정 및 디버깅 워크플로우를 익혔습니다.  

## 주차별 구현 내용

### Week 1: Scheduling
- 스케줄러 구조 및 우선순위 기반 스케줄링 구현  
- 타이머 인터럽트 빈도 조절 문제 해결: `timer_sleep()` 함수 보완  
- 우선순위 기아 현상 해결을 위한 Priority Donation 구현  
- MLFQS (Multi-Level Feedback Queue Scheduler) 구현  

### Week 2: System Call
- 20개 이상의 시스템 콜 인터페이스 설계 및 구현 (`halt`, `exit`, `exec` 등)  
- 멀티스레드 환경에서 시스템 콜 동시성 문제 방지를 위한 락(lock) 처리  

### Week 3: Virtual Memory
- 페이징 기초, 페이지 테이블 관리 및 Page Fault 처리 구현  
- 메모리 배열과 페이지 특성을 고려하여 메모리 할당 로직 구현  
- LRU 기법 기반 페이지 교체 알고리즘 구현  
- 메모리 할당 실패 시 예외 처리 구현  

## 개념 및 시행착오 정리
### Week 1: Scheduling
- **Link**
  - [timer.c 함수 정리 및 sleep 기능 구현](https://scientific-string-9e5.notion.site/KraftonJungle-Day54-PintOS-Week1-timer-c-sleep-13063eaa9930807bb4efedf7a0f49dea?pvs=74)
  - [Process, Thread, Context Switching, MLFQS 개념 정리](https://scientific-string-9e5.notion.site/KraftonJungle-Day57-PintOS-Week1-Process-Thread-Context-Switching-MLFQS-13163eaa993080c4a9e6c39a1a6fe204?pvs=74)
  - [Semaphore, Mutex, Condition Variable, Race Condition, Deadlock 개념 정리](https://scientific-string-9e5.notion.site/KraftonJungle-Day58-PintOS-Week1-Semaphore-Mutex-Condition-Variable-Race-Condition-Deadlock-13463eaa993080f2ad8ccc6ed570147b?pvs=74)
  - [PintOS Priority Scheduling 구현(1)](https://scientific-string-9e5.notion.site/KraftonJungle-Day59-PintOS-Week1-PintOS-Priority-Scheduling-1-13563eaa993080a39da7dbb7d1b7f813?pvs=74)
  - [PintOS Priority Scheduling 구현(2)](https://scientific-string-9e5.notion.site/KraftonJungle-Day59-PintOS-Week1-PintOS-Priority-Scheduling-2-13663eaa993080a59d04f07ffe4caa9f?pvs=74)
  - [MLFQS 구현](https://scientific-string-9e5.notion.site/KraftonJungle-Day61-PintOS-Week1-MLFQS-13863eaa993080b693e3d6a9fde76702?pvs=74)
### Week 2: System Call
- **Link**
  - [개념 정리 및 User Programs - Argument Passing 구현](https://scientific-string-9e5.notion.site/KraftonJungle-Day66-PintOS-Week2-User-Programs-Argument-Passing-13c63eaa993080a4b59ce9f282a34765?pvs=74)
  - [User Programs - System Call 구현](https://scientific-string-9e5.notion.site/KraftonJungle-Day68-User-Programs-System-Call-13e63eaa993080c0bd70e97d3045af09)
  - [User Programs - File Manipulation 구현](https://scientific-string-9e5.notion.site/KraftonJungle-Day68-PintOS-Week2-User-Programs-File-Manipulation-14263eaa993080debd51d9bde0673609?pvs=74)
### Week 3: Virtual Memory
- **Link**
  - [페이징 및 가상 메모리 개념 정리](https://scientific-string-9e5.notion.site/KraftonJungle-Day74-PintOS-Week3-14963eaa993080228fa5c3570a037732?pvs=74)
 

<!--

**Here are some ideas to get you started:**

🙋‍♀️ A short introduction - what is your organization all about?
🌈 Contribution guidelines - how can the community get involved?
👩‍💻 Useful resources - where can the community find your docs? Is there anything else the community should know?
🍿 Fun facts - what does your team eat for breakfast?
🧙 Remember, you can do mighty things with the power of [Markdown](https://docs.github.com/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
-->
