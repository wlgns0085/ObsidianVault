![[Screenshot from 2025-08-25 15-02-56 1.png]]
![[Pasted image 20250825153218.png]]




### RVIZ 처리 순서
지형 생성
- 기준점이 될 Global 좌표 설정
	- 안테나 위치, HomePosition 위치, 수동설정 등의 방법으로 설정
	- WGS or UTM의 Global 좌표계 필요
- 비행영역(기준점 좌표 1.5km 반경)의 위성지도 다운로드
	- ESRI World Imagery 활용
- 비행영역의 DEM 파일 파싱 및 지표면 데이터 생성
	- gdal 활용




| 좌표계 | +X  | +Y  | +Z  | 용도             |
| --- | --- | --- | --- | -------------- |
| NED | 북   | 동   | 아래  | 항공기, 드론 비행     |
| ENU | 동   | 북   | 위   | 지도, GNSS, RViz |
RVIZ Axes
- 빨간색: X축, 앞쪽 방향
- 초록색: Y축, 왼쪽 방향
- 파란색: Z축, 위쪽 방향


