# Codyssey_Native_Basic_1-2

[Intro]
---
## Step 1: 미션을 수행할 AI 모델을 선정한다.

|AI모델|평가축|배점|
|:---:|:---:|:---:|
|GPT|형식/톤제어|5|
||정보정확성|5|
||속도|3|
|Gemini|형식/톤제어|3|
||정보정확성|3|
||속도|1|
|Claude|형식/톤제어|5|
||정보정확성|5|
||속도|5|

결론: GPT로 결과물을 도출하고 Claude로 검증/비교 작업을 진행하겠다.
<details><summary> 미션 실행 가이드 펼치기 </summary>

  ```
        # 미션 통합 가이드: AI 브랜드 광고 제작 프로젝트
    > GPT와 Claude의 답변을 비교·보완하여 실행 순서대로 재구성한 최종 가이드
    
    ---
    
    ## 🎯 미션 한 줄 요약
    **"가상(또는 실제) 브랜드의 광고 영상(10초 이내)을 AI 도구만으로 만들고, 그 기획·제작 과정을 스토리보드 문서(PDF)로 정리해서 제출하는 과제"**
    
    너는 이번 미션에서 **"광고 기획자 + AI 오퍼레이터"** 역할을 맡게 됩니다.
    
    ## 📦 최종 제출물 = 2가지
    | 구분 | 내용 | 형식 |
    |---|---|---|
    | ① 설계도 | 스토리보드 문서 | PDF |
    | ② 완성품 | 브랜드 광고 영상 | MP4 (10초 이내) |
    
    ---
    
    # Step 1. 브랜드 기획하기
    
    먼저 광고할 브랜드를 하나 정합니다. 실제 브랜드도, 가상 브랜드도 가능합니다.
    
    **정해야 할 항목**
    - 브랜드 이름
    - 타겟(누구를 위한 브랜드인가)
    - 톤앤매너(분위기)
    - USP (다른 브랜드와 다른 차별점)
    
    **예시**
    - 브랜드명: MoonTea
    - 타겟: 공부하는 10대
    - 톤앤매너: 따뜻함, 감성적, 편안함
    - USP: "집중할 때 마시는 감성 차"
    
    ---
    
    # Step 2. 캠페인 목표 & 핵심 메시지 정하기
    
    이 광고를 **왜** 만드는지 정합니다.
    
    - 브랜드를 처음 알리기 위해서인지
    - 제품 구매를 유도하려는 것인지
    - 기존 고객의 재방문을 유도하려는 것인지
    
    그리고 이를 압축한 **핵심 메시지 1문장**을 작성합니다.
    
    > 예: "지친 공부 시간, MoonTea 한 잔으로 마음을 쉬게 하세요."
    
    ---
    
    # Step 3. 씬(Scene)별 스토리보드 작성하기
    
    영상을 장면 단위로 나눠서 계획표를 만듭니다. **각 씬마다 아래 항목을 전부 채워야 합니다.**
    
    - [ ] 씬 번호
    - [ ] 씬 길이(몇 초)
    - [ ] 이 장면이 전달할 메시지
    - [ ] 화면 구성 (인물 유무, 배경, 자막 여부 등)
    - [ ] 내레이션 또는 화면 카피 문구
    - [ ] 사용할 AI 도구 종류 (이미지/영상/오디오)
    - [ ] 그 도구를 고른 이유
    - [ ] 실제 입력한 프롬프트 원문
    - [ ] 생성 결과 한 줄 요약
    - [ ] 생성된 파일명 또는 링크
    
    > ⚠️ 영상 전체가 아니라 **씬 단위 계획**이 먼저입니다. 이 계획표가 이후 Step 5(프롬프트 생성) 작업의 기준이 됩니다.
    
    **스토리 구조는 둘 중 하나를 반드시 만족해야 합니다.**
    
    | 방법 | 구조 |
    |---|---|
    | A. 짧은 이야기 구조 | 문제 제시 → 변화/전환 → 해결·제안 |
    | B. 명확한 메시지 전달 | 누구에게 → 어떤 가치를 주는지가 분명히 드러남 |
    
    **영상 마지막 3~5초에는 아래 중 1개 이상 반드시 포함:**
    - 로고 / 브랜드명 / 슬로건 / CTA(예: "지금 만나보세요")
    
    ---
    
    # Step 4. AI 도구 선정하기
    
    **필수: 아래 3종류를 각각 1개 이상 사용**
    
    | 용도 | 도구 예시|
    |---|---|
    | 이미지 생성 | Midjourney, DALL·E, Leonardo |
    | 영상 생성/변환 | Runway, Pika, Kling |
    | 오디오 생성 | Suno, ElevenLabs, 기타 TTS |
    
    - 그림만 AI로 만들고 소리는 사람이 넣는 방식은 **불가** → 소리도 AI 기반이어야 함
    - 도구별로 **대체 도구**를 하나씩 미리 정해두는 것을 추천 (대기열 지연, 크레딧 부족 등 대비)
    
    ---
    
    # Step 5. 프롬프트 작성 및 생성 실행
    
    Step 3의 계획표를 기준으로 씬마다 실제 AI에 프롬프트를 입력해 결과물(이미지/영상/오디오)을 생성합니다.
    
    - 프롬프트 원문은 그대로 기록해둘 것 (문서 제출용)
    - 결과물 파일명을 씬 번호와 매칭해 관리 (예: scene1_bg.png, scene1_va.mp3)
    
    ---
    
    # Step 6. 프롬프트 수정 전/후 비교 기록하기 (필수 최소 1개)
    
    Step 5 과정에서 **적어도 한 장면 이상**은 프롬프트를 고쳐본 과정을 기록해야 합니다.
    
    - [ ] 처음 프롬프트
    - [ ] 무엇이 문제였는지
    - [ ] 어떻게 수정했는지
    - [ ] 수정 후 결과가 어떻게 좋아졌는지
    
    > 👉 "그냥 만들었다"가 아니라 "생각하고 개선했다"는 과정을 보여주는 항목입니다.
    
    ---
    
    # Step 7. 편집 및 영상 합치기
    
    Step 5에서 만든 이미지/영상/오디오 결과물을 편집 프로그램으로 이어붙여 하나의 영상으로 완성합니다.
    
    **편집 프로그램(Premiere Pro, CapCut 등)은 아래 용도로만 사용 가능(보조용)**
    - 컷 자르기 / 이어붙이기
    - 자막 삽입
    - 색감 미세 조정
    - 소리 크기 조절
    
    **절대 금지 사항**
    - ❌ 직접 촬영한 영상 사용
    - ❌ 유료 스톡 영상 사용
    - ❌ 딥페이크, 혐오·선정성·폭력성 높은 콘텐츠
    - ❌ 핵심 그림/소리 자체를 편집 프로그램으로 새로 제작 (반드시 AI 생성 결과물이어야 함)
    
    **최종 영상 조건 재확인**
    - 길이 10초 이내 / MP4 형식
    - AI 시각 요소(이미지 or 영상) 포함
    - AI 청각 요소(BGM, 효과음, 음성 중 최소 1개) 포함
    
    ---
    
    # Step 8. 스토리보드 문서(PDF) 정리하기
    
    Step 1~6에서 정리한 내용을 하나의 PDF 문서로 종합합니다.
    
    **문서 구성 순서**
    1. 브랜드 설명 (Step 1)
    2. 캠페인 목표 + 핵심 메시지 (Step 2)
    3. 씬별 계획표 전체 (Step 3, 5 결과 포함)
    4. 프롬프트 수정 전/후 비교 (Step 6)
    5. 사용 도구 목록 + 대체 도구 (Step 4)
    
    ---
    
    # Step 9. 최종 점검 체크리스트
    
    **제출 1: PDF 문서**
    - [ ] 브랜드 설명 있음
    - [ ] 광고 목표 있음
    - [ ] 핵심 메시지 1문장 있음
    - [ ] 씬별 정보(번호/길이/메시지/화면구성/카피/도구/이유/프롬프트/결과요약/파일명) 모두 기재
    - [ ] 사용 도구와 선택 이유 기재
    - [ ] 프롬프트 수정 전/후 최소 1개 기재
    
    **제출 2: MP4 영상**
    - [ ] 10초 이내
    - [ ] AI로 만든 이미지/영상 포함
    - [ ] AI로 만든 소리 포함
    - [ ] 스토리 구조(A 또는 B) 성립
    - [ ] 마지막 3~5초에 브랜드 요소 노출
    
    ---
    
    # Step 10. 제출하기
    
    완성된 PDF 문서와 MP4 영상 파일 두 개를 제출합니다.
    
    ---
    
    # ➕ 보너스 (선택 사항)
    
    - 인물 등장 장면에 립싱크 적용
    - 동일한 스토리보드를 다른 AI 도구 조합으로 재제작해보기
    - 화면 비율을 여러 개로 제작 (유튜브 16:9 / 숏폼 9:16 / 인스타 피드 1:1)
    
    ---
    
    # 💡 이 미션이 평가하려는 능력
    1. 브랜드를 정의할 수 있는가
    2. 광고 메시지를 설계할 수 있는가
    3. 장면 단위로 기획할 수 있는가
    4. 목적에 맞는 AI 도구를 선택할 수 있는가
    5. 프롬프트를 개선하며 결과물을 발전시킬 수 있는가
    6. 여러 AI 산출물을 하나의 완성된 영상으로 통합할 수 있는가
    
    즉, **기획 → 프롬프트 작성 → 생성 → 수정 → 편집 → 완성**의 전 과정을 스스로 설계하는 것이 이 과제의 핵심입니다.
    
  ```
