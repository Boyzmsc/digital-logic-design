# 논리 회로 설계 (Quiz_1)

x1 - 열 확인 (열 감지 센서 이용)
x2 - 기침 증상 (통과할 때 해당인원에게 질문 조사)
x3 - 호흡기 증상 (호흡곤란, 목아픔 등 질문 조사)A - 80% 예상 확신 (검역소, 방역대 호출, 해당 인원에게 통보)
B - 20~80% 확신 (임시 관리 인원으로 등록, 해당 인원에게 자가격리 권고요청, 간단한 신상정보만 검역소에 전달)
C - 0~20% 확신 (통과시킴, 손씻기*마스크 착용 자동 음성안내)논리식 :
A = x1 * (x2 + x3)
-> 발열 + 호흡기 증상(기침 포함) 있는 즉시 코로나 의심환자라고 가정
B = x1' * (x2 + x3)
-> 발열은 없지만 호흡기 증상이 있을 시 임시 관리 인원으로 등록 가정
C = x1' * x2' * x3'
-> 위 증상들 다 없을 시 통과시킴

시스템 기능 설정은 약간의 과장을 포함하고 있습니다
감사합니다.