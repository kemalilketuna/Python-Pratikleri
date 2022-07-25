# Liste Methotları ve Listelerde İşlemler

## Boş Bir Listeyi Tanımlama
1. Köşeli parantez kullanarak tanımlanabilir.  
`listenin ismi` = [ &nbsp;]  
  
2. list() anahtar kelimesini kullanarak tanımlanabilir.  
`listenin ismi` = list()
    
&nbsp;    
```python
urunler = []
urunler = list()
```

&nbsp;  
## Elemanları Önceden Belirli Bir Liste Oluşturma  
`listenin ismi` = [ eleman 1, eleman 2, eleman 3 . . . ]
```python
esyalar = ["krem", "tıraş losyonu", "pena"]
```

&nbsp;  
## Tanımlanan Listeye Eleman Ekleme
`listenin ismi`.append(elaman)

```python
esyalar = ["krem", "tıraş losyonu", "pena"]
esyalar.append("gitar teli")
print(esyalar) #--> ['krem', 'tıraş losyonu', 'pena', 'gitar teli']
```

## Listedeki Tüm Elemanları Silme
`listenin ismi`.clear()

```python
print(esyalar) #--> ['krem', 'tıraş losyonu', 'pena', 'gitar teli']
esyalar.clear()
print(esyalar) #--> []
```

&nbsp;   
## Listeyi Kopyalama
Eğer bir listeyi kopyalamak için başka bir listeye atama yaparsak ilk listede yapılan değişikler ikinci liste için de geçerli olur.
  
Örnek:
```python
liste1 = ["nescafe", "süt", "cici bebe"]
liste2 = liste1
print(liste2) #--> ["nescafe", "süt", "cici bebe"]
liste1[0] = "kola" # listedeki 1. eleman "kola" ile değişiyor.
del liste1[2] # listedeki 3. eleman siliniyor.
print(liste1) #--> ['kola', 'süt', 'cici bebe']
print(liste2) #--> ['kola', 'süt', 'cici bebe']
```
liste1'deki tüm değişikler görüldüğü gibi liste2 için de uygulandı.  
Eğer liste1'in liste2'ye kopyalamak istiyorsak ama liste1'deki değişikliklerin liste2'ye uygulanmasını istemiyorsak `listenin ismi`.copy() methodunu kullanmamız gerekiyor.

Örnek:
```python
liste1 = ["nescafe", "süt", "cici bebe"]
liste2 = liste1.copy()
print(liste2) #--> ["nescafe", "süt", "cici bebe"]
liste1[0] = "kola" # listedeki 1. eleman "kola" ile değişiyor.
del liste1[2] # listedeki 3. eleman siliniyor.
print(liste1) #--> ['kola', 'süt', 'cici bebe']
print(liste2) #--> ["nescafe", "süt", "cici bebe"]
```
Görüldüğü gibi `listenin ismi`.copy() methodunu kullanınca liste1 kopyalandı ama liste1'deki değişikler liste2 için geçerli olmadı.

