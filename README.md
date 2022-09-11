# webova

## İşlevi

webova responsive tasarımlar oluşturmanızı sağlayan bir yapıdır. Bunun yanında işinizi kolaylaştıracak class 'larla daha hızlı tasarım çıkarmanızı sağlar.

sm                | md               | lr
-------------     | -------------    | -------------
450px ve sonrası  | 800px ve sonrası |  1024px ve sonrası

<hr />

### Açıklama
Webova ekranı 12 birime böler. "gr-" ifadesinden sonra gelen ilk değer class 'ın verildiği elemanın kaç birim olacağını, ikinci değer class 'ın verildiği elemanların etrafında ne kadar boşluk olacağını (0, 10px, 20px 'lik boşluk bırakılabilir), üçüncü değer ise hangi ekran çözünürlükleri için geçerli olcağını belirtir. Eğer üçüncü değerde herhangi birşey belirtmezsek tüm ekran çözünürlükleri için geçerli olacaktır

### Örnek Responsive Kodları

```
<div class="grid__box">
  <div class="grid__row">
    <div class="gr-8-20-md gr-6-10"></div>
    <div class="gr-4-20-md gr-6-10"></div>
  </div>
</div>
```

Yukarıdaki kodda 0px 'den 800px 'e kadar 6 birimlik bir boyut oluşturalacaktır, 800px 'den sonrası için class 'ta belirtilen değerler kadarlık boyut 
oluşturalacaktır. Ayrıca "grid__box" yerine "grid__container" 'da kullanılabilir. Aralarındaki fark "grid__box" ekranın tamamını kullanırken, "grid__container" ekranın %85 'lik bir kısmını kullanır.

<hr />

### Örnek Display Özellikleri
1. display = flex, block, inline-block, inline, none, inline-flex, grid, inline-grid
2. align-items = stretch, center, flex-start, flex-end, baseline, initial, inherit
3. justify-content = flex-start, flex-end, center, space-between, space-around, space-evenly, initial, inherit
4. flex-direction = row, row-reverse, column, column-reverse, initial, inherit

Kullanımları örnek kodda gösterildiği gibidir.

```
<div class="d_flex"></div>
<div class="align_flex-start"></div>
<div class="justify_center"></div>
<div class="direction_row"></div>
```

Eğer display özelliklerini yukarıdaki örneğe benzer şekilde kullanırsak tüm ekran çözünürlükleri için geçerli olacaktır. Eğer sadece tek bir çözünürlük için geçerli olsun istiyorsak:
```
<div class="d_none-md"></div>
<div class="align_center-sm"></div>
<div class="justify_space-between-lr"></div>
<div class="direction_column-reverse-md"></div>
```
şeklinde classı belirttikten sonra sonuna '-' ifadesini koyarak çözünürlüğüde belirtmemiz gerek

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
