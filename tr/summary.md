# Özet

## Neden programlama dilleri kullanmalısınız?

Dünyamızda hemen hemen her şey bilgisayarlarla veya bilgisayarlar tarafından yapılıyor, bunu herkes biliyor.  Ancak herkesin bilmediği şey, herkesin programlama dillerini kullanabileceğidir.  Havalı bir Holywood hackerı veya 250 IQ bilişim adamı olmanıza gerek yok.  Bilgisayarlar (yazılım) kim olursanız olun size yardımcı olabilir.  Bir tasarımcıysanız, hangi anahtar kelimeleri kullanabileceğinizi söyleyen bir yazılıma sahip olmayı çok isterdiniz, değil mi?  Ya da bir çevirmen olduğunuzu varsayalım.  Bilgisayarlar ve çeviri yapay zekaları nedeniyle işsiz kalma korkusuyla yaşıyorsunuz.  Neden işini çalmalarını bekliyorsun?  İşinizi geliştirmek için bunları kullanın.

## Neden bunları öğrenmelisiniz?

Bilgisayarların işlerimizi almasına izin vermeyeceğimiz, ancak onları bizim için kullanacağımız konusunda anlaştığımıza inanıyorum.  Peki, bunu nasıl yapacağız?  İhtiyacımız olan her yazılım ve komut dosyası için yüzlerce dolar harcayacak mıyız?  Kendimize bir programcı mı tutacağız?  Hayır, programları nasıl yazacağınızı ve kullanacağınızı kendiniz öğrenmelisiniz.

Korkma, zor değil.  Aslında çocuk oyuncağı.  Ayrıca, ulaşmak için bir hedefiniz var.  Bu, işleri sizin için daha da kolaylaştıracaktır.  Kim bilir, bir gün sen de programcı olabilirsin.  Şimdi başla, gerisi gelecektir.

## Nereden başlamalıyım?

Peki.  Programlama dillerinin ne olduğunu ve neden öğrenmeniz gerektiğini öğrendiniz.  Ancak piyasada yaklaşık 700 programlama dili var ve kimse işini kaybetmemek veya onlardan yardım almak için hepsini kullanmayı öğrenemez.

Peki, programlama dillerini kullanabilen bu insanlar ne yapıyor?  En çok kullanacaklarını ve yararlanacakları dili kullanmayı öğrenirler.  Sabit ve veri bilimi ile uğraşmak istiyorsanız Python öğrenmeli veya çalıştırılabilir programlar oluşturmak istiyorsanız C vb. dilleri öğrenmelisiniz.

**AMA BURADA BİR OYUN DEĞİŞTİRİCİ VAR: ONE.**

İster bir web sitesi oluşturmak, ister çalıştırılabilir bir program yazmak olsun, tüm amaçlarınız için **One** öğrenmelisiniz.

## One nedir?

One açık kaynaklı, kendi kendine barındırılan, önyükleme yapan bir programlama dilidir. [Max](github.com/BaseMax), [John](github.comjbampton) ve katkıcılarımızla birlikte geliştirilmeye başlandı.

Adı One'dır (Tek) çünkü dilin amacı, kullanıcılara çözmeleri gereken her türlü problem için öğrenmeleri ve kullanmaları için tek bir programlama dili sağlamaktır.

## One'ı kullanmaya başlama

One size bir rüya gibi geldi ve ilginizi çekti ama nereden başlayacağınızı bilmiyorsunuz. Bu **One ile Başlarken** kılavuzunu okuyarak buradan başlayabilirsiniz.

<!--
We should add a section here about installing One
-->

### Programlama dilleri ne yapar?

Üç kişi olduğunu hayal edin: Fransızca, İngilizce ve çevirmen.  Fransız adam İngilizce bilmiyor ve İngiliz adam Fransızca bilmiyor.  İngiliz adamın bir şeyler yapması gerekiyor ama görevinin ne olduğunu bilmiyor.  Görevi ona Fransız adam tarafından söylenmeli ama İngilizce konuşamıyor.  Yani birbirlerini anlamak için bir tercümana ihtiyaçları var.

Bir programlama dili, söylediğiniz her şeyi bilgisayarın diline çeviren bir çevirmen gibidir.  Böylece bilgisayar sizi anlayabilir ve emirlerinizi yerine getirebilir.  Bir dil olduğu için kendine has gramer kuralları vardır ve biz ona "sözdizimi" (syntax) diyoruz.

<!--
### The Syntax of One
the syntax part should be added here

### One'nin Sözdizimi
sözdizimi parçası buraya eklenmelidir
-->

### Girdi ve çıktı nedir (Input Output)?

Bilgisayarlar da duyabilir ve konuşabilir.  Bizimle bu şekilde iletişim kuruyorlar.  Elbette mikrofonunuz ve web kameranız hakkında konuşmuyoruz.  O zaman bizimle nasıl iletişim kuruyorlar?  Girdiler ve çıktılar ile.

