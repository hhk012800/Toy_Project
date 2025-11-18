발전소에서는 터빈과 보일러에 부착된 센서를 통해 시간 단위로 주요 지표를 수집 컬럼명 설명 Timestamp 시간 (1시간 단위) UnitID 설비 ID (Turbine_A, Boiler_1 등) Temperature 설비 내부 온도 (°C) Pressure 내부 압력 (bar) Vibration 진동 수치 (mm/s) GasFlow 연료 유량 (m³/h) SteamOutput 증기 생산량 (ton/h) Failure 고장 여부 (1=고장, 0=정상)

1> 데이터 전처리

2> EDA

고장(1)과 정상(0) 그룹 간 평균 Temperature, Pressure, Vibration 차이를 변화 추이

3> 딥러닝 기반 예측

주어진 센서 데이터를 기반으로 Failure 여부를 예측하는 분류 모델을 딥러닝으로 설계(간단하게) 입력: Temperature, Pressure, Vibration, GasFlow, SteamOutput 출력: Failure (0 or 1)
