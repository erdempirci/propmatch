# PropMatch

İki sekmeli prop hesabı aracı:

**Seans Risk** — Masaniello tabanlı seans risk hesaplayıcı. Prop hesabının toplam kayıp limitine göre seans kasasını belirler ve her işlemde kaç $ riske atılacağını, lot karşılığını hesaplar.

**Hedge** — Prop challenge'ını gerçek hesapla ters yönde hedge eder. Oran: `h = (Sigorta − Gerçek K/Z) ÷ (Prop bakiye − Patlama seviyesi)`; sigorta = hesap ücreti + masraf payı. Prop patlarsa ücret geri gelir, geçerse gerçek hesaptaki kayıp fonlu hesabın maliyetidir. Trailing (gün sonu / gün içi), kilit seviyesi, tutarlılık kuralı, günlük plan ve futures (NQ→MNQ, ES→MES) yuvarlaması desteklenir.

- Tek dosya: `index.html` (statik, build gerektirmez)
- Veriler tarayıcının localStorage'ında tutulur

Finansal tavsiye değildir. Bazı prop firmaları dışarıdan hedge'i kurallarında yasaklar; kontrol edin.
