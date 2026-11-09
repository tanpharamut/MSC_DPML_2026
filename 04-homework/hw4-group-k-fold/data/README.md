# ข้อมูลของ HW4

ไฟล์ CSV สองไฟล์ในโฟลเดอร์นี้ **ไม่ได้เก็บใน Git** (อยู่ใน `.gitignore`)
เพราะขนาดเกินเกณฑ์ที่ GitHub แนะนำ — เก็บไว้เฉพาะในเครื่อง

| ไฟล์ | ขนาด | จำนวนแถว | real (0) | fake (1) |
|---|---:|---:|---:|---:|
| `train_data.csv` | ~96 MB | 1,317,236 | 320,475 | 996,761 |
| `test_data.csv` | ~29 MB | 329,309 | 80,410 | 248,899 |

## คอลัมน์

**`train_data.csv`**

```
Image Path, Predicted Gender, Predicted Age, Skin Tone, Target,
Skin Tone Group, Intersection
```

**`test_data.csv`** (มีคอลัมน์ reliability เพิ่มมาสองคอลัมน์)

```
Image Path, Predicted Gender, Predicted Age, Reliability Score Gender,
Reliability Score Age, Skin Tone, Target, Skin Tone Group, Intersection
```

## วิธีใช้

วาง CSV ไว้ในโฟลเดอร์นี้ แล้วตั้งค่า `CSV_PATH` ใน notebook
(`../notebooks/ai-face-group-kfold-v5.ipynb`) ให้ชี้มาที่ไฟล์ เช่น

```python
CSV_PATH = Path("../data/train_data.csv")
```

Notebook ใช้แค่คอลัมน์ `Image Path` (สำหรับดึง group key) และ `Target`
จึงไม่จำเป็นต้องมีไฟล์รูปภาพจริงก็รันได้
