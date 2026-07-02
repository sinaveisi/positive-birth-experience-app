# 🤰 Positive Birth Experience App

**A published, peer-reviewed mHealth app for midwifery education**

<p>
  <img src="https://img.shields.io/badge/Kotlin-100%25-7F52FF?style=flat-square&logo=kotlin&logoColor=white" />
  <img src="https://img.shields.io/badge/Jetpack%20Compose-UI-4285F4?style=flat-square&logo=jetpackcompose&logoColor=white" />
  <img src="https://img.shields.io/badge/Architecture-MVVM-orange?style=flat-square" />
  <img src="https://img.shields.io/badge/Published-BMC%20Medical%20Education-005AA9?style=flat-square" />
</p>

This Android app is the software artifact behind a peer-reviewed study published in **BMC Medical Education (2025)**. It delivers the WHO's *Intrapartum Care for a Positive Childbirth Experience* guideline to midwifery students through interactive flashcards and scenario-based quizzes, and was evaluated with real students in a pre/post knowledge study.

> 📄 **Paper:** Maghalian M., Veisi S., Mirghafourvand M., Rezaei M., Samad-Soltani T., Naghizadeh A., Ghanbari-Homaie S. *Developing and testing a mobile application for imparting knowledge: the positive birth experience guideline to midwifery students.* BMC Med Educ 25, 577 (2025).
> DOI: [10.1186/s12909-025-07147-1](https://doi.org/10.1186/s12909-025-07147-1) · Open Access

---

## 📱 What it does

The app translates the WHO's intrapartum care recommendations into two learning modes:

- **Flashcard training** — WHO recommendations across labor & birth care, and the first, second, and third stages of labor, plus newborn and postnatal maternal care, delivered as spaced, recurring reminders until the learner confirms mastery.
- **Scenario-based assessment** — seven case-based quiz scenarios (clinically reviewed by ten midwifery/reproductive health experts) where each answer is classified as *recommended*, *not recommended*, or *not feasible given context* — mirroring how the WHO guideline itself frames decisions. A minimum score gate gets learners to review and retry before advancing.

## 🧪 The research behind it

The app was piloted with 30 second- and third-year midwifery students at Tabriz University of Medical Sciences over a 30-day usage window, using a one-group pre/post design:

- **Knowledge gain:** statistically significant improvement in guideline knowledge after 30 days of use (mean difference +4.75, 95% CI 3.56–5.93, p < 0.001), with significant gains in every subsection except postpartum maternal care.
- **App evaluation:** assessed with a DeLone & McLean-based instrument across six dimensions (system, information, and service quality; use; satisfaction; net benefit). Information quality and system quality scored highest; service quality and satisfaction were identified as areas for improvement.

Full methodology, instruments, and results are in the paper — this repo is the app itself, not a data/analysis repo (no datasets are hosted here; see the paper's Data Availability statement).

## 🏗️ Architecture

Built natively in **Kotlin** with **Jetpack Compose**, following Google's recommended **MVVM** pattern:

- **Model** — local on-device data access layer
- **ViewModel** — mediates between data and UI, caching state across configuration changes (e.g. screen rotation)
- **View** — Compose UI layer

## 🚀 Getting started

```bash
git clone https://github.com/sinaveisi/quiz-app.git
cd quiz-app
./gradlew installDebug
```

Requires Android Studio (Giraffe+) and a device/emulator running Android 8.0 (API 26) or higher.

## 📖 Citation

If you use or reference this work, please cite the paper:

```bibtex
@article{maghalian2025positive,
  title   = {Developing and testing a mobile application for imparting knowledge: the positive birth experience guideline to midwifery students},
  author  = {Maghalian, Mahsa and Veisi, Sina and Mirghafourvand, Mojgan and Rezaei, Mansour and Samad-Soltani, Taha and Naghizadeh, Asma and Ghanbari-Homaie, Solmaz},
  journal = {BMC Medical Education},
  volume  = {25},
  pages   = {577},
  year    = {2025},
  doi     = {10.1186/s12909-025-07147-1}
}
```

## 📜 License

This project's source is shared for educational and research purposes. The published article is distributed under [CC BY-NC-ND 4.0](http://creativecommons.org/licenses/by-nc-nd/4.0/) — non-commercial use with attribution, no derivatives of the article itself.

## 👤 Author

**Sina Veisi** — Medical Informatics, Urmia University of Medical Sciences
