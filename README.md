# Herbal-SkinCare-Advisor
A simple AI-inspired herbal skincare advisor 🌿 | Enter your age &amp; skin type, get a personalized herb recommendation with images.
Herbal-SkinCare-Advisor/
│
├── README.md
├── requirements.txt
├── data/
│   ├── chamomile.jpg
│   ├── mint.jpg
│   └── rosemary.jpg
│
├── src/
│   ├── main.py
│   └── herbs_data.jsonimport json
import random
from PIL import Image

# Load herbs data
with open("src/herbs_data.json", "r", encoding="utf-8") as f:
    herbs = json.load(f)

def recommend_herb(age, skin_type):
    skin_type = skin_type.lower()
    if skin_type not in herbs:
        return None, None
    # Randomly pick one herb for diversity
    herb = random.choice(herbs[skin_type])
    return herb["name"], herb["image"]

if __name__ == "__main__":
    print("🌿 Herbal SkinCare Advisor 🌿")
    age = int(input("Enter your age: "))
    skin_type = input("Enter your skin type (oily, dry, sensitive): ")

    herb_name, herb_img = recommend_herb(age, skin_type)
    if herb_name:
        print(f"\nRecommended Herb for you: {herb_name}")
        img = Image.open("data/" + herb_img)
        img.show()
    else:
        print("Sorry, no recommendation for this skin type yet."){
  "oily": [
    {"name": "Mint 🌱", "image": "mint.jpg"}
  ],
  "dry": [
    {"name": "Chamomile 🌼", "image": "chamomile.jpg"}
  ],
  "sensitive": [
    {"name": "Rosemary 🌿", "image": "rosemary.jpg"}
  ]pillow
}# 🌿 Herbal SkinCare Advisor

This project is a simple **AI-inspired herbal recommendation system** for skincare.  
Users can enter their **age** and **skin type**, and the system suggests a suitable **herb** along with its **image**.

---

## 🚀 Features
- Input: **Age** and **Skin Type** (oily, dry, sensitive).
- Output: Herbal recommendation + Image.
- Herbs database stored in JSON format.
- Expandable with more herbs and skin conditions.

---

## 🗂️ Project Structure---

## ⚙️ Installation
```bash
git clone https://github.com/your-username/Herbal-SkinCare-Advisor.git
cd Herbal-SkinCare-Advisor
pip install -r requirements.txtpython src/main.py
