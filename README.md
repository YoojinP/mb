[데이터셋_정리.txt](https://github.com/user-attachments/files/24248950/_.txt)
cosmos av 데이터셋
----------------------------------------------------------

[메타 정보]
▷ 다양한 도로 상황
	- 50% 미국, 50% 유럽 데이터로 구성
	- 맑음/ 눈/ 비/ 안개 날씨 데이터 포함
	- 건조/ 눈/ 젖은 노면 상태 데이터 포함
	- 낮/ 밤 데이터 포함
	- 대/중/소/제로 교통량 데이터 포함
	- 터널/ 다리/ 회전 교차로/ 건널목/ 톨부스/ 경사 등 데이터 포함
▷ 약 31만개의 클립(.mp4) 
	- 클립은 20초/ 30fps
▷ 약 16만개의 센서 데이터 
	- 7개 카메라/ 10개 레이더/ ego motion/ 칼리브레이션/ 기계 라벨
▷ 총 용량은 약 100 TB

▷ 다음주 추가 업데이트 있을 예정

----------------------------------------------------------

[구성]
▷ 캘리브레이션
	- 카메라 intrinsic 
	- 센서들 extrinsic
	- vehicle dimension: 자동차 크기 및 폭
	
▷카메라 
	- 프레임 인덱스 당 바운딩박스, 라벨 정보x
	- 프레임 인덱스 당 타임스텝
	- 프레임 인덱스 당 이미지
	
▷라벨 
	- ego motion: ego 자동차 정보
		- timestamp
		- qx, qy, qz, qw
		- x, y, z
		- vx, vy, vz
		- ax, ay, az
		- curvature
▷라이다
	- reference timestamp
	- draco point cloud
	
▷메타데이터
	- data collection: 데이터 기록 메타 정보 
	- sensor presence: 클립마다 어떤 센서 데이터 존재하는지 기록
	
▷레이더
	- timestamp: ego motion 기반 로컬 시간
	- sensor timestamp: 센서 내부 기록 시간
	- num returns
	- doppler ambiguity
	- max returns
	- detection index
	- radar model
	- azimuth
	- elevation



