<img src="assets/logo_shinretro.png" width="55%" title="shinretro 로고" />

# shinretro

현재 버전: [0.201](CHANGELOG.md) [![GPLv3 라이선스](https://img.shields.io/badge/license-GPLv3-blue.svg)](LICENSE)

[Pegasus Frontend](http://pegasus-frontend.org)용 유연하고 조정 가능한 테마입니다.  
[Valentin MEZIN](https://github.com/valsou)의 테마 [neoretrō](https://github.com/valsou/neoretro) v0.131과 [Luciano Oliveira](https://github.com/luciano-work)의 다크 버전을 기반으로 포크되었습니다.

***

<details>
  <summary><b>스크린샷</b></summary>
  <img src="assets/screenshot/home_dark.png"  title="홈"/>
  <img src="assets/screenshot/home_light.png" title="홈"/>
  <img src="assets/screenshot/home_ozonedark.png"  title="홈"/>
  <img src="assets/screenshot/collection_dark.png" title="컬렉션" />
  <img src="assets/screenshot/collection_light.png" title="컬렉션" />
  <img src="assets/screenshot/collection_ozonedark.png" title="컬렉션" />
  <img src="assets/screenshot/games_dark.png" title="게임" />
  <img src="assets/screenshot/games_light.png" title="게임" />
  <img src="assets/screenshot/games_ozonedark.png" title="게임" />
  <img src="assets/screenshot/settings_dark.png" title="설정" />
  <img src="assets/screenshot/settings_light.png" title="설정" />
  <img src="assets/screenshot/settings_ozonedark.png" title="설정" />
</details>

***

<details>
  <summary><b>비디오</b></summary>
  
  [Retro Gaming Replay](https://www.youtube.com/channel/UC_9gbkxeMk3usXvSzYzimMw)의 테마 리뷰
  
  [![신규 Pegasus 프론트엔드 테마 네오 레트로 다크 - 안드로이드 기기에 적합한 게임 디스플레이](https://img.youtube.com/vi/YbPcsC95Qc0/0.jpg)](http://www.youtube.com/watch?v=YbPcsC95Qc0)

  컬렉션 이미지가 변경된 [RoeTaKa](https://www.youtube.com/channel/UCAbHcM41hzH9lku_3XqFYZg)의 커스텀 버전
  
  [![AYN Odin Pro - Pegasus: 커스텀 Shinretro](https://img.youtube.com/vi/sm5J7JoTYs8/0.jpg)](https://www.youtube.com/watch?v=sm5J7JoTYs8)
  
</details>
  
***

**기여를 환영합니다**

테마의 버그를 수정하거나 기능을 추가하고 싶다면?  
코딩이 어렵지만 번역을 추가하거나 멋진 아트워크를 제공하고 싶다면?  

용기를 내어 풀 리퀘스트를 보내 주세요! 😊  
가이드는 [여기](HACKING.md)에서 확인할 수 있습니다.

## 기능
- 선택 가능한 색상 테마  
`다크(dark)` `라이트(light)` `오존 다크(ozone dark)`
- 커스텀 가능한 게임 화면
- 다양한 온스크린 컨트롤 옵션  
`유니버설(Switch 스타일)` `XBOX` `Playstation`
- 다국어 지원
- 비디오 재생 옵션 토글

기타 설정에 대한 설명은 [여기](SETTINGS.md)에서 확인하세요.
  
## 사용 중인 메타데이터
- boxFront
- screenshot
- titlescreen (screenshot 대체)
- wheel
- background
- video

## 컬렉션 화면에서의 비디오 사용
> **참고:** 컬렉션 화면에 표시되는 비디오는 테마에 포함되지 않습니다.  
> Pegasus 메타데이터에서 기본 비디오를 설정하여 컬렉션에 추가할 수 있습니다. 예제:
> 
    collection: Sony Playstation 2
    shortname: ps2
    assets.video: media/videos/default.mp4

## 컬렉션 카테고리
컬렉션을 시스템, 시리즈, 장르 등으로 그룹화할 수 있습니다.  
컬렉션 메타데이터 파일에 'x-collectiontype' 필드를 추가하면, 컬렉션 캐러셀 화면에서 필터 버튼을 사용해 카테고리를 변경할 수 있습니다.

<img src="assets/screenshot/collectiontypes.png" title="컬렉션 카테고리" />

## 아케이드 포트 플래그
게임이 아케이드 포트로 태그되어 있으면, 플레이어 및 장르 태그 옆에 아케이드 포트 태그가 표시됩니다.

사용하려면 게임 메타데이터에 'x-arcadeport' 필드를 추가하고 값으로 'True'를 입력하세요.

<img src="assets/screenshot/arcade_port.png" title="아케이드 포트 플래그" />

## 클리어 리본
완료한 게임을 추적하려면, 게임이 완료된 경우 그리드 보기에서 "완료됨" 리본을 표시할 수 있습니다.

사용하려면 게임 메타데이터에 'x-completed' 필드를 추가하고 값으로 'True'를 입력하세요.

<img src="assets/screenshot/completed.png" title="완료됨 리본" />

## 커스텀 정렬
컬렉션에서 특정 순서로 정렬하고 싶다면, 이 테마는 커스텀 정렬을 지원합니다.

사용하려면, 특정 컬렉션에 대해 'x-customsort-*collectionshortname*' 필드를 추가하고 정렬 번호를 지정하세요.

예제:
> 
    game: Super Mario Bros.
    x-customsort-mario: 010

    game: Super Mario Bros. 2
    x-customsort-mario: 015

    game: Super Mario Bros. Deluxe
    x-customsort-mario: 011

최종 정렬 결과:
<img src="assets/screenshot/customsort.png" title="커스텀 정렬" />

## 예제 메타데이터 파일
컬렉션 메타데이터 예제:
> 
    collection: Ace Combat
    shortname: acecombat
    sort-by: Ace Combat
    x-collectiontype: Series

게임 메타데이터 예제:
> 
    game: Altered Beast
    x-completed: False
    x-arcadeport: True

## 진행 중인 작업
- [ ] 코드 정리
- [ ] 추가 언어 지원
- [ ] 컬렉션 및 제조사용 누락된 배경/로고 추가

## 향후 고려 사항
- [ ] 기본 컬렉션 비디오 제공
- [ ] 컬렉션별 기본 배경 이미지 제공
- [ ] 장르별 필터 추가
- [ ] 어트랙트 모드 추가

## 감사 인사
- [Valentin MEZIN](https://github.com/valsou) : neoretrō 원작자
- [Luciano Oliveira](https://github.com/luciano-work) : neoretrō의 다크 테마 제작자
- [HunkDeath](https://github.com/HunkDeath) & [fansubmaniac](https://github.com/fansubmaniac) : 프랑스어 번역
- [RickEves](https://github.com/RickEves) : 포르투갈어 번역
- [RoeTaKa](https://www.youtube.com/channel/UCAbHcM41hzH9lku_3XqFYZg) : 커스텀 사운드 효과 및 BGM
- [kukufeng](https://github.com/kukufeng) : 중국어 번역
- [Reipang](https://www.youtube.com/channel/UCEnrvXHZ-86rDuTsALYp2fg) : 한국어 번역