</details>

---
[결과물1: 설계도 .pdf]
## Step 2: 브랜드 기획하기
광고할 브랜드를 하나 정한다.
[나] 실존하는 브랜드 '대전서구이글스 유소년야구단'으로 정했다.
- 브랜드 이름: 대전서구이글스 유소년야구단
- 타겟: 대전 관내 야구에 관심이 있거나 야구를 배우고 있는 유소년 야구학생선수 및 그 학부모/주변인
- 톤앤매너(분위기): 활기찬, 에너제틱, 청춘, 젊음, 팀컬러(주로 검정/주황 라인)
- USP: 야구 선수를 하기 위해 공부를 포기하고, 가족 및 친구와 보내는 시간을 줄이는 게 정답은 아니다.

## Step 3: 캠페인 목표 & 핵심 메세지 정하기
이 광고를 왜 만드는지?
- 유소년기 야구를 공부와 가족들과 함께 즐기며 할 수 있다는 걸 널리 알린다.

핵심 메세지 1문장: "공부하는 야구, 생활 속의 야구, 즐기는 야구"

## Step 4: 씬(Scene)별 스토리보드 작성하기 & AI 도구 선정하기
(1) Story board  

| 항목 | 씬1 | 씬2 | 씬3 | 씬4 |
|---|---|---|---|---|
| 씬 번호 | 1 | 2 | 3 | 4 |
| 씬 길이(초) | 2 | 3 | 3 | 2 |
| 전달 메시지 | 유소년 야구 시작하려면 공부는 포기해야 하는가? (질문을 던짐) | 정답은 그렇지 않다. 운동과 학업 병행을 지향하는 리그가 존재합니다. (투구 장면) | 그 리그에서 공부하며 야구선수로서 꿈을 키워가는 대전서구이글스 (타격 장면) | 팀 로고 소개, 슬로건 노출 |
| 화면 구성 | 검은색 배경이 등장하며 "야구선수로 키우려면 공부는 포기해야 한다며?" 말머리에 텍스트가 fade in/out으로 부드럽게 표현된다. | 투수가 와인드업 자세를 취한 뒤 공을 힘차게 던지는 모습. | 타자가 공을 힘차게 치는 모습. | 다시 검은 배경에 '대전서구이글스' 로고와 슬로건("공부하는 야구, 생활 속의 야구, 즐기는 야구") 문자가 페이드인하며 영상이 끝. |
| 내레이션/카피 문구 | 내레이션: (남성, 속삭이는 목소리) "야구선수로 키우려면 공부는 포기해야 한다며?" / 효과음: 없음 / 자막: 없음 | 내레이션 (차분한 여성 아나운서 목소리): "아니오! 운동과 학업 병행을 지향하는 대한유소년야구연맹이 있으니까요." / 효과음: 야구선수가 투구하는 소리 / 자막: 없음 | 내레이션(차분한 여성 아나운서 목소리): "대전서구이글스! 여기서 야구선수의 꿈과 학업, 두 마리의 토끼를 잡으세요!" / 효과음: 타자가 타격하는 소리 / 자막: 없음 | 자막: "공부하는 야구, 생활 속의 야구, 즐기는 야구" |
| 사용 AI 도구 | Capcut (배경 이미지 + 텍스트 페이드인/아웃) + ElevenLabs (내레이션 TTS) | Sora-2 (Text to image AI image genetaion) + ElevenLabs (내레이션 TTS) | Sora-2 (Text to image AI image genetaion) + ElevenLabs (내레이션 TTS) | Capcut (배경 이미지 + 텍스트&로고 페이드인) |
| 도구 선정 이유 | 완전히 어두운 배경과 한국어 표현의 온건성을 위해 배경과 텍스트의 fade in/out 효과는 편집 툴만 사용(AI 영상 사용 시, 과도한 토큰 소모와 결과물의 불완전성으로 영상 제작 효율이 매뉴얼 생성 대비 매우 떨어짐). 속삭이는 남성 목소리는 감정 표현이 섬세한 ElevenLabs TTS (Eleven v3)로 구현 | Kling, Runway 사용 시, 유료 결제 압박과 유효한 결과물 생성이 안되는 어려움을 겪어 네이토의 미디어 생성 모델(Sora-2, 가장 저렴)을 활용한 T2V 기법 (네이토(범용 AI모델의 API 활용 플랫폼) 사용 시 reference 첨부가 불가한 현상으로 인해 I2V 기법을 적용할 수 없었음)으로 4개의 비디오를 생성했고, 그 중 1개가 유효하게 생성되었다. | 씬2와 동일한 이유로 네이토 미디어 생성 모델(Sor-2)을 활용했고, 1개의 비디오가 유효하게 생성되었다. | 씬1과 동일한 이유(화면/음성 구성이 일치함.), 모든 씬에서 내레이션은 Elevenlabs TTS가 가장 저렴하고 효율적이며 고품질의 음성을 생성하여 선정하였다. |
| 실제 프롬프트 원문 | (ElevenLabs TTS - Eleven v3 사용, 중년 남성 목소리 옵션 선택) [Whisper] 야구선수로 키우려면 공부는 포기해야 한다며? | (Sora-2, 네이토) (1)참조 <br><br> [ElevenLabs TTS - 차분한 여성 아나운서] 아니오! 운동과 학업 병행을 지향하는 대한유소년야구연맹이 있으니까요. | (Sora-2, 네이토) (2)참조 <br><br>[ElevenLabs TTS - 차분한 여성 아나운서] 대전서구이글스! 여기서 야구선수의 꿈과 학업, 두 마리의 토끼를 잡으세요! | Not Applicable |
| 생성 결과 요약 | | | | |
| 생성 파일명/링크 | | | | |

