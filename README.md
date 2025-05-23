# Лабораторные работы по курсу "Методы, средства и технологии мультимедиа"

**Студент:** Громов Тимофей Сергеевич 
**Группа:** М8О-407Б-21  

---

### Лабораторная работа № 6 – Исследование моделей классификации

**Датасет:** [Intel Image Classification](https://www.kaggle.com/datasets/puneet6060/intel-image-classification)  
**Метрики:** Accuracy, Precision, Recall, F1-score

**Итог:**

| Model       | Accuracy | Macro F1 | Precision | Recall |
|-------------|---------:|---------:|----------:|-------:|
| ResNet18    | 0.967    | 0.964    | 0.965     | 0.962  |
| ViT-B16     | 0.986    | 0.985    | 0.985     | 0.986  |
| EffNetV2-S  | 0.960    | 0.959    | 0.958     | 0.960  |
| DeiT-S      | 0.984    | 0.983    | 0.982     | 0.984  |
| SimpleCNN   | 0.860    | 0.854    | 0.855     | 0.853  |
| TinyViT     | 0.777    | 0.770    | 0.771     | 0.769  |

---

### Лабораторная работа № 7 – Проведение исследований моделями семантической сегментации

**Датасет:** [CamVid (road scenes)](https://www.kaggle.com/datasets/carlolepelaars/camvid)  
**Метрики:** Dice, mIoU, Pixel Accuracy

**Итог:**

| Model               | mIoU  | Dice   | PixelAcc |
|---------------------|-------:|--------:|----------:|
| UNet (ResNet18)     | 0.805 | 0.9636 | 0.9318   |
| SimpleUNet          | 0.681 | 0.8302 | 0.8600   |
| Improved SimpleUNet | 0.698 | 0.8405 | 0.8700   |

---

### Лабораторная работа № 8 — Проведение исследований моделями обнаружения и распознавания объектов

**Датасет:** [Pothole Detection](https://www.kaggle.com/datasets/andrewmvd/pothole-detection)  
**Метрики:** Precision, Recall, mAP@0.5, mAP@0.5:0.95

**Итог:**

| Model                  | Precision | Recall | mAP@0.5 | mAP@0.5:0.95 |
|------------------------|----------:|--------:|--------:|--------------:|
| YOLOv8-nano (baseline) | 0.681     | 0.574   | 0.642   | 0.384        |
| YOLOv8-small (improved)| 0.739     | 0.503   | 0.601   | 0.352        |
| SSD-Lite (custom impl) | 0.225     | 0.150   | 0.180   | 0.090        |

---

В рамках каждой лабораторной работы были построены бейзлайны, предложены улучшения и реализованы собственные архитектуры. Эксперименты проводились на CPU с ограничением времени обучения до 30 минут.
