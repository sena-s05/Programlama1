#Programlama 1 - Döngülü Hesap Makinesi Ödevi

print("Döngülü Hesap Makinesi")

while True:    #Programın sonsuz bir döngüye girmesini sağlar. İşlem bittiğinde menü tekrar ekrana gelir.
    print("--------------------------------")
    print("+ Toplama (+)")
    print("- Çıkarma (-)")
    print("* Çarpma (*)")
    print("/ Bölme (/)")
    print("** Üs Alma (**)")
    print("// Tam Bölme (//)")
    print("q Çıkış")  #Kullanıcının programdan istediği zaman çıkabilmesi için quit.
    print("--------------------------------")

    #Kullanıcıdan işlem seçimi alıyoruz.
    secim = input("Yapmak istediğiniz işlemi girin (+, -, *, /, **, // veya çıkış için 'q'): ")
    
    #Çıkış koşulu
    if secim.lower() == 'q':  #secim.lower() sayesinde kullanıcı q yerine Q girse bile program çalışır.
        print("Hesap makinesinden çıkılıyor.")
        break  #Döngüyü kır.

    # Geçerli bir işlem seçilip seçilmediğini kontrol ediyoruz.
    if secim in ('+', '-', '*', '/', '**', '//'):  #secim değişkeninin değeri, parantez içindeki karakterlerden biriyle eşleşiyorsa 'in' (yani onların içindeyse).
        try:  #try ve except ayrılmaz ekip arkadaşı. İşlemleri yapmayı dene (try), eğer kullanıcı harf girerse ve değer hatası (except ValueError) çıkarsa programı kapatma, uyarıyı göster.
        
            # Kullanıcıdan sayıları alıyoruz.
            sayi1 = float(input("Birinci sayıyı girin: ")) #float küsüratlı sayılar için.
            sayi2 = float(input("İkinci sayıyı girin: "))  #float küsüratlı sayılar için.
            print("--------------------------------")
            
            #Toplama 
            if secim == '+':
                sonuc = sayi1 + sayi2
                print(f"Sonuç: {sayi1} + {sayi2} = {sonuc}")
                
            #Çıkarma
            elif secim == '-':  #if değilse elif.
                sonuc = sayi1 - sayi2
                print(f"Sonuç: {sayi1} - {sayi2} = {sonuc}")
                
            #Çarpma
            elif secim == '*':
                sonuc = sayi1 * sayi2
                print(f"Sonuç: {sayi1} * {sayi2} = {sonuc}")
                
            #Bölme
            elif secim == '/':
                if sayi2 != 0:  #sayi2 0 değilse işlemi yap.
                    sonuc = sayi1 / sayi2
                    print(f"Sonuç: {sayi1} / {sayi2} = {sonuc}")
                else:  #if ya da elif değilse else.
                    print("Hata: Bir sayı 0'a bölünemez!")  #sayi2 0 ise.
                
            #Üs Alma
            elif secim == '**':
                sonuc = sayi1 ** sayi2
                print(f"Sonuç: {sayi1} ** {sayi2} = {sonuc}")
               
            #Tam Bölme
            elif secim == '//':
                if sayi2 != 0:
                    sonuc = int(sayi1 // sayi2)  #sonucun tam sayı (integer) çıkması için int.
                    print(f"Sonuç: {int(sayi1)} // {int(sayi2)} = {sonuc}") 
                else:
                    print("Hata: Bir sayı 0'a bölünemez!")
                    
        except ValueError:  #try ve except ayrılmaz ekip arkadaşı. İşlemleri yapmayı dene (try), eğer kullanıcı harf girerse ve değer hatası (except ValueError) çıkarsa programı kapatma, uyarıyı göster.
            print("Hata: Lütfen geçerli bir sayı girin!")
    else:
        print("Geçersiz bir seçim yaptınız! Lütfen +, -, *, /, **, // veya çıkış için 'q' girin.")