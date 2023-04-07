#kilit2
Bilgisayar biliminde Raita algoritması , Boyer-Moore-Horspool algoritmasının performansını artıran bir dizi arama algoritmasıdır . Bu algoritma , Boyer-Moore dizi arama algoritmasına benzer şekilde, kalıp için aranan diziyi önceden işler . Belirli bir dizideki belirli bir alt dizinin arama modeli, Boyer–Moore–Horspool algoritmasından farklıdır. Bu algoritma 1991 yılında Timo Raita tarafından yayınlandı.
Raita algoritması, verilen metindeki her bir örüntü karakterini karşılaştırarak belirli bir "T" metninde bir örüntü "P" arar. Arama aşağıdaki gibi yapılacaktır. Bir metin için pencere "T" uzunluğu "P" olarak tanımlanır.
1.	İlk olarak, desenin son karakteri pencerenin en sağındaki karakterle karşılaştırılır.
2.	Eşleşme varsa, desenin ilk karakteri pencerenin en solundaki karakterle karşılaştırılır.
3.	Tekrar eşleşirlerse, desenin orta karakterini pencerenin orta karakteriyle karşılaştırır.
Ön kontroldeki her şey başarılı olursa, orijinal karşılaştırma ikinci karakterden son bir karaktere kadar başlar. Algoritmanın herhangi bir aşamasında bir uyumsuzluk varsa, ön işleme aşamasında hesaplanan kötü karakter kaydırma işlevini gerçekleştirir. Kötü karakter kaydırma işlevi, Boyer-Moore-Horspool algoritmasında önerilenle aynıdır. [1]
Benzer bir ön kontrolün modern bir formülasyonu , bir lineer/ikinci dereceden dizi eşleyici olan , libc++ ve libstdc++'da bulunur . memcmp"Orijinal karşılaştırmada" karakterleri atlamamak için iyi optimize edilmiş bir sürümünün varsayılması , modelin hizalanması muhtemel olduğundan daha verimli olma eğilimindedir. [2]

