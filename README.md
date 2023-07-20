# ERGPT
OpenAI API-based application to address the delay in transporting emergency patients
Project for 2023 KHIDI Public Data Usage Idea Contest

# **[Eng]**  
## 🔎 Problem Definition
Key Issue: Delays in emergency room transfers and patient refusals for critically ill patients.

Problem Analysis  
**Where?**: Identifying the point where delays occur in the emergency patient process  
🔸Call reception > Ambulance dispatch > On-site treatment & evaluation > Decision to transfer to ER > Patient transfer > Hospital admission > Transfer to ward > Discharge  
🔸Delays primarily occur at the Decision to transfer to ER and during Transfer to ward.  

**Why?**  
1) First responders find it challenging to accurately assess the patient's condition.
2) Difficulty in determining the emergency room with the appropriate on-call specialist and medical facilities for the patient's treatment.

## ✨ Solutions  
**A. KTAS classification using GPT API**    

🔸Input: Basic patient information (gender, age range, symptoms) and vital signs (blood pressure, pulse, respiration rate, temperature, level of consciousness)    

🔸Output: KTAS classification code

* KTAS (Korean Triage and Acuity Scale): Established according to the "Korean Emergency Patient Severity Classification Standard" under Article 18-3 of the Enforcement Rules of the Emergency Medical Service Act. It classifies patients into five levels based on their symptoms, using primary and secondary considerations, consisting of a total of 4,368 classification items.

**B. Optimal ER Selection based on KTAS and Hospital Data**    

🔸Input: Patient's KTAS code, on-call specialist and facility status by hospital, ambulance location, and estimated travel time.    

🔸Output: Selection of the best-suited hospital.

  
# **[Kor]**  
## 🔎 문제 정의

핵심 문제: 중증응급환자의 응급실 이송 지연과 환자 거부

문제 분석  
**Where?**: 응급 환자 Process 중 Delay가 발생하는 지점 파악  
🔸신고 접수 > 구급차 출동 > 현장 치료 및 평가 > 응급실 이송 결정 > 환자 이송 > 내원 > 전원 > 퇴원  
🔸**응급실 이송 결정** 및 **전원**에서 지연이 발생함.  

**Why?**
1) 구조대원이 환자의 상태를 명확히 판단하기 어려움
2) 환자의 치료에 적합한 당직 전문의와 의료 설비가 있는 응급실을 판단할 수 없음

## ✨ 해결 방법
**A. GPT API를 활용한 KTAS 분류**    

🔸Input: 기본적인 환자 정보 (성별, 연령대, 증상) 및 바이탈 정보 (혈압, 맥박, 호흡 수, 체온, 의식 수준)  

🔸Output: KTAS 분류코드

* KTAS (Korean Triage and Acuity Scale): 응급의료에 관한 법률 시행규칙 제18조의 3에 의거 제정된 "한국 응급환자 중증도 분류기준"으로, 환자의 증상을 근거로 1, 2차 고려사항을 적용하여 환자의 응급도를 5단계로 나누어 평가하며 총 4,368개의 분류 항목으로 이루어져 있습니다.

**B. KTAS 및 병원 데이터 기반 최적 응급실 선정**  

🔸Input: 환자의 KTAS 코드, 병원별 당직 전문의 및 설비 현황, 구급차 위치 및 예상 이동시간  

🔸Output: 최적의 병원 선정
