[사용방법 guide]
- 최초 사용시 필수 사전 작업

1. VScode 설치
2. Python 설치
3. Git 설치

4. VScode내에서 Ctrl + Shift + P → 'Python Select interpreter' click → 설치한 Python 경로로 interpreter setting 완료 (잘 모르면 googling)
(만약 검색이 되지 않는다면 vscode extensions (단축키 : Ctrl+Shift+x에서 python 검색 후 install 필요)

5. VScode에서 터미널 띄우기 (Ctrl + ` (tab키 위에 있는))

6. code를 돌릴 위치로 이동 
cd code를 돌릴경로 입력후 Enter치면 이동.
ex) cd C:\Windows  → 입력

7. git clone https://github.com/Jin-Kwon-Lee/COSCO_SR.git

8. pip install -r requirements.txt 명령어 입력
9. pip install error 나는경우 고급 환경 설정에서 PATH에 pip 위치를 입력해서 인식되도록 해야 함.
아래 링크 참고
https://joy-notes.com/vscode-%ED%8C%8C%EC%9D%B4%EC%8D%AC-pip-%EC%84%A4%EC%B9%98-%EC%9C%88%EB%8F%84%EC%9A%B0%EC%9A%A92022%EB%85%84-%EA%B8%B0%EC%A4%80/

내컴퓨터 >> 속성 >> 고급시스템설정 >> 고급탭 >> 환경변수 >> Path변수 편집  >> 새로만들기
"C:\Users\user\AppData\Local\Programs\Python\Python312\Scripts"  (보통 다음과 같은 경로에 있음. 참고로 AppData는 폴더에서 숨김처리되어 있어 직접입력하는게 좋음) >> 확인후 VScode 재실행

10. 8번 다시 재실행


- 최초 사용이 아닐 경우
1. input_data file에 넣고 싶은 data를 모두 가져온다. (전체 data : Ctrl + Shift + space +end)
주요 column명은 "반드시" 변경되지 않도록 한다. column밑에 값으로 복사를 하여
col에 맞게 value가 들어갔는지 1차로 확인한다.

2. 저장 한 후 input data file을 종료한 뒤, VScode terminal 창에서 "py run.py" or  "python run.py" 명령어를 입력하여 실행한다.

3. result_data.xlsx 를 열어 첫번째 sheet는 무시하고 다음 BL num로 되어있는 sheet의 data의 결함이 있는지 확인한다.

