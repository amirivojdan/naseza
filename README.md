## Naseza (ناسزا)
*A Large-Scale Dataset for Persian Hate Speech and Offensive Language Detection*


### Overview

**Naseza (ناسزا)** is a curated dataset of Persian text samples collected from Telegram channels focused on political discussions and sports fan clubs.
The dataset is designed to support hate speech and offensive language detection tasks in Persian, addressing a key gap in available linguistic resources for Persian NLP research.


### مرور کلی

ناسزا (Naseza) یک پیکره‌ی گزینش‌شده از نمونه‌های متنی زبان فارسی است که برای استفاده در شناسایی گفتار نفرت‌آمیز و زبان توهین‌آمیز در فارسی طراحی شده و شکاف موجود در منابع زبانی در دسترس برای پژوهش‌های پردازش زبان طبیعی فارسی را پر می‌کند. این پیکره به طور عمده از کانال‌های تلگرام با محوریت بحث‌های سیاسی و هواداران ورزشی گردآوری شده است. 


### 📊 Dataset Summary

| Label         | Samples | Description                                                                                             |
| ------------- | ------- | ------------------------------------------------------------------------------------------------------- |
| **Offensive** | 1,963   | Contains insults, slurs, or verbally aggressive language directed toward individuals, teams, or groups. |
| **Normal**    | 3,059   | Contains neutral, non-offensive, or contextually benign language.                                       |

Total samples: **5,022**

All samples are written in Persian and come from informal, colloquial user-generated text in Telegram discussions.


### 📄 Format Example


```json 
[
    {
        "id": 39,
        "text": "اون دیگه نه.",
        "label": [
            "Normal"
        ],
        "Comments": []
    },
    {
        "id": 40,
        "text": "تیم به گا رفت دیگه کاری ازمون بر نمیاد",
        "label": [
            "Offensive"
        ],
        "Comments": []
    }
]
```

### Future Works

- [ ] Data augmentation (ex. inserting random markers)
- [ ] Increase dataset size by using fuzzy string matching (Levenshtein distance) between normalized candidate tokens and offensive lexicon
- [ ] Ensemble of classifiers
- [ ] Character-level classification

### ⚖️ License

The dataset is released under the **CC0-1.0 license** (Public Domain Dedication).
You are free to use, modify, and redistribute the data for both research and commercial purposes.

