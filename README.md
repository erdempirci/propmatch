# PropMatch

İki sekmeli prop hesabı aracı:

**Seans Risk** — Masaniello tabanlı seans risk hesaplayıcı. Prop hesabının toplam kayıp limitine göre seans kasasını belirler ve her işlemde kaç $ riske atılacağını, lot karşılığını hesaplar.

**Hedge (altın)** — Prop challenge'ını gerçek hesapta ters yönde altın pozisyonuyla hedge eder. Prop bakiyesi, gerçek bakiye ve prop lotu girilir; gerçek hesapta açılacak lot (0,01 adımlı) çıkar. Oran: `h = (Ücret + Masraf payı − Gerçek K/Z) ÷ (Prop bakiye − Patlama seviyesi)`. Prop patlarsa ücret geri gelir, geçerse gerçek hesaptaki kayıp fonlu hesabın maliyetidir. Varsayılan: prop 1 lot = 10$/1$ hareket, gerçek 1 lot = 100$/1$ hareket (ayarlardan değişir).

- Tek dosya: `index.html` (statik, build gerektirmez)
- Veriler tarayıcının localStorage'ında tutulur

Finansal tavsiye değildir. Bazı prop firmaları dışarıdan hedge'i kurallarında yasaklar; kontrol edin.
