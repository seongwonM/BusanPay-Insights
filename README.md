# 🏙️ 부산 지역화폐 분석 및 활성화 방안  
📊 **Big Data 학회 비어플(Baf) 23-1학기 프로젝트 5조**  

[![Website](https://img.shields.io/badge/Visit%20Baf-Website-blue?style=for-the-badge&logo=google-chrome&logoColor=white)](https://www.dgubaf.com/forum/peurojegteu/je19hoe-23-1haggi-peurojegteu-1)  

---

## 📌 프로젝트 개요  
📍 **목적:**  
부산광역시 지역화폐 **동백전** 데이터를 분석하여 **군구별 소비 특성**을 파악하고, 지역화폐 활성화 방안을 제안합니다.  

📍 **주요 분석 내용:**  
- 🏢 **부산 지역화폐 거래 데이터 분석 (6~8월 기준)**
- 🔍 **군구별 EDA (Exploratory Data Analysis)**
- 📈 **소비 트렌드 분석 (업종별, 연령대별, 시간대별 등)**
- 🤖 **Clustering을 활용한 군집화 및 지역별 소비 특성 분류**
- 💡 **활성화 방안 도출 (고령층, 20대, 특정 지역 맞춤 전략)**  

---

## 🗂️ 데이터 개요  

📍 **사용 데이터:**  
| 데이터셋명 | 설명 |
|------------|--------------------------------|
| `busan_local_currency.csv` | 부산 지역화폐 군구별 거래 데이터 |
| `busan_population.csv` | 부산 인구수 데이터 |
| `busan_merchants.csv` | 부산 지역화폐 가맹점 데이터 |

📍 **주요 변수:**  
| 변수명 | 설명 |
|--------|--------------------------------|
| `strd_date` | 기준일자 |
| `ccg_nm` | 시군구명 |
| `tpbuz_nm` | 업종명 |
| `bth_yr` | 출생연도 |
| `sex_cd` | 성별 코드 |
| `trns_cnt` | 거래 건수 |
| `ttl_trns_amt` | 총 거래 금액 |

---

## 🔍 **EDA & 주요 분석**  

### 📊 **1. 군구별 소비 패턴 분석**  
✔ 부산 **16개 구** 대상  
✔ 금요일, 토요일 소비 금액이 가장 많음  
✔ 여성 사용자가 많고, 주로 **편의점, 생활용품, 외식 업종에서 소비**  

### 📊 **2. 시간대별 거래 특성**  
✔ 거래 건수 **12시, 18시**(식사 시간대)에서 가장 많음  
✔ 평균 거래 금액은 **19~20시 (퇴근 후, 회식 시간대)가 가장 높음**  

### 📊 **3. 연령대별 소비 특성**  
✔ 전체적으로 **30~50대가 가장 많이 사용**  
✔ **20대는 금정구에서 가장 많이 소비** → 부산대학교 영향  
✔ **60대 이상은 의료, 교육 분야 소비 비중 높음**  

### 🤖 **4. Clustering을 활용한 지역 그룹화**  
✔ **K-modes & K-means** 기법 사용  
✔ 📌 주요 분류:  
  - **소비 중심 지역** (부산진구, 해운대구, 동래구)  
  - **거래량 대비 소비 비율 낮은 지역** (사하구, 영도구)  
  - **소비 특성이 독특한 지역** (금정구 → 20대 소비 많음)  

---

## 💡 **활성화 방안 제안**  

🔹 **고령층 대상 활성화 방안**  
- 💳 카드 사용이 어려운 노인을 위한 **동백전 오프라인 사용처 확대**  
- 🏥 의료 가맹점 확대 → 의료비 지출이 많은 지역(수영구, 영도구) 타겟  

🔹 **20대 소비층 확대 방안**  
- 🎟 **생활·레저 분야 가맹점 확대** → 20대가 많은 금정구 중심으로  
- 🎭 **문화·취미 업종 활성화** → 해운대구, 연제구 (문화 소비↑)  

🔹 **특정 지역 맞춤 전략**  
- 🛍 패션 거리 홍보 → 중구(광복 패션 거리)  
- 🕒 가맹점 운영 시간 조정 → 출퇴근 시간 이용 가능하도록  

---

## 🛠️ 사용 기술  
✅ **분석 도구:** `Python`, `Pandas`, `Scikit-learn`  
✅ **분석 기법:** `K-means`, `Random Forest`  
✅ **시각화 도구:** `Seaborn`, `Matplotlib`

---

## 📜 팀원 소개  
👨‍💻 **프로젝트 참여자:**  
- **10기** 최은진  
- **11기** 이다현  
- **12기** 문성원  

---

## 📎 관련 링크  
🔗 **[Big Data 학회 비어플(Baf)](https://www.dgubaf.com/)**  
🔗 **[프로젝트 발표 자료](files/presentation.pdf)**  
🔗 **[데이터 출처](https://www.data.go.kr/)**  

---

## 📌 레포지토리 구조  

📂 **부산지역화폐분석**  
│── 📄 **README.md**  → 프로젝트 개요  
│  
├── 📂 **data**  → 원본 데이터셋  
│   ├── 📄 busan_population.csv  
│   ├── 📄 jult_군구,연령별.xlsx  
│   ├── 📄 june_군구,연령별.xlsx  
│   ├── 📄 population_august.xlsx  
│   ├── 📄 population_july.xlsx  
│   ├── 📄 population_june.xlsx  
│   ├── 📄 부산광역시_지역화폐(동백전) 가맹점 현황_20221222.csv  
│   ├── 📄 부산시 인구.csv  
│   ├── 📄 업종코드.csv  
│   ├── 📄 업종코드_중분류.csv  
│  
├── 📂 **eda**  → 탐색적 데이터 분석 (EDA)  
│   ├── 📄 20230317.ipynb  
│   ├── 📄 20230510.ipynb  
│   ├── 📄 card_dh.ipynb  
│   ├── 📄 eda_230324.ipynb  
│   ├── 📄 ej0401.ipynb  
│   ├── 🌍 map.html  
│   ├── 📄 map0512.ipynb  
│   ├── 📄 preProcess.ipynb  
│   ├── 📄 pre_process_20230318.ipynb  
│   ├── 📄 pre_process_20230401.ipynb  
│   ├── 📄 project_20220310_sw.ipynb  
│   ├── 📄 project_20230318_sw.ipynb  
│   ├── 📄 study1.ipynb  
│  
├── 📂 **modeling**  → 머신러닝 & 모델링  
│   ├── 📄 LDH_final.ipynb  
│   ├── 📄 MSW_final.ipynb  
│   ├── 📄 numerical.ipynb  
│   ├── 📄 수치형합본.csv  
│  
├── 📂 **files**  → 발표자료  
│   ├── 📄 presentation.pdf  
│  
└── 📄 .DS_Store (Mac 시스템 파일)
