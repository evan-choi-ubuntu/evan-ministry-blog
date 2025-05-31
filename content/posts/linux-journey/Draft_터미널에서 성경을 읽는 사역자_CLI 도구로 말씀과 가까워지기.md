# 터미널에서 성경을 읽는 사역자: CLI 도구로 말씀과 가까워지기

*2025년 5월 29일 - 세 번째 이야기*

---

## 세 번의 각성, 하나의 여정

[첫 번째 글](링크)에서 나는 MSX 8비트 컴퓨터의 검은 화면에서 시작된 낭만을 잃고, 화려한 클라우드 생태계에 지쳐 우분투로 돌아온 이야기를 했다.

[두 번째 글](링크)에서는 Word와 Notion을 버리고 마크다운과 Obsidian으로 설교문을 작성하게 된 실용적 이유들을 나누었다.

이제 세 번째 이야기다. 그 검은 터미널 화면에서 **하나님의 말씀을 읽는다는 것**에 대해.

---

## 그날 밤, 터미널 앞에서

우분투 설치 후 며칠이 지난 어느 저녁이었다. 설교 준비를 위해 성경을 펼쳐야 했는데, 문득 이런 생각이 들었다.

*"내가 MSX 시절 그렇게 그리워했던 그 검은 화면... 거기서 성경을 읽을 수는 없을까?"*

Firefox를 열어 온라인 성경을 보려다가 멈췄다. 그 화려한 웹사이트들, 광고 배너들, 복잡한 인터페이스들이 갑자기 너무 피곤하게 느껴졌다.

그래서 터미널을 열었다.

```bash
evan@ubuntu:~$ apt search bible
```

---

## CLI 성경의 발견

검색 결과에 나타난 것들을 보고 나는 깜짝 놀랐다.

### **1. Bible.Org CLI**
```bash
sudo apt install bible-kjv
```

설치 후 실행해보니:

```bash
evan@ubuntu:~$ bible
Welcome to the Bible reader!
Type 'help' for commands.

bible> John 3:16
John 3:16 - For God so loved the world, that he gave his only 
begotten Son, that whosoever believeth in him should not 
perish, but have everlasting life.

bible> search love
Searching for 'love'...
Found 442 verses containing 'love'
```

### **2. BibleTime CLI**
더 고급 기능을 원해서 설치한 또 다른 도구:

```bash
sudo apt install bibletime
```

### **3. Bible Gateway CLI (Python)**
```bash
pip install bible-gateway
bg John 3:16
```

그런데 이 모든 도구들을 사용하면서 느낀 것은... **단순히 도구의 편리함이 아니었다**.

---

## 검은 화면 위의 하얀 글자, 그 거룩함

터미널에서 성경을 읽기 시작하면서 경험한 것들:

### **1. 온전한 집중**
```bash
bible> Romans 8:28
Romans 8:28 - And we know that all things work together 
for good to them that love God, to them who are the called 
according to his purpose.
```

화려한 GUI도, 광고도, 알림도 없었다. 오직 **검은 화면과 하얀 글자뿐**. [첫 번째 글에서 그리워했던](링크) 그 MSX의 단순함이 거기 있었다.

브라우저에서 성경을 읽을 때는 항상 다른 탭들이 신경 쓰였다. 메일 알림, 유튜브 추천, 소셜미디어... 하지만 터미널에서는 **오직 말씀만 있었다**.

### **2. 직접적인 대화**
```bash
bible> search "be still"
Psalm 46:10 - Be still, and know that I am God: I will be 
exalted among the heathen, I will be exalted in the earth.
```

마치 하나님과 일대일로 대화하는 느낌이었다. 중간에 끼어드는 광고도, 화려한 디자인도 없이 **순수한 텍스트로 된 하나님의 말씀**과 마주하는 경험.

### **3. 검색의 순수함**
웹사이트에서 성경을 검색할 때는 항상 무언가 다른 것들이 함께 나타난다. 관련 기사, 추천 영상, 광고... 하지만 CLI에서는:

```bash
bible> search "fear not"
Found 63 verses containing 'fear not'

Isaiah 41:10 - Fear thou not; for I am with thee: be not 
dismayed; for I am thy God: I will strengthen thee; yea, 
I will help thee; yea, I will uphold thee with the right 
hand of my righteousness.

Isaiah 43:1 - But now thus saith the LORD that created thee, 
O Jacob, and he that formed thee, O Israel, Fear not: for 
I have redeemed thee, I have called thee by thy name; 
thou art mine.
```

**순수한 검색 결과만** 나타난다. 검색하고자 했던 바로 그 말씀들만.

---

## 설교 준비가 또 다시 변했다

[두 번째 글에서 설명했듯이](링크), 마크다운과 Obsidian으로 설교 준비 시간이 30% 단축되었다고 했다. 그런데 터미널 성경까지 더해지니 더욱 놀라운 일이 일어났다.

