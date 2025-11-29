## HW2.write_README
#### [과제2] README 파일 작성하기 (top, ps, jobs, kill)
----

# ***1. top (실시간 프로세스 모니터링)***

  - 개념 :       
      - 현재 시스템의 CPU, 메모리, 프로세스 상태를 실시간 갱신하여 보여주는 명령어
  
  - 정보 :   
    | 항목 | 설명 |
    |-----|-----|
    | load average | 실행/대기 프로세스 수의 평균 |
    | %CPU / %MEM | CPU/메모리 점유율 |
    | RES / VIRT | 실제/가상 메모리 |
    | TIME+ | 프로세스 실행 누적 시간 | 
  
  - 옵션 :
    | | 옵션 | 설명 |
    |-----|-----|-----|
    |1| -o < 컬럼 > | 정렬 기준 변경 (%CPU / %MEM / PID...) |
    |2| -p < PID > | 특정 PID(프로세스 하나)만 모니터링 |
    |3| -d < 초 > | 새로고침 시간 간격 조절 |
  
    - 예시 :    
         
      (1) -o %MEM : 메모리 많이 쓰는 순으로 정렬     

        `top -o %MEM`     
        ![-o 옵션](images/top/top(-o)_option.PNG)    

      (2) -p 1 : "PID 1"만 모니터링

        `top -p 1`      
        ![-p 옵션](images/top/top(-p)_option.PNG)    

      (3) -d 2 : 2초마다 갱신

        `top -d 2`     
        ![-d 옵션](images/top/top(-d)_option.PNG)    



# ***2. ps (현재 실행 중인 프로세스 확인)***

  - 개념 : 
    - 현재 실행 중인 프로세스를 "정적인 상태"로 한 번 출력
    - top처럼 실시간 갱신 X
  
  - 옵션 :
    | | 옵션 | 설명 |
    |-----|-----|-----|
    |1| a | 모든 사용자 프로세스 |
    |2| u | 사용자 중심 상세 출력 |
    |3| x | 터미널 없는 프로세스 포함 |
    |4| -e | 전체 프로세스 출력 |
    |5| -f | full format (부모 PID 등 표시) |
    |6| --forest | 프로세스 트리 구조 출력 |
  
    - 예시 :    
         
      (1) aux : 모든 프로세스 보기     

        `ps aux`    
        ![aux 옵션](images/ps/ps(aux)_option.PNG)    

      (2) -p 1 : 부모-자식 관계 트리 구조 출력

        `ps -ef --forest`       
        ![-ef --forest옵션](images/ps/ps(-ef_--forest)_option.PNG)    


 
# ***3. jobs (현재 터미널 세션의 백그라운드 작업 확인)***

  - 개념 : 
    - 현재 실행 중인 프로세스를 "정적인 상태"로 한 번 출력
    - top처럼 실시간 갱신 X
  
  - 옵션 :
    | | 옵션 | 설명 |
    |-----|-----|-----|
    |1| a | 모든 사용자 프로세스 |
    |2| u | 사용자 중심 상세 출력 |
    |3| x | 터미널 없는 프로세스 포함 |
    |4| -e | 전체 프로세스 출력 |
    |5| -f | full format (부모 PID 등 표시) |
    |6| --forest | 프로세스 트리 구조 출력 |
  
    - 예시 :    
         
      (1) aux : 모든 프로세스 보기     

        `ps aux`    
        ![aux 옵션](images/ps/ps(aux)_option.PNG)    

      (2) -p 1 : 부모-자식 관계 트리 구조 출력

        `ps -ef --forest`       
        ![-ef --forest옵션](images/ps/ps(-ef_--forest)_option.PNG)    









