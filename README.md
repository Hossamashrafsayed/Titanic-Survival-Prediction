# Epsilon-Ai
# 🚢 Titanic Survival Prediction

<div align="center">

![Python](https://img.shields.io/badge/Python-3.10+-blue?logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-2.0+-150458?logo=pandas&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-1.3+-F7931E?logo=scikit-learn&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-2.0+-red)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3.7+-11557C)
![Seaborn](https://img.shields.io/badge/Seaborn-0.12+-4C72B0)
![Kaggle](https://img.shields.io/badge/Kaggle-Titanic-20BEFF?logo=kaggle&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green)

**تحليل شامل لبيانات ركاب تايتانيك وبناء نماذج تعلم آلي للتنبؤ بفرص النجاة**

</div>

---

## 📌 نظرة عامة على المشروع

هذا المشروع يقدم **تحليلاً استكشافياً كاملاً (EDA)** لبيانات ركاب سفينة **RMS Titanic** الشهيرة، ثم يبني ويقارن بين عدة **نماذج تعلم آلي (Machine Learning)** للتنبؤ باحتمالية نجاة الراكب بناءً على خصائصه (العمر، الجنس، الطبقة، ... إلخ).

المشروع مستوحى من مسابقة **Kaggle Titanic: Machine Learning from Disaster** — أشهر مسابقة للمبتدئين في عالم الـ ML.

### 🎯 أهداف المشروع
- فهم العوامل التي أثّرت على فرص النجاة (الجنس، العمر، الطبقة، ...).
- معالجة البيانات الناقصة (Missing Values) بذكاء.
- استخراج ميزات جديدة (**Feature Engineering**) من الأعمدة الموجودة.
- بناء وتقييم عدة نماذج تصنيف (**Classification**).
- اختيار أفضل نموذج بناءً على **Accuracy** و **Cross-Validation**.

---

## 📂 محتويات المشروع (Table of Contents)

- [نظرة عامة](#-نظرة-عامة-على-المشروع)
- [البيانات](#-البيانات-dataset)
- [التقنيات المستخدمة](#-التقنيات-المستخدمة)
- [هيكل المشروع](#-هيكل-المشروع)
- [التثبيت والتشغيل](#-التثبيت-والتشغيل)
- [التحليل الاستكشافي (EDA)](#-التحليل-الاستكشافي-eda)
- [معالجة البيانات و Feature Engineering](#-معالجة-البيانات-و-feature-engineering)
- [نماذج التعلم الآلي](#-نماذج-التعلم-الآلي)
- [النتائج](#-النتائج)
- [أهم الاستنتاجات](#-أهم-الاستنتاجات)
- [التطويرات المستقبلية](#-التطويرات-المستقبلية)
- [المؤلف](#-المؤلف)
- [الترخيص](#-الترخيص)

---

## 📁 البيانات (Dataset)

| الخاصية | القيمة |
|---------|--------|
| **المصدر** | [Kaggle Titanic Competition](https://www.kaggle.com/c/titanic/data) |
| **ملف التدريب** | `train.csv` (891 صف × 12 عمود) |
| **ملف الاختبار** | `test.csv` (418 صف × 11 عمود) |
| **المتغير الهدف** | `Survived` (0 = لم ينجُ، 1 = نجا) |
| **نسبة النجاة** | ≈ 38.4% |

### الأعمدة الرئيسية
| العمود | النوع | الوصف |
|--------|-------|-------|
| `PassengerId` | int | رقم الراكب |
| `Survived` | int | **الهدف** (0/1) |
| `Pclass` | int | فئة التذكرة (1 = أولى، 2 = ثانية، 3 = ثالثة) |
| `Name` | object | اسم الراكب (يحتوي على اللقب) |
| `Sex` | object | الجنس (male / female) |
| `Age` | float | العمر (177 قيمة ناقصة) |
| `SibSp` | int | عدد الأشقاء/الأزواج على متن السفينة |
| `Parch` | int | عدد الآباء/الأبناء على متن السفينة |
| `Ticket` | object | رقم التذكرة |
| `Fare` | float | سعر التذكرة |
| `Cabin` | object | رقم المقصورة (687 قيمة ناقصة) |
| `Embarked` | object | ميناء الصعود (C = Cherbourg, Q = Queenstown, S = Southampton) |

---

## 🛠 التقنيات المستخدمة

| الأداة | الاستخدام |
|--------|-----------|
| **Python 3.10+** | لغة البرمجة |
| **Pandas** | معالجة البيانات |
| **NumPy** | العمليات الرياضية |
| **Matplotlib / Seaborn** | التصور البياني |
| **Scikit-Learn** | نماذج ML والتقييم |
| **XGBoost / LightGBM** | نماذج Gradient Boosting |
| **Jupyter Notebook** | بيئة التطوير |

---

## 🗂 هيكل المشروع
