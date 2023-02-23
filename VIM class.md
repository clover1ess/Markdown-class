# <span style ='color:yellow; background-color:green'>**Vim Class**</span>

## <span style='color:black; background-color:orange;'>**Insert / Normal / Visual / Visual line**</span>
* Insert mode - 작성모드, 영/한 상관없이 명령모드로 넘어갈 수 있음
* Normal mode - 명령모드, 명령어 모두 사용 가능, Esc로 가능, 작성모드로 넘어갈 땐 i키로 가능  
* Visual mode - 복사 모드, 이 상태에선 단어, 문장 등 세밀하게 복사 가능, 소문자 v로 가능  
* Visual line - 줄복사 모드, 해당 줄 복사 바로 가능, 대문자 V키로 가능 

## <span style='color:#000000; background-color:orange;'>**행 이동**</span>
- 기본적으로 h, j, k, l로 상하좌우 이동 가능하다. 
- 단어 기준은 b(이전 단어 첫글자로), w(다음 단어 첫글자로), e(다음 단어 마지막 글자로)
- 문장 기준은 0(앞으로), $(뒤로), H(보이는 화면 맨 위로), M(보이는 화면 중간으로), L(보이는 화면 아래로)
- 행 이동은 행 번호를 친 후 gg or G를 입력하면 그 행의 첫 번째 글자로 이동. Ctrl e = 스크롤 다운, Ctrl u = 스크롤 업 
- Ctrl y = 해당 칸의 마우스포인터를 옮기지 않고 스크롤 업

## <span style='color:black; background-color:orange;'>**문장 & 단어 지우기**</span>

- 명령, 복사, 줄복사 모드 셋 다 d,c로 지울 수 있다. 
- 명령모드에서는 cc를 누르면 입력모드로 돌아간다. 
- 단어기준으로 dw(단어 지우기), daw(공백 포함해서 지우기), diw(공백 제외해서 지우기)가 가능하며, vwc, vwd와 같은 명령어도 가능하다. 
- 문장기준으로 Vd or Vc, cc와 같은 명령어가 가능하다. 
- 행, 파일 기준 V(원하는 페이지)gg or G, v ii c or d로 삭제 가능하다.
- 지우는 건 다양한 방식들이 있어서 자신이 편한 방식으로 할 수 있으며, 몇 줄, 어디까지 지우는 것을 편하게 할 수 있으므로 많이 다뤄보는 것이 좋다. 
드래깅
- 복사모드 or 줄복사 모드로 전환 후 원하는 만큼(단어 기준 or 행 기준)으로 드래깅 한다. 
- v ii는 그 파일의 전체 텍스트를 드래깅한다.(단, 줄복사 모드에서는 불가능) 
- v + $ or v + 0는 각각 파일 뒤쪽 또는 앞쪽 드래깅 하는 것. 
- 복사모드 or 줄복사 모드 둘 다 h,j,k,l과 같은 기본 행 이동 기능이 가능하다.  
- Shift + r -> 그 문장 바꾸기, r만 눌러서 한 단어만 바꾸기 가능<br>
## <span style='color:black; background-color:orange;'>**복사**</span>

- 명령모드, 복사모드, 줄복사 모드 셋 다 y로 복사 가능하다. 
- 기본적으로 VIM은 삭제가 곧 Ctrl x의 기능을 갖고 있다. 즉, cc or d만으로도 삭제와 동시에 복사가 가능하다.  
- 복사, 줄복사 모드는 d로 삭제 시 명령모드, c로 삭제 시 입력 모드로 돌아간다.  

## <span style='color:black; background-color:orange;'>**붙여넣기**</span>

- 어떤 모드이든 p로 가능하다. 
- 복사에서 했던 삭제를 p로 붙여넣기가 가능하다. 
- 문장 다시 쓰기 -> shift r or s로 그 문장의 앞부터 다시 쓸 수 있다.(단, 칸 수는 유지가 되며, 고치는 동안에도 그 칸 수가 동일하다.)
- shift + r에서는 영어 한글 둘 다 전환해가며 쓸 수 있다. 대신에 전환해서 썼을 때 띄어쓰기가 잘 안보일 수 있다.  
## <span style='color:black; background-color:orange;'>**파일 다루기**</span>

* Ctrl 1,2,3 (작업페이지 생성 / 페이지는 총 8개까지 생성 가능) / Ctrl w (작업페이지 삭제) 
* Ctrl n or Alt f n (파일 새로 생성), Ctrl F4 (작업페이지에서 파일 삭제), Ctrl shift p로는 markdown 관련 작업 가능 
* Ctrl shift e (파일 탐색기 열기), Ctrl p (파일 검색하기)
* Ctrl shift s or ZZ(다른 이름으로 저장하기), Ctrl s or :w (저장하기), :wqa (저장하면서 모든 페이지 닫기)
- 단, 파일 저장할 때 다른 이름으로 바꾸면 이전에 저장한 파일과 같이 둘 다 저장되어 있다. 
- 이용 가능한 파일 - html, md, txt, png, jpg, mp3, ini, js 등 
- 이용 불가능한 파일 - pdf, jfif, word, 한컴 등 

## <span style='color:black; background-color:orange;'>**이 수업을 일반인이나 개발자가 써야하는 이유?**</span>

- Vim이 좋은 프로그램인 건 알지만 다른 문서작업 프로그램이 더 익숙하다면 그걸 쓰는 게 훨씬 더 좋을 것이다.  

## <span style='color:black; background-color:orange;'>**일반인의 경우**</span>

- 일단 마우스 없이 편하게 명령어만을 이용하여 사용 가능
- markdown파일로 만들 경우 노션처럼 제작해서 프린팅을 할 수 있다. 즉, PDF파일로 전환해서 인쇄까지도 가능하다.  
- 일반인도 개발자인 척(?) 할 수 있다. 

## <span style='color:black; background-color:orange;'>**개발자의 경우**</span> 

- 소, 중, 대괄호 내의 글자를 빠르게 지우고 변환하고, 반복되는 코드는 .을 이용해서 복제할 수 있다. 
- IDE보단 IDE + Vim을 하면 훨씬 더 생산성이 늘어나는 건 확실하다.(VSCode와 Vim이 매우 잘 맞는다.)
- 자신에게 최적화된 개발 환경 구축이 된다. 