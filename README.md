# route-guide-maps

버스배차알림 앱의 **노선 길잡이** 기능이 내려받는 오프라인 지도 파일 저장소입니다.
지도 파일은 [Releases](../../releases)에 권역별로 올라가 있습니다.

| 릴리스 태그 | 지역 | 지도 크기 | 파일 |
|---|---|---|---|
| `seoul-20261009` | 서울 | 41.9MB | `seoul.pmtiles`, `seoul.manifest.json` |
| `capital-20261009` | 수도권 (서울·경기·인천) | 145.8MB | `capital.pmtiles`, `capital.manifest.json` |
| `gangwon-20261009` | 강원 | 109.4MB | `gangwon.pmtiles`, `gangwon.manifest.json` |
| `chungcheong-20261009` | 충청 | 136.7MB | `chungcheong.pmtiles`, `chungcheong.manifest.json` |
| `jeolla-20261009` | 전라 | 130.7MB | `jeolla.pmtiles`, `jeolla.manifest.json` |
| `gyeongsang-20261009` | 경상 | 182.2MB | `gyeongsang.pmtiles`, `gyeongsang.manifest.json` |
| `jeju-20261009` | 제주 | 10.2MB | `jeju.pmtiles`, `jeju.manifest.json` |

- 형식: [PMTiles](https://github.com/protomaps/PMTiles) v3 벡터 타일, 최대 확대 15
- 원본: [Protomaps Basemap](https://protomaps.com/) 일일 빌드(스키마 4.x)에서 권역 범위만 잘라냄
- 앱은 Firestore의 지도 목록에서 주소·버전·SHA-256을 읽어 이 파일을 받습니다. 파일 이름이나 태그를 바꾸면 목록도 함께 고쳐야 합니다.

## 라이선스와 출처

지도 데이터 © [OpenStreetMap contributors](https://www.openstreetmap.org/copyright), [Open Database License (ODbL) 1.0](https://opendatacommons.org/licenses/odbl/1-0/).

이 저장소의 지도 파일은 OpenStreetMap 데이터로 만든 Protomaps Basemap 빌드를 범위만 잘라 그대로 배포한 것이며, ODbL을 따릅니다. 지도를 화면에 표시할 때는 "© OpenStreetMap contributors"를 표시해야 합니다.
