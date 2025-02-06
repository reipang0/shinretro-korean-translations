<img src="assets/logo_shinretro.png" width="55%" title="shinretro 로고" />

# shinretro

현재 버전: [0.201k](CHANGELOG.md) [![GPLv3 라이선스](https://img.shields.io/badge/license-GPLv3-blue.svg)](LICENSE)

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

※ 오랜 기간 업데이트가 이루어지지 않아 풀 리퀘스트에 응답이 없을 수 있습니다.

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
> **참고:** 컬렉션 화면에 표시되는 비디오는 현재 테마에 포함되지 않았습니다.  
> Pegasus 메타데이터에서 기본 비디오를 설정하여 컬렉션에 추가할 수 있습니다.> 예제:
> 
    collection: Sony Playstation 2
    shortname: ps2
    assets.video: media/videos/default.mp4

## 컬렉션 카테고리 설정 방법
컬렉션을 시스템, 시리즈, 장르 등으로 그룹화할 수 있습니다.  
메타데이터 파일에 'x-collectiontype' 필드를 추가하면, 컬렉션 메뉴 화면에서 필터 버튼을 이용해 카테고리를 변경할 수 있습니다.

<img src="assets/screenshot/collectiontypes.png" title="컬렉션 카테고리" />

## 아케이드 포트 태그 표시 방법
게임이 아케이드 포트로 태그되어 있으면, 플레이어 및 장르 태그 옆에 아케이드 포트 태그가 표시됩니다.
사용하려면 게임 메타데이터에 'x-arcadeport' 필드를 추가하고 값으로 'True'를 입력하세요.

<img src="assets/screenshot/arcade_port.png" title="아케이드 포트 플래그" />

## 클리어 리본 표시 방법
클리어한 게임을 별도로 표시할 수 있습니다.

사용하려면 게임 메타데이터에 'x-completed' 필드를 추가하고 값으로 'True'를 입력하세요.

<img src="assets/screenshot/completed.png" title="완료됨 리본" />

## 커스텀 정렬
이 테마는 컬렉션에 대한 커스텀 정렬을 지원합니다.  
예를 들어 특정 순서로 플레이할 게임 플레이리스트를 만들거나, 시리즈 기반으로 컬렉션을 구성할 때 출시 연도나 게임 제목 순서가 일정하지 않더라도 원하는 순서대로 정렬할 수 있습니다.

기본 `sort-by` 메타데이터 필드를 사용하면 정렬 제목을 설정할 수 있지만, 이는 특정 게임이 속한 모든 컬렉션에 적용됩니다.  
즉, "마리오" 시리즈 컬렉션에서 정렬 순서를 맞춰도, 동일한 게임이 "NES" 시스템 컬렉션에 있을 경우 잘못된 위치에 표시될 수 있습니다.

이 기능을 사용하려면, 커스텀 정렬을 적용할 각 게임에 대해 다음 형식의 새 필드를 게임 메타데이터에 추가하세요.  
`x-customsort-컬렉션_짧은이름`: 정렬번호

예제:  
마리오 게임들을 시리즈별로 연대순으로 정렬하면서, 리메이크판은 원작과 함께 그룹화하고 싶다고 가정해 보겠습니다.  
(즉, NES용 "Super Mario Bros"가 가장 먼저 오고, 그 뒤에 Game Boy Color 및 Game Boy Advance 리메이크가 배치되며, 이후 "Super Mario Bros 2"와 "Super Mario Advance"가 이어지도록 설정)

이 경우, 관련 게임의 메타데이터는 다음과 같이 구성됩니다. (정렬 번호 값을 주의 깊게 확인하세요.)

예제:
> 
    game: Super Mario Bros.
    file: ..\..\..\roms\nes\Super Mario Bros. (World).7z
    sort-title: Super Mario Bros.
    x-customsort-mario: 010

    game: Super Mario Bros. 2
    file: ..\..\..\roms\nes\Super Mario Bros. 2 (USA) (Rev A).7z
    sort-title: Super Mario Bros. 2
    x-customsort-mario: 015

    game: Super Mario Bros. Deluxe
    file: ..\..\..\roms\gbc\Super Mario Bros. Deluxe (USA, Europe) (Rev B).7z
    sort-title: Super Mario Bros. Deluxe
    x-customsort-mario: 011

    game: Classic NES Series: Super Mario Bros.
    file: ..\..\..\roms\gba\Classic NES Series - Super Mario Bros. (USA, Europe).7z
    sort-title: Classic NES Series: Super Mario Bros.
    x-customsort-mario: 012

    game: Super Mario Advance
    file: ..\..\..\roms\gba\Super Mario Advance (USA, Europe).7z
    sort-title: Super Mario Advance
    x-customsort-mario: 016

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
    game: 수왕기
    file: roms\amiga\AlteredBeast_v2.0_0819.lha
    sort-title: Altered Beast
    release: 1989
    developer: Sega
    publisher: Sega
    genre: Action
    players: 2
    x-system: amiga
    rating: 0.8
    description: 당신은 신 제우스에 의해 부활한 전사로, 그의 딸 아테나를 구출해야 합니다. 고대 그리스를 배경으로 한 이 게임에서, 언데드와 악마의 무리를 상대하며, 각 스테이지의 보스를 처치한 후 마지막에는 아테나를 붙잡고 있는 신 네프와 대결해야 합니다. "Altered Beast"라는 제목은 주인공의 변신 능력을 의미합니다. 이 플랫폼 게임에서는 두 개의 머리를 가진 늑대를 처치하여 '스피릿 볼'을 수집하면, 늑대인간, 용, 호랑이, 곰 등 다양한 형태로 변신할 수 있습니다(버전에 따라 다름). 각 변신 형태는 해당 스테이지에 따라 정해져 있으며, 비행 능력이나 강력한 공격과 같은 특별한 능력을 제공하여 인간 상태의 기본적인 펀치 및 킥을 뛰어넘는 강한 전투력을 발휘할 수 있습니다. 이 게임은 싱글 플레이 모드뿐만 아니라, 같은 화면에서 함께 플레이할 수 있는 멀티플레이 협력 모드도 지원합니다.
    x-completed: False
    x-arcadeport: True

## 진행 중인 작업
※ 현재 업데이트가 멈춘 상태이기 때문에 추가 업데이트가 제공되지 않을 수 있습니다.

## 향후 고려 사항
- [ ] 컬렉션 및 제조사용 배경/로고 추가

## 감사 인사
- [Valentin MEZIN](https://github.com/valsou) : neoretrō 원작자
- [Luciano Oliveira](https://github.com/luciano-work) : neoretrō의 다크 테마 제작자
- [HunkDeath](https://github.com/HunkDeath) & [fansubmaniac](https://github.com/fansubmaniac) : 프랑스어 번역
- [RickEves](https://github.com/RickEves) : 포르투갈어 번역
- [RoeTaKa](https://www.youtube.com/channel/UCAbHcM41hzH9lku_3XqFYZg) : 커스텀 사운드 효과 및 BGM
- [kukufeng](https://github.com/kukufeng) : 중국어 번역
- [Reipang](https://www.youtube.com/channel/UCEnrvXHZ-86rDuTsALYp2fg) : 한국어 번역
