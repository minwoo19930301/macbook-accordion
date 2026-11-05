<p align="center">
  <a href="https://github.com/minwoo19930301/macbook-accordion/releases/latest/download/MacBookAccordion-0.1.3.dmg"><img src="https://img.shields.io/badge/DOWNLOAD%20DMG-0.1.3-FFCC00?style=for-the-badge&labelColor=111111" alt="Download DMG"></a>
</p>

# MacBook Accordion

MacBook 화면 각도 센서로 연주하는 작은 아코디언입니다.

<table>
  <tr>
    <td width="70%"><img src="assets/macbook-accordion-usage.png" alt="MacBook 을 아코디언처럼 잡고 연주하는 모습"></td>
    <td width="30%" align="center"><img src="assets/app-icon.png" alt="앱 아이콘" width="180"></td>
  </tr>
</table>

## 설치

1. 위 **DOWNLOAD DMG** 를 눌러 받습니다.
2. DMG 를 열고 `MacBook Accordion.app` 을 `Applications` 로 끌어 놓습니다.
3. `Applications` 에서 실행합니다. Dock 고정도 여기서 실행한 앱으로 합니다.

서명 안 된 개인 빌드라 처음 열 때 막히면, 앱을 Control-클릭 → `열기` 를 한 번 누르면 됩니다.

## 연주법

1. 카메라 옆 조도 센서를 손가락으로 가립니다.
2. 가린 채로 화면을 열고 닫습니다. 각도가 바뀌어 다음 음으로 넘어갈 때 소리가 납니다.
3. 손을 떼면 소리 없이 움직일 수 있습니다.

카메라 영상이 아니라 조도 값만 읽어서 카메라 권한이 필요 없습니다. 2019년 16인치 MacBook Pro 이후 모델에서 동작합니다. 일부 M1/M2 는 센서 문제가 있습니다.

## 빌드

```shell
./scripts/package_dmg.sh 0.1.3   # dist/MacBookAccordion-0.1.3.dmg
```

원본 실험: [samhenrigold/LidAngleSensor](https://github.com/samhenrigold/LidAngleSensor)
