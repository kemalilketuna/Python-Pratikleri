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
## Elemanları Önceden Belirli Liste Oluşturma  
`listenin ismi` = [ eleman 1, eleman 2, eleman 3 . . . ]
```python
esyalar = ["krem", "tıraş losyonu", "pena"]
```

&nbsp;  
## Tanımlanan Listeye Eleman Ekleme
`listenin ismi`.append(elaman)

````python
esyalar = ["krem", "tıraş losyonu", "pena"]
esyalar.append("gitar teli")
print(esyalar) #--> ['krem', 'tıraş losyonu', 'pena', 'gitar teli']
```