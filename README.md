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
<div class="gr_box">
  <div class="gr_row">
    <div class="gr-8-20-md gr-6-10-sm"></div>
    <div class="gr-4-20-md gr-6-10-sm"></div>
  </div>
</div>
```

Yukarıdaki kodda 0px 'den 800px 'e kadar 6 birimlik bir boyut oluşturalacaktır, 800px 'den sonrası için class 'ta belirtilen değerler kadarlık boyut 
oluşturalacaktır. Ayrıca "gr_box" yerine "gr_container" 'da kullanılabilir. Aralarındaki fark "gr_box" ekranın tamamını kullanırken, "gr_container" ekranın %85 'lik bir kısmını kullanır.

<hr />

### Diğer Özellikler
1. display = flex, block, inline-block, inline, none, inline-flex, grid, inline-grid
2. align-items = stretch, center, flex-start, flex-end, baseline
3. justify-content = flex-start, flex-end, center, space-between, space-around, space-evenly
4. flex-direction = row, row-reverse, column, column-reverse
5. box-sizing = border-box, content-box
6. position = static, sticky, absolute, relative, fixed

Kullanımları örnek kodda gösterildiği gibidir.

```
<div class="d_flex"></div> <!-- display: flex -->
<div class="ai_flex-start"></div> <!-- align-items: flex-start -->
<div class="jc_center"></div> <!-- justify-content: center -->
<div class="dir_row"></div> <!-- flex-direction: row -->
<div class="bs_border-box"></div> <!-- box-sizing: border-box -->
<div class="pos_fixed"></div> <!-- position: fixed -->
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
