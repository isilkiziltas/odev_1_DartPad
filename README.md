//1. çift sayıların sayısını bulma
void main() {
  List<int> numbers = [5, 10, 15, 20, 25];

  int ciftSayiSayisi = numbers.where((sayi) => sayi % 2 == 0).length;

  print("Çift sayıların sayısı: $ciftSayiSayisi"); // Çıktı: Çift sayıların sayısı: 2


//2. Map Değerlerinin Toplamını Kontrol Etme

  Map<String, int> notlar = {'Ali': 4, 'Veli': 6, 'Ahmet': 8};

  int toplam = notlar.values.reduce((a, b) => a + b);

  if (toplam > 10) {
    print("Büyük");
  } else {
    print("Küçük");
  }
  //3. Set İçerisinde 10 Sayısı Kontrolü
   Set<int> sayilar = {1, 2, 3, 4, 5, 10, 15};
  
  if (sayilar.contains(10)) {
    print('10 bulundu');
  } else {
    print('10 bulunamadı');
  }
}
