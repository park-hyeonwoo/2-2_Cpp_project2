inf_int 클래스

< 멤버 변수 >
- char* digits: 숫자를 뒤집어서 저장 
- unsigned int length: 숫자의 길이를 나타냄
- bool thesign: 숫자의 부호를 나타냄 (양수면 true, 음수면 false)

< 생성자 >
- inf_int(): default 값 0
- inf_int(int): int형으로 입력받을 경우
- inf_int(const char*): 문자열로 입력받을 경우
- inf_int(const inf_int&): 복사 생성자

< 함수 >
- operator=: 지정 연산자
- operator==: 두 수가 같으면 true, 다르면 false를 반환
- operator!=: 두 수가 다르면 true, 같으면 false를 반환
- operator>: 첫번째 수가 두번째 수보다 크면 true, 아니면 false를 반환
- operator<: 두번째 수가 첫번째 수보다 크면 true, 아니면 false를 반환
- operator+: 두 수를 더함. (Add함수 이용) 부호가 같으면 +연산자로, 다르면 -연산자로 연산
- operator-: 앞의 수에서 뒤의 수를 뺌. (Sub함수 이용) 부호가 같으면 -연산자로, 다르면 +연산자로 연산
- operator*: 두 수를 곱함. 각 자릿수를 곱한 값을 알맞은 index에 Add함수를 이용하여 더해줌 
- operator<<: 숫자를 출력
- Add: 지정된 자릿수에 수를 더함. index의 크기만큼 동적 할당을 해주고 자리 올림이 발생하면 윗자리에 1을 더함
- Sub: 지정된 자릿수에서 수를 뺌. index의 크기만큼 동적 할당을 해주고 자리 내림이 발생하면 윗자리에서 1을 뺌