(1) 씬2 Sora-2 프롬프트
```
A handsome 10-year-old Korean boy with glasses, youth baseball pitcher, 
wearing a black and orange baseball uniform in the style of a Baltimore-inspired 
little league team, with a team logo-style patch on the right chest and a smaller 
emblem patch on the left upper sleeve, standing on a dusty pitcher's mound, 
mid-afternoon sunlight, cinematic sports photography style, shallow depth of field, 
24fps, 16:9.

0:00-0:02 — Wind-up: 
Boy stands tall on the mound, glove and ball held together at chest, 
slowly raises front leg into a high leg kick, eyes locked on target, 
calm focused expression through his glasses.

0:02-0:04 — Cocking / Weight Shift:
Body begins rotating, throwing arm cocks back behind the head, 
hips drive forward, torso coils, front leg begins descending toward the mound.

0:04-0:06 — Drive / Plant:
Front foot plants firmly on the rubber, hips and shoulders rotate explosively 
toward home plate, throwing arm whips forward, glasses stay steady on his face, 
intense determined expression.

0:06-0:07 — Release:
Explosive release moment — ball leaves fingertips, full torso rotation completed, 
arm fully extended toward home plate, sharp focused eyes, slight motion blur on the ball.

0:07-0:08 — Follow-through:
Throwing arm sweeps down and across the body, back leg lifts off the rubber, 
slight forward lunge, dust kicks up from the mound, uniform patches visible 
on chest and sleeve.

Camera: low-angle tracking shot, slow push-in during the release moment (0:04-0:06), 
slight slow-motion emphasis on release, smooth handheld realism.

Negative prompt: blurry face, distorted hands, extra limbs, warped ball, 
unnatural pose, low resolution, glasses falling off, logo distortion, 
inconsistent uniform color.

Technical: 24fps, 16:9 aspect ratio, slight motion blur, natural sunlight, 
realistic cinematic sports broadcast look.
```

