# SAP--ABAP-PROJECT
ABAP: Customer Discount Calculation Engine 🛒
Bu proje, SAP sistemleri üzerinde müşteri alışveriş verilerini işleyen ve belirli iş kurallarına (business rules) göre dinamik indirim oranları hesaplayan bir ABAP raporudur.

📌 Proje Hakkında
Bu rapor, veri analitiği ve kurumsal kaynak planlama (ERP) süreçlerinin kesişiminde yer alan temel bir finansal hesaplama örneğidir. Kullanıcıdan alınan girdi verilerini (Müşteri adı ve tutar) değerlendirerek, önceden tanımlanmış eşik değerlerine göre en uygun indirim oranını belirler ve nihai ödeme tablosunu oluşturur.

🛠 Teknik Özellikler
      Dil: ABAP (Advanced Business Application Programming)
      Sistem: SAP S/4HANA / ECC
      Kullanılan Yapılar: * PARAMETERS: Kullanıcı etkileşimli veri girişi.
      IF...ELSEIF...ENDIF: Koşullu mantık ve segmentasyon.
      P (Packed Number): Finansal veriler için yüksek hassasiyetli sayısal veri tipi.

📊 İndirim Mantığı (Business Logic)

Program, alışveriş tutarını üç ana kategoriye ayırarak işlem yapar:
Alışveriş Tutarı	İndirim Oranı	Açıklama
0 - 1.000 TL	%0	İndirim uygulanmaz.
1.001 - 5.000 TL	%5	Standart indirim uygulanır.
5.000 TL Üzeri	%10	Premium müşteri indirimi uygulanır.

🚀 Kurulum ve Kullanım

    SAP sisteminizde SE38 işlem koduna (T-Code) gidin.

    Program adı olarak ZCUSTOMER_DISCOUNT yazın ve "Oluştur" butonuna tıklayın.

    Paylaşılan kaynak kodu editöre yapıştırın.

    Kaydedip aktif ettikten sonra F8 ile çalıştırın.

    Müşteri adını ve tutarı girerek sonuçları rapor ekranında görüntüleyin.

📝 Çıktı Örneği
Plaintext

Müşteri Adı : Mercan Köseoğlu
Alışveriş Tutarı : 6.000,00
İndirim : 600,00
Toplam Ödenecek : 5.400,00

Geliştiren: Mercan Köseoğlu
Data Analyst & SAP ABAP Consultant
