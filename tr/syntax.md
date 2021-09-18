# Sözdizimi

One'ın sözdizimi, biraz daha basit ve daha akıcı olmakla birlikte, C-benzeri dillerden gelen insanlara aşina olacak şekilde tasarlanmıştır.

Komut dosyaları, `.One` dosya uzantısına sahip düz metin dosyalarında saklanır. Önceden derleme yapılmaz: programlar, tipik bir betik dili gibi yukarıdan aşağıya doğru doğrudan kaynaktan çalıştırılır. (Dahili olarak, programlar verimlilik için bayt koduna derlenir, ancak bu bir uygulama ayrıntısıdır.)

## Yorum satırları

Satır yorumları şununla başlar: `//` ve satırın sonunda biter.:

```
// Bu bir yorum satırı (programda çalıştırılmayacak).
```

<!-- prettier-ignore-start -->
Blok yorumları /* ile başlar ve */ ile biter.  Birden çok satıra yayılabilirler: <!-- markdownlint-disable MD037 -->
<!-- prettier-ignore-end -->

```
/* Bu
   bir
   çok-satırlı
   yorum. */
```

C'den farklı olarak, blok yorumları One'da iç içe girebilir:

```
/* Bu bir /* iç içe girmiş */ yorum satırı. */
```

Bu kullanışlıdır, çünkü kod zaten blok yorumları içeriyor olsa bile, bir kod bloğunun tamamını kolayca yorumlayabilmenizi sağlar.
Ayrılmış kelimeler #

Bir dilin üslubu hakkında hızlı bir fikir edinmenin bir yolu, hangi kelimeleri sakladığını görmektir. İşte One'ın sahip olduğu şeyler:

as break class construct continue else false for foreign if import
in is null return static super this true var while

## Tanımlayıcılar

Adlandırma kuralları diğer programlama dillerine benzer. Tanımlayıcılar bir harf veya alt çizgi ile başlar (rakam ile başlayamaz) ve harf, rakam ve alt çizgi içerebilir. Büyük küçük harf duyarlıdır.

```
hi
camelCase
PascalCase
_under_score
abc123
ALL_CAPS
```

Alt çizgi (`_`) ile başlayan tanımlayıcılar One'da özeldir. Sınıflarda alanları belirtmek için kullanılırlar.

## Yeni satırlar (alt satır)

Yeni satırlar (\n) One'da anlamlıdır. İfadeleri ayırmak için kullanılırlar:

```
// İki ifade:
System.print("merhaba") // Yeni satır.
System.print("hoşçakal")
```

Ancak bazen, bir ifade tek bir satıra sığmaz ve ortada yeni bir satırın sıkışması onu açar. Bununla başa çıkmak için One'ın çok basit bir kuralı vardır: Bir ifadeyi sonlandıramayan herhangi bir belirteçten sonraki yeni satırı yok sayar.

```
System.print( // Buradaki yeni satır yoksayılır.
    "hi")
```

Pratikte bu, her ifadeyi kendi satırına koyabileceğiniz ve çok fazla sorun yaşamadan gerektiğinde satırlar arasında sarabileceğiniz anlamına gelir.
