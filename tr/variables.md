# Değişkenler (Variables)

Değişkenler, bir bilgisayar programında referans alınacak ve işlenecek bilgileri depolamak için kullanılır.  Ayrıca, verileri tanımlayıcı bir adla etiketlemenin bir yolunu sağlarlar, böylece programlarımız okuyucu ve kendimiz tarafından daha net anlaşılabilir.  Değişkenleri bilgi içeren kaplar olarak düşünmek yararlıdır.  Tek amaçları, verileri bellekte etiketlemek ve depolamaktır.  Bu veriler daha sonra programınız boyunca kullanılabilir.

## Değişken Tanımlama (Oluşturma)

```
<değişken türü> <değişken adı> = <değeri>;
```

Burada tür, Bir'in türlerinden biridir (int veya String gibi) ve değişken, değişkenin adıdır (x veya ad gibi).  Değişkene değer atamak için eşittir işareti kullanılır.

### Örnek

```
String metin = "One harika!"
System.print(metin)
```

Mevcut bir değişkene yeni bir değer atarsanız, önceki değerin üzerine yazacağını unutmayın:

### Örnek

```
String metin = "One güzel bir dil!"
metin = "One havalı :)"
System.print(metin) // Çıktı şöyle olacaktır: One havalı :)
```

## Diğer türler

One'da farklı değişken türleri vardır, örneğin:

### Örnek

```
int number = 10;
float floatNumber = 10.99f;
char letter = 'O';
boolean bool = true;
String metin = "One harika!";
```

## Birden Fazla Değişken Tanımlama

Aynı türden birden fazla değişken bildirmek için virgülle ayrılmış bir liste kullanın:

### Örnek

```
int a = 10, b = 15, c = 20
System.print(a)
System.print(b)
System.print(c)
```
