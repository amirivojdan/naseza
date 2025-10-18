<p align="center">
    <em><h2 align="center">NASEZA / ناسزا</h2></em>
    <em><h3 align="center">A Large-Scale Dataset for Persian Hate Speech and Offensive Language Detection</h3></em>
</p>

<p align="center">
    <a href="https://doi.org/10.5281/zenodo.17355123"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.17355123.svg" alt="DOI"></a>
</p>

### Overview

**Naseza (ناسزا)** is a curated dataset of Persian text samples collected from Telegram channels focused on political discussions and sports fan clubs.
The dataset is designed to support hate speech and offensive language detection tasks in Persian, addressing a key gap in available linguistic resources for Persian NLP research.


### مرور کلی

ناسزا (Naseza) یک پیکره‌ی گزینش‌شده از نمونه‌های متنی زبان فارسی است که برای استفاده در شناسایی گفتار نفرت‌آمیز و زبان توهین‌آمیز در فارسی طراحی شده و شکاف موجود در منابع زبانی در دسترس برای پژوهش‌های پردازش زبان طبیعی فارسی را پر می‌کند. این پیکره به طور عمده از کانال‌های تلگرام با محوریت بحث‌های سیاسی و هواداران ورزشی گردآوری شده است. 


### 📊 Dataset Summary

| Label         | Samples | Description                                                                                             |
| ------------- | ------- | ------------------------------------------------------------------------------------------------------- |
| **Offensive** | 2,429   | Contains insults, slurs, or verbally aggressive language directed toward individuals, teams, or groups. |
| **Normal**    | 3,290   | Contains neutral, non-offensive, or contextually benign language.                                       |

Total samples: **5,719**

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
- [x] Character-level classification

### ⚖️ License

The dataset is released under the **CC0-1.0 license** (Public Domain Dedication).
You are free to use, modify, and redistribute the data for both research and commercial purposes.

### Citation

If you use this dataset in your research or projects, please cite it as:

**APA Style:**

> Amirivojdan, A. (2025). *Naseza: A Large-Scale Dataset for Persian Hate Speech and Offensive Language Detection* (Version v1.0.0) [Dataset]. Zenodo. [https://doi.org/10.5281/zenodo.17355123](https://doi.org/10.5281/zenodo.17355123)

**BibTeX:**
```bibtex
@dataset{amirivojdan_2025_naseza,
  author       = {Ahmad Amirivojdan},
  title        = {Naseza: A Large-Scale Dataset for Persian Hate Speech and Offensive Language Detection},
  year         = {2025},
  publisher    = {Zenodo},
  version      = {v1.0.0},
  doi          = {10.5281/zenodo.17355123},
  url          = {https://doi.org/10.5281/zenodo.17355123},
  license      = {CC0-1.0}
}

