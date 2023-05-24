# TOP

![image](https://github.com/ynn117/0522mHelloWorld/assets/133843571/d58e57ba-03a8-49f8-b916-0329b6f21b48)

**-현재 실행되고 있는 프로세스에 관한 정보를 출력하는 명령어**

**-시스템의 상태를 전반적으로 가장 빠르게 파악 가능**

**-3초 간격으로 화면을 갱신하며 정보를 보여줌**

![image](https://github.com/ynn117/0522mHelloWorld/assets/133843571/1ece01a1-91bf-42c9-9109-3f56272a882f)

* 시스템 현재시간: 15:18:09
* 서버 구동시간: 172
* 현재 접속 유저수: 5
* 로드 에버리지(1분 , 5분, 15분 동안 시스템 부하량 평균값)

# tasks
![image](https://github.com/ynn117/0522mHelloWorld/assets/133843571/79a3dec9-0a10-449b-9199-1c77f3866be0)

* Tasks: 현재프로세스들의 상태
* total: 전체프로세스 수
* running: 실행중 수
* sleeping: 대기중 수
* stoppde: 종류 수
* zombie: 좀비 수

# CPU사용량
![image](https://github.com/ynn117/0522mHelloWorld/assets/133843571/dafe681b-10f2-4c3d-a21e-294e9c1678f7)
* us: 사용자 프로세스
* sy: 커널 프로세스
* ni: 프로세스 우선순위
* id: 사용안하는 비율
* wa: IO완료기다리는 비율
* si: 소프트웨어 인터럽트
* st: VM에 할당된 비율(st)을 출력

# 메모리양
![image](https://github.com/ynn117/0522mHelloWorld/assets/133843571/df67261b-5579-4439-822c-42bd2e605d3c)

* total: 총 메모리 양
* free: 사용가능 메모리 양
* used: 사용중 메모리 양
* buff/cache: 커널 버퍼 사용메모리 양 
* avail Mem: 물리적 메모리 양


## @top 실행 후 명령어

|  **명령어**  | **설명** |
|----------|-----------------------|
| shift + p | CPU 사용률 내림차순 |
| shit + m | 메모리 사용률 내림차순 |
| shift + t | 프로세스가 돌아가고 있는 시간 순 |
| k | kill. k 입력 후 PID 번호 작성. signal은 9 |
| f | sort field 선택 화면 -> q 누르면 RES순으로 정렬 |
| a | 메모리 사용량에 따라 정렬 |
| b | Batch 모드로 작동 |
| 1 | CPU Core별로 사용량 보여줌 |

# 프로세스 상태

* SHR 옆에 있는 S 항목으로 볼 수 있음
*  D : Uninterruptiable sleep. 디스크 혹은 네트워크 I/O를 대기
* R : 실행 중(CPU 자원을 소모)
* S : Sleeping 상태, 요청한 리소스를 즉시 사용 가능
* T : Traced or Stopped. 보통의 시스템에서 자주 볼 수 없는 상태
* Z : zombie. 부모 프로세스가 죽은 자식 프로세스