Girdi, bilgisayarların bir şeyler yapmasını sağlamak için yaptığınız her şeydir.  Örneğin, klavyede bir tuşa basmak bir girdidir veya farenizle tıklamak bir girdidir.

Çıktı, bilgisayarınızın verdiği tepkidir.  Masaüstünüzdeki bir dosyaya tıkladığınızda bilgisayara bir girdi verirsiniz ve karşılığında bilgisayar o dosyayı açarak size bir çıktı verir.

Bu mantığı anlamak önemlidir ve bu sizin için işleri daha kolay hale getirecektir.

### Değişkenler nedir?

Değişkenler, değerleri depolamak için kullanılan kutulardır.

Çevirmen benzetmesini hatırlıyor musunuz?  Fransızca bir kelime her söylendiğinde tercüman o kelimeyi aklında tutar ve gerektiğinde geri verir.

Programlama dillerinde verileri depolamak ve gerektiğinde kullanmak için değişkenler oluşturabiliriz.

```text
merhaba = bonjour
araba = voiture
aşk = amour
```

Yukarıdaki örnekte, `merhaba` değişkenin adıdır ve `bonjour` içinden dönen (geri gelen) değerdir. Bu bilgiyi aklımızda tutuyoruz çünkü gelecekte buna ihtiyacımız olacağına inanıyoruz.

<!--
Assigning value to a variable section should be added here.
Variable types section should be added here.

Bir değişkene değer atama bölümü buraya eklenmelidir.
Değişken türleri bölümü buraya eklenmelidir.
-->

### if / else (eğer / değilse) koşulları nedir?

Bilgisayarlarımızla konuşurken bazı koşullu durumları onlara anlatmamız gerekebilir.  Bu gibi durumlarda if/else deyimlerini kullanırız ve bilgisayarlara birden fazla durum ve birden fazla seçenek veririz.

```python
if hello = bonjour:
    print("'Bonjour' Fransızcada 'Hello' demektir.")
```

Yukarıdaki kodda, bilgisayar  `hello = bonjour` eşit ise `"Bonjour" Fransızcada "Hello" demektir.` Ama ya koşul yerine getirilmezse? Yani eşit değilse, o zaman bilgisayar hiçbir şey yapmaz çünkü yapmasını söylemedik.  Bilgisayara başka bir koşul verelim.

```python
if hello = merhaba:
    print("'Merhaba' means 'Hello' in Turkish)
else:
    print("I don't know the language you are speaking")
```

Bu nedenle, bilgisayara koşul sağlanırsa yürütülecek bir if koşulu ve koşul karşılanmadığında yürütülecek olan bir else koşulu verdik.  Yukarıdaki programı çalıştırıp bilgisayara Fransızca ve Türkçe dışında bir kelime verirsek bilgisayar bize şunu söyleyecektir:
`"I don't know the language you are speaking" (Hangi dili konuştuğunu bilmiyorum)`

If/else ifadeleri temelde böyledir.  İleride bununla ilgili daha çok şey öğreneceksiniz ama unutmayın, bu bir başlangıç kılavuzudur.

### Fonksiyonlar nedir?

Diyelim ki bir program yazıyorsunuz ama programınızın bir bölümünü birden çok kez kullanmanız gerekiyor.  Aynı satırları tekrar tekrar yazmak sıkıcı ve yorucu olurdu değil mi?  Benimle aynı fikirdeyseniz, fonksiyonların nasıl kullanılacağını öğrenmek isteyebilirsiniz.

Fonksiyonlar temelde programınızda tekrar tekrar kullandığınız küçük bir kod parçasıdır.  Oluşturduğunuz bir özelliğe her ihtiyaç duyduğunuzda aynı satırları yazmak yerine, bir fonksiyon tanımlayabilir ve tekrar tekrar kullanabilirsiniz.  Daha kolay ve daha hızlı.

Çevirmen benzetmemizi hatırlayalım.

```python
if hello = merhaba:
    print("'Merhaba' means 'Hello' in Turkish")
else:
    print("I don't know the language you are speaking")
```

Bu satırları biraz değiştirerek tekrar tekrar yazmak yerine bir fonksiyon tanımlayabilirsiniz.

```python
def translator(word):
    if hello = word:
        print(word + "means 'Hello'.)
    else:
        print("I don't know the word you said")
```

Şimdi, girdi olarak `word` alan ve bu kelimenin `Merhaba` anlamına gelip gelmediğini kontrol eden bir fonksiyon tanımladık.  Doğru ise, ekrana yazacağı şey:

```text
word means 'Hello'. (kelimenin anlamı 'Merhaba'.)
```

Yanlış ise, ekrana yazacağı şey:

```text
I don't know the word you said. (Söylediğin kelimeyi bilmiyorum.)
```