### **Before: 웹 기반 성경 연구**
1. 브라우저 열기 (로딩 시간)
2. 성경 사이트 접속 (광고 로딩)
3. 원하는 구절 검색
4. 여러 번역본 비교를 위해 탭 여러 개 열기
5. 관련 구절 찾기 위해 또 다른 검색
6. 산만한 환경에서 집중력 분산
7. 중요한 구절들 복사해서 메모장에 정리

**총 소요 시간: 약 25분**

### **After: 터미널 + Obsidian 연동**
1. 터미널에서 즉시 구절 검색
```bash
bible> John 3:16
```
2. 관련 구절 즉시 검색
```bash
bible> search "eternal life"
```
3. 중요한 구절들을 바로 Obsidian 노트에 기록
```bash
bible> John 3:16 >> /srv/admin_hub/성경연구/영생.md
```
4. 온전한 집중 상태에서 묵상
5. Obsidian에서 `[[요한복음3장16절]]` 링크 생성

**총 소요 시간: 약 12분**

**52% 시간 단축!** 하지만 더 중요한 것은 **집중도의 향상**이었다.

---

## 나만의 CLI 성경 연구 워크플로우

몇 달간의 시행착오를 거쳐 정착된 나만의 방법:

### **1. 매일 아침 묵상 루틴**
```bash
# 6:30 AM - 하루를 터미널로 시작
evan@ubuntu:~$ cd /srv/admin_hub/묵상일기
evan@ubuntu:묵상일기$ bible

bible> random verse
Proverbs 3:5-6 - Trust in the LORD with all thine heart; 
and lean not unto thine own understanding. In all thy ways 
acknowledge him, and he shall direct thy paths.

# 즉시 오늘의 묵상 파일 생성
bible> exit
evan@ubuntu:묵상일기$ vim 2025-05-29-잠언3장5-6절.md
```

### **2. 설교 본문 연구**
```bash
# 이번 주 설교 본문이 로마서 8장이라면
bible> Romans 8
# 전체 장 읽기

bible> search "Spirit" Romans 8
# 로마서 8장 내에서 "성령" 관련 구절 찾기

bible> cross-reference Romans 8:28
# 교차 참조 구절들 확인
```

### **3. 주제별 연구**
```bash
bible> search "love" | head -20
# "사랑" 관련 구절 상위 20개

bible> search "love" Gospel
# 복음서에서만 "사랑" 검색

bible> concordance love
# "사랑"에 대한 성경 사전 정보
```

---

## 기술과 영성의 만남: 더 깊은 의미

터미널에서 성경을 읽는 것이 단순히 **도구의 선택**을 넘어 **영성의 차원**에서 가져다준 변화들:

### **1. 디지털 금식의 은혜**
웹브라우저의 모든 유혹들로부터 벗어나 **순수한 텍스트와 마주하는 시간**. 이것은 마치 광야에서 하나님과 만나는 경험과 같았다.

### **2. 명령어와 기도의 유사성**
```bash
bible> search "comfort"
```
이런 명령어를 입력할 때마다 느끼는 것은, 이것이 마치 **하나님께 구하는 기도**와 같다는 것이다. 

"하나님, 위로에 대한 말씀을 보여주세요."

그리고 즉시 응답이 온다:
```
2 Corinthians 1:3 - Blessed be God, even the Father of our 
Lord Jesus Christ, the Father of mercies, and the God of 
all comfort;
```

### **3. 검은 화면의 영성**
[첫 번째 글에서 언급했듯이](링크), 나는 화려한 GUI에 지쳐 단색 텍스트를 그리워했다. 터미널의 검은 화면은 **묵상과 기도를 위한 성소**가 되었다.

외부의 모든 자극을 차단하고, 오직 하나님의 말씀과 나 사이의 **거룩한 정적** 속에서 만나는 시간.

---

## 실용적 팁들

몇 달간의 경험을 통해 정리한 터미널 성경 읽기 팁들:

### **1. 필수 설치 도구들**
```bash
# KJV 성경 (기본)
sudo apt install bible-kjv

# 히브리어/그리스어 도구
sudo apt install biblical-hebrew

# 성경 사전
sudo apt install bible-dict

# 교차 참조 도구
pip install bible-cross-reference
```

### **2. 유용한 단축키 설정**
```bash
# ~/.bashrc에 추가
alias morning="bible random"
alias study="bible search"
alias verses="bible"

# 빠른 검색을 위한 함수
biblesearch() {
    bible search "$1" | head -10
}
```

### **3. Obsidian 연동 자동화**
```bash
# 중요한 구절을 자동으로 Obsidian에 저장
bible_to_obsidian() {
    echo "## $(date '+%Y-%m-%d %H:%M')" >> /srv/admin_hub/성경구절모음.md
    bible "$1" >> /srv/admin_hub/성경구절모음.md
    echo "" >> /srv/admin_hub/성경구절모음.md
}
```

