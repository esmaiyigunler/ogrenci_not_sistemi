ogrenciBilgileri = [{"isim": "Elif", "not": 95}, {"isim": "Ece", "not": 90}, {"isim": "Ecrin", "not": 89}]

def ogrenciEkle(ogrenciBilgileri, ogrenciAdi, notu):
    yeniOgrenci = {"isim": ogrenciAdi, "not": notu}
    ogrenciBilgileri.append(yeniOgrenci)
    print(ogrenciAdi + " isimli öğrenci " + str(notu) + " notuyla listeye eklendi.")

def notGuncelle(ogrenciBilgileri, ogrenciAdi, yeniNot):
    for ogrenci in ogrenciBilgileri:
        if ogrenci["isim"] == ogrenciAdi:
            ogrenci["not"] = yeniNot
            print(ogrenciAdi + " isimli öğrencinin notu: " + str(yeniNot) + " olarak güncellendi.")
            return
    print(ogrenciAdi + " isimli öğrenci bulunamadı.")

def notSil(ogrenciBilgileri, ogrenciAdi):
    for ogrenci in ogrenciBilgileri:
        if ogrenci["isim"] == ogrenciAdi:
            ogrenciBilgileri.remove(ogrenci)
            print(ogrenciAdi + " isimli öğrencinin notu silindi.")
            return
    print(ogrenciAdi + " isimli öğrenci bulunamadı.")

def notGoruntuleme(ogrenciBilgileri):
    for ogrenci in ogrenciBilgileri:
        print("Öğrenci: " + ogrenci["isim"] + ", Not: " + str(ogrenci["not"]))

def enYuksekNot(ogrenciBilgileri):
    if not ogrenciBilgileri:
        print("Liste boş.")
        return
    enYuksek = max(ogrenciBilgileri, key=lambda x: x["not"])
    print("En yüksek nota sahip öğrenci: " + enYuksek["isim"] + ", Not: " + str(enYuksek["not"]))

while True:
    print("\nÖğrenci Not Sistemine Hoş Geldiniz")
    print("1. Öğrenci ismi ve not eklemek")
    print("2. Not güncelleme")
    print("3. Not silme")
    print("4. Not görüntüleme")
    print("5. En yüksek notu görüntüleme")
    print("6. Çıkış")

    secim = int(input("Lütfen yapmak istediğiniz işlemi seçiniz (1-6): "))

    if secim == 1:
        ogrenciAdi = input("Eklemek istediğiniz öğrencinin adını yazınız: ")
        notu = int(input("Eklemek istediğiniz öğrencinin notunu yazınız: "))
        ogrenciEkle(ogrenciBilgileri, ogrenciAdi, notu)
    elif secim == 2:
        ogrenciAdi = input("Notunu güncellemek istediğiniz öğrencinin adını yazınız: ")
        yeniNot = int(input("Öğrencinin güncel notunu giriniz: "))
        notGuncelle(ogrenciBilgileri, ogrenciAdi, yeniNot)
    elif secim == 3:
        ogrenciAdi = input("Notunu silmek istediğiniz öğrencinin adını yazınız: ")
        notSil(ogrenciBilgileri, ogrenciAdi)
    elif secim == 4:
        notGoruntuleme(ogrenciBilgileri)
    elif secim == 5:
        enYuksekNot(ogrenciBilgileri)
    elif secim == 6:
        print("Sistemden çıkış yapılıyor.")
        break
    else:
        print("Geçersiz bir seçim yaptınız...")