(2) 씬3 Sora-2 프롬프트
```
Low-angle telephoto lens sports broadcast video of a focused young Korean baseball batter (around 10 years old) at home plate, executing a powerful batting swing. He wears a black uniform jersey with distinct orange stripes and piping, paired with white pants featuring orange side lines. His matte black protective batting helmet with a jaw guard prominently features a simple version of the Rakuten Eagles team logo on the front. He swings a composite baseball bat, making perfect contact with an incoming baseball, sending it flying with natural motion blur indicating high velocity. Directly behind him, a young crouching catcher in full white and grey protective gear and a home-plate umpire are focused on the play, forming a clear triangular alignment on the dirt and grass field. The background features a quiet, empty stadium with green outfield fences and concrete stands, bathed in bright afternoon sunlight, providing a clear but beautifully blurred shallow depth of field. Realistic skin textures, faint grain typical of a sports broadcast, dynamic and raw cinematic movement. Single shot, seamless motion, no cuts.
```

Kling과 Runway를 활용해 이미지 기반 영상 생성(I2V)을 시도해 보았다. 그러나 Kling의 무료 플랜은 월간 크레딧 제한으로 인해 한 달에 고작 한 편의 영상만 제작할 수 있었고, Runway 역시 하루에 1~2편 남짓 생성하는 데 그치는 데다 결과물의 품질마저 떨어져 만족스러운 유효 결과물을 얻기 어려웠다. 이처럼 영상 생성 AI를 선정하는 과정에서 과도한 비용 부담과 저품질 결과물이라는 높은 장벽을 경험하다 보니, 음성 생성 AI를 고를 때는 선뜻 다른 모델들을 다양하게 테스트해 볼 엄두조차 나지 않았다. 결국 이러한 심리적 위축 속에서 단 한 번의 시도로 비용과 품질 모두 높은 만족도를 준 ElevenLabs(TTS)를 최종 모델로 선정하게 되었다.