### **4. 묵상 일기 자동화**
```bash
# 매일 아침 묵상 파일 생성
morning_devotion() {
    DATE=$(date '+%Y-%m-%d')
    FILE="/srv/admin_hub/묵상일기/${DATE}-묵상.md"
    
    echo "# ${DATE} 묵상" > "$FILE"
    echo "" >> "$FILE"
    echo "## 오늘의 말씀" >> "$FILE"
    bible random >> "$FILE"
    echo "" >> "$FILE"
    echo "## 묵상과 기도" >> "$FILE"
    echo "" >> "$FILE"
    
    vim "$FILE"
}
```

---

## 공동체와의 나눔

혼자만의 경험으로 끝내지 않고, 교회 청년들과도 나누기 시작했다.

### **청년부 성경공부 혁신**
```bash
# 청년부 모임에서
"오늘은 '사랑'에 대해 공부해봅시다."

# 프로젝터로 터미널 화면 공유
bible> search "love" Gospel | head -5

# 실시간으로 관련 구절들이 나타나는 것을 보며
# 청년들의 집중도가 확연히 달라졌다
```

**청년들의 반응:**
- "와, 성경이 데이터베이스 같아요!"
- "이렇게 빠르게 찾을 수 있다니..."
- "스마트폰보다 집중이 잘 돼요"

### **설교 중 실시간 검색**
설교 도중에도 터미널을 활용:
```bash
# 설교 중에 갑자기 관련 구절이 생각날 때
bible> search "peace" | grep Jesus
```
즉시 관련 구절을 찾아 회중과 나눌 수 있게 되었다.

---

## 오픈소스 정신과 성경의 만남

이 모든 과정에서 깨달은 것은 **오픈소스 정신과 성경의 공통점**이었다.

### **무료로 공개된 하나님의 말씀**
```bash
bible> John 3:16
# 이 명령어로 나오는 구절은 완전히 무료다
# 구독료도, 광고도 없다
```

하나님의 말씀이 **"값없이 받았으니 값없이 주라"**는 원칙처럼, 터미널의 성경 도구들도 모두 무료로 제공된다.

### **투명하고 단순한 접근**
웹사이트의 복잡한 인터페이스나 상업적 목적이 개입되지 않은, **순수한 텍스트로서의 하나님의 말씀**.

### **전 세계 개발자들의 헌신**
이 CLI 도구들을 만든 개발자들은 **아무런 대가 없이** 하나님의 말씀을 더 쉽게 접할 수 있도록 헌신했다. 이것이야말로 진정한 **디지털 선교**가 아닐까?

---

## 지금도 계속되는 여정

[첫 번째 글의 MSX 추억](링크)에서 시작되어, [두 번째 글의 마크다운 전환](링크)을 거쳐, 이제 터미널에서 성경을 읽는 이 세 번째 여정까지.

모든 것이 하나로 연결되어 있다:

- **단순함에 대한 그리움** → 터미널의 검은 화면
- **진정한 소유권에 대한 갈망** → 로컬에 저장된 성경 텍스트  
- **연결된 지식에 대한 열망** → CLI 도구들과 Obsidian의 만남
- **복음적 가치와의 일치** → 오픈소스 정신과 "값없이 주라"는 말씀

---

## 매일 아침의 고백

이제 매일 아침 터미널을 열며 이렇게 기도한다:

```bash
evan@ubuntu:~$ bible

bible> random verse
```

어떤 구절이 나올지 모르지만, 그 **검은 화면 위의 하얀 글자**들을 통해 하나님이 오늘 내게 주시는 말씀을 기다린다.

MSX 앞에서 꿈꿨던 그 순수한 기대감이, 이제는 **하나님의 말씀을 향한 갈망**으로 승화되었다.

---

## 마무리: 계속 이어질 이야기

이 시리즈는 여기서 끝나지 않는다. 

다음에는 **Git으로 설교문을 버전 관리하는 이야기**, **Hugo로 교회 웹사이트를 만든 경험**, **AI 도구들을 사역에 접목한 시행착오들**...

모든 이야기가 하나의 큰 주제로 연결되어 있다:

**"기술과 복음이 만나는 지점에서, 어떻게 더 순수하고 효과적으로 하나님을 섬길 것인가?"**

MSX에서 시작된 여정이 계속되고 있다. 그리고 이 여정의 끝에는 분명 **더 아름다운 사역의 모습**이 기다리고 있을 것이다.

---

*"주의 말씀은 내 발에 등이요 내 길에 빛이니이다" (시편 119:105)*

```bash
evan@ubuntu:~$ bible Psalm 119:105
Psalm 119:105 - Thy word is a lamp unto my feet, and a light unto my path.

evan@ubuntu:~$ # 오늘도 주님의 말씀으로 시작합니다.
```

*이 글은 Ubuntu 22.04의 터미널에서 vim으로 작성되었으며, bible-kjv와 Obsidian을 연동하여 완성되었습니다. 모든 CLI 도구 설정법과 스크립트는 Creative Commons 라이선스로 공유됩니다.*

---

**다음 글 예고**: "Git으로 설교문을 버전 관리하는 사역자: 하나님의 말씀도 커밋한다"