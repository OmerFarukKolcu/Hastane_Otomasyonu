# Hastane_Otomasyonu
Konsol üzerinde çalışan hastane otomasyonu. 
Hastane otomasyonu. Ödevin güncel konularla ilişkisi olması bakımından COVID-19 hastaları ağırlıklı düzenleme yapıldı.

Yeni bir kayıt açabilmeniz için yeni_kayit fonksiyonunu kullanıldı. Kayıt olan kişi aynı fonksiyonun içerisinde dosyalama işlemlerine ve belirli bir listeye yazılma tabi tutuluyor. Hastanın COVID-19 hastası olup olmadığını corona_kontrol() fonksiyonu ile kontrol ediyoruz. Bu fonksiyon da aynı şekilde kullanımı kullanıcıya bırakılmayan bir fonksiyon. Eğer hastanın COVID-19 teşhisi varsa yeni bir dosyalama yapılır ve bu dosya da sadece COVID-19 teşhisli hastalar tutulur. Bu dosyanın uzunluğuna göre de 150 olarak belirlenmiş , COVID-19 teşhisli hastalara ayrılmış yatak sayısı tekrar belirlenir.
Kişi hakkında ki kayıtların her zaman bulunabilir olması için kayıt silme işlemi yerine kayıt arşivleme işlemi yapılır. Bu işlem yapılırken kayit_arsivleme() fonksiyonu kullanıldı COVID-19 teşhisli hastanın kaydı arşivlenirken hastanın hastane ile ilişkisinin neden kesildiği sorulur ve sebebi hastanın iyileşmesi veya vefat etmesi ise verilerin paylaşılması için COVID-19 hastası kişiler iyileşenler_list.txt veya olum_list.txt dosyalarında depolanırlar ve dosyaların uzunluklarına göre iyileşen veya vefat eden hasta sayılarına ulaşılır.

Herhangi bir kayıtlı hastanın durumunu görmek için hasta_kontrol() fonksiyonu kullanıldı.COVID-1 9 teşhisli hastalar hem corona.txt hem de kaytlilar.txt dosyasında kayıtlı olması herksi kontrol edebilme imkanı sunuyor.
İstenildiği gibi menu_m() adında bir fonksiyon yapılarak kullanıcıya hangi işlemleri yapmak istediği soruldu.
Koleksiyon veri tiplerinden liste ve sözcük kullanıldı.
Kayıt güncellenirken hastanın korona olup olmadığı kontrol edildi. Hasta korona ise corona.txt listesinde de güncelleme gerçekleşir.
Kayıt arşivleme fonksiyonunda COVID-19 hastaları için k_kayit_arsivleme() fonksiyonu tanımlanmış ve kullanılmıştır.

FOR ENGLISH:
# Hospital_Automation
Hospital automation running on a console. 
Hospital automation. In order for the assignment to be related to current issues, COVID-19 patients were arranged mainly.

The new_kayit function was used to open a new record. The registered person is subjected to filing operations and writing to a specific list within the same function. We check whether the patient has COVID-19 with the corona_kontrol() function. This function is also a function whose use is not left to the user. If the patient has a COVID-19 diagnosis, a new file is created and only patients with COVID-1 9 diagnoses are kept in this file. According to the length of this file, the number of beds allocated to patients with COVID-1 9 diagnoses, which was set as 1 50, is redetermined.

In order to ensure that the records about the person are always available, kayit_arsivleme() is performed instead of record deletion. While archiving the record of a patient diagnosed with COVID-1 9, it is asked why the patient was disconnected from the hospital, and if the reason is the patient's recovery or death, the COVID-19 patients are stored in the files healers_list.txt or olum_list.txt to share the data, and the number of patients who have recovered or passed away can be accessed according to the length of the files.

The hasta_kontrol() function was used to see the status of any registered patient. The fact that patients with COVID-19 diagnosis are registered in both corona.txt and kaytlilar.txt file allows you to check everyone.
As requested, a function called menu_m() was created to ask the user which operations they want to perform.
The collection data types list and word were used.
When updating the record, it was checked whether the patient was corona or not. If the patient is corona, the corona.txt list is also updated.
In the record archiving function, the k_kayit_arsivleme() function was defined and used for COVID-19 patients.
