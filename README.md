# GuessNumber.py

# this is a test code that i should write without looking for informations
# guess number
# ley's begin

import random

name = str(input("Ismingizni kiriting:  "))
print(f"Assalomu alaykum {name}, Bu o'yinda koputer o'ylagan sonni topishingiz kerak bo'ladi")
print("Qani boshladik")

comp = random.randint(0, 10)
effort = 3

while effort > 0:
    user = int(input("Iltimos raqamni kiriting (0 dan 10 gacha): "))

if user > comp:
   effort -= 1
   print(f"Kompyuter kichikroq sonni o'ylagan edi! Urinish soni: {effort}")
elif user < comp:
   effort -= 1
   print(f"Kompyuter kattaroq sonni o'ylagan edi! Urinish soni: {effort}")
else:
    print("Tabriklaymiz, siz to'g'ri topdingiz!")
    print(f"Kompyuter {comp} sonini o'ylagan edi!")
    break

if effort == 0:
    print("Afsuski siz topa olmadingiz!")
    print(f"Kompyuter {comp} sonini o'ylagan edi!")
