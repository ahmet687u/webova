# Grid

## İşlevi

Grid responsive tasarımlar oluşturmanızı sağlayan bir yapıdır. Bunun yanında işinizi kolaylaştıracak class 'larla daha hızlı tasarım çıkarmanızı sağlar.

xxs           | sm                | md               | lr
------------- | -------------     | -------------    | -------------
0px sonrası   | 450px ve sonrası  | 800px ve sonrası |  1024px ve sonrası

<hr />

### Açıklama
Grid ekranı 12 birime böler. "gr-" ifadesinden sonra gelen ilk değer class 'ın verildiği elemanın kaç birim olacağını, ikinci değer class 'ın verildiği elemanların etrafında ne kadar boşluk olacağını (0, 10px, 20px 'lik boşluk bırakılabilir), üçüncü değer ise hangi ekran çözünürlükleri için geçerli olcağını belirtir.

### Örnek Responsive Kodları

```
<div class="grid__box">
  <div class="grid__row">
    <div class="gr-8-20-md gr-6-10-xxs"></div>
    <div class="gr-4-20-md gr-6-10-xxs"></div>
  </div>
</div>
```

Yukarıdaki kodda 0px 'den 800px 'e kadar 6 birimlik bir boyut oluşturalacaktır, 800px 'den sonrası için class 'ta belirtilen değerler kadarlık boyut 
oluşturalacaktır. Ayrıca "grid__box" yerine "grid__container" 'da kullanılabilir. Aralarındaki fark "grid__box" ekranın tamamını kullanırken, "grid__container" ekranın %85 'lik bir kısmını kullanır.

<hr />

### Örnek Display Özellikleri
1. display = "flex", "block", "inline-block", "inline", "none", "inline-flex"
2. align-items = "center", "flex-start", "flex-end"
3. justify-content = "center", "space-between", "flex-start", "flex-end", "space-around", "space-evenly"

Kullanımları örnek kodda gösterildiği gibidir.

```
<div class="d__flex"></div>
<div class="align__flex-start"></div>
<div class="justify__center"></div>
```

Aşağıdaki kodun karşılığı:
display: flex;
align-items: center;
justify-content: center;

``` 
<div class="flex__center"></div>
```

<hr />

### Örnek Margin Padding Kodları

5px           | 10px          | 15px          | 20px
------------- | ------------- | ------------- | -------------
1             | 2             | 3             |  4

``` 
<div class="m-3"></div>
<div class="mt-1"></div>
<div class="mx-2"></div>
<div class="p-2"></div>
<div class="pb-4"></div>
<div class="py-1"></div>
```
