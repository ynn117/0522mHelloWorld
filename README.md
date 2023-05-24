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

|  **옵션**  | **설명** |
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

# PS

![image](https://github.com/ynn117/0522mHelloWorld/assets/133843571/27e0bf55-0d40-4135-a818-89553ee52e36)

**-명령어는 현재 실행중인 프로세스 목록을 보여준다.**

**-비정상적인 프로세스가 올라왔는지 확인함.**

**-리눅스 관리 전반적으로 많이 사용되는 명령어**

(주로 파이프라인, grep명령어와 함께 사용하여 특정 프로세스를 확인하는데 많이 사용됨)

## 실행 후 명령어

|  **옵션**  | **설명** |
|----------|-----------------------|
| -e | 모든 프로세스를 출력함 |
| -f | 풀 포맷으로 보여줌(UID, PID 등) |
| -l | 긴 포맷으로 보여줌 |
| p,-p | 특정 PID의 프로세스를 보여줌 |
| -u | 특정 사용자의 프로세스를 보여줌 |

**-ps 상태-**

* USER: 프로세스 소유자의 USERNAME (BDS 계열)
* UID: 프로세스 소유자의 USERNAME (SYSTEM V 계열)
* PID: 프로세스 식별번호
* %CPU: CPU 사용비율
* %MEM: 메모리 사용비율

# jobs

![image](https://github.com/ynn117/0522mHelloWorld/assets/133843571/008bc81f-0bb7-4887-a221-f025b1d23405)

**-실행중인 백그라운드 목록 출력**

# 실행 후 명령어

|  **옵션**  | **설명** |
|----------|-----------------------|
| -e | 각 프로세스 ID에 대해 한 행씩 출력 |
| -n | 프로세스 그룹 중에 표 프로세스 ID를 출력 |
| -l | 프로세스 그룹 ID를 state 필드 앞에 출력 |
| -S | 백그라운드에 있는 프로세스 중 멈춰있는 프로세스만 출력|
| command | 지정한 명령어를 실행 |

# 상태

|  **상태**  | **설명** |
|----------|-----------------------|
| Running | 작업이 계속 진행중임 |
| Done | 작업이 완료되어 0을 반환 |
| Done(code) | 작업이 종료되었으며 0이 아닌 코드를 반환 |
| Stopped | 작업이 일시 중단 |
| Stopped(SIGTSTP) | SIGTSTP 시그널이 작업을 일시 중단 |
| Stopped(SIGSTOP) | SIGSTOP 시그널이 작업을 일시 중단 |
| Stopped(SIGTTIN) | SIGTTIN 시그널이 작업을 일시 중단 |
| Stopped(SIGTTOU) | SIGTTOU 시그널이 작업을 일시 중단 |

# Kill