씬 1
[00:00-00:50]
투수 뒤에서 바라본 인조 잔디 야구장(리틀리그 야구장, 마운드는 흙)의 넓은 전경 샷, 홈 플레이트 뒤에 걸려 있는 텅 빈 현수막(배경색은 흰색, 텍스트는 "2026년 순창고추장배 유소년야구대회", 가운데 정렬, 텍스트 컬러 2026년(파랑색), 순창고추장배(빨강색), 유소년야구대회(검정색), 현수막 사이즈(가로로 긴, 1:9), 따뜻한 늦은 오후 햇살, 멀직이 들려오는 매미 울음소리, 고요한 긴장감, 영화 같은 스포츠 다큐멘터리 스타일, Aspect ratio 16:9.

씬 3
Low-angle telephoto lens sports broadcast video of a focused young Korean baseball batter (around 10 years old) at home plate, executing a powerful batting swing. He wears a black uniform jersey with distinct orange stripes and piping, paired with white pants featuring orange side lines. His matte black protective batting helmet with a jaw guard prominently features a simple version of the Rakuten Eagles team logo on the front. He swings a composite baseball bat, making perfect contact with an incoming baseball, sending it flying with natural motion blur indicating high velocity. Directly behind him, a young crouching catcher in full white and grey protective gear and a home-plate umpire are focused on the play, forming a clear triangular alignment on the dirt and grass field. The background features a quiet, empty stadium with green outfield fences and concrete stands, bathed in bright afternoon sunlight, providing a clear but beautifully blurred shallow depth of field. Realistic skin textures, faint grain typical of a sports broadcast, dynamic and raw cinematic movement. Single shot, seamless motion, no cuts.

(2) 오디오 계획

| 항목 | 상세 내용 |
|---|---|
|사용 AI 도구|Suno (BGM 생성)|
|도구 선정 이유|에너제틱하고 처운 느낌의 배경음악을 짧은 길이로 맞춤 생성 가능|
|실제 프롬프트 원문|upbeat energetic sports anthem, youthful, drums and brass, 10 seconds, trumphat feeling|
|생성 결과 요약||
|생성 파일명/링크|bgm_main.mp3|


[결과물2: 영상파일 .mp4]
