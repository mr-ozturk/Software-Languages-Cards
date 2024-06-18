İNDEX.HTML KODLARININ AÇIKLAMASI:
<html lang="en">: Belgenin dilini İngilizce olarak belirtir.
<meta charset="UTF-8" />: Karakter kodlamasını UTF-8 olarak ayarlar.
<meta http-equiv="X-UA-Compatible" content="IE=edge" />: Tarayıcının en iyi uyumluluk modunda çalışmasını sağlar.
<meta name="viewport" content="width=device-width, initial-scale=1.0" />: Sayfanın, farklı cihazlarda düzgün görüntülenmesini sağlar.
<title>EDUCATION CARDS</title>: Sayfa başlığını belirler.
<link rel="stylesheet" href="style.css" />: Harici bir CSS dosyasını sayfaya dahil eder.

<body>: Belgenin gövde kısmını tanımlar.
<section class="hero">: Hero bölümü, genellikle büyük görseller veya videolar içeren, sayfanın dikkat çeken üst kısmıdır.
<video autoplay loop muted plays-inline class="back-video">: Otomatik oynatılan, döngüye alınmış ve sessize alınmış bir video tanımlar.
<source src="Video/video.mp4"/>: Videonun dosya yolunu belirtir.
<section class="content">: İçerik bölümü.
<h1><i>EVERYTHING ABOUT THE SOFTWARE</i></h1>: Başlık metni, eğik yazı tipiyle.
<a href="Hover Card/index.html" target="_blank"><i>CLICK HERE TO EXPLORE</i></a>: "Hover Card/index.html" sayfasına yeni bir sekmede açılan bağlantı.

Bu yapı, görsel olarak etkileyici bir arka plan videosu ve üzerinde bir başlık ile bağlantı içeren basit bir web sayfası oluşturur. 
CSS dosyası (style.css) bu öğelerin stilini belirler, ancak bu dosya burada yer almıyor. Bu dosyanın içeriği, sayfanın görsel düzenini ve tasarımını daha da özelleştirmek için kullanılacaktır.

STYLE.CSS KODLARININ AÇIKLAMASI:
Genel Stil Ayarları:
padding: 0;: Tüm öğelerin iç boşluklarını sıfırlar.
margin: 0;: Tüm öğelerin dış boşluklarını sıfırlar.
box-sizing: border-box;: Kenarlık ve dolgu değerlerinin öğenin toplam genişlik ve yüksekliğine dahil edilmesini sağlar.
font-family: sans-serif;: Tüm metinlerin sans-serif yazı tipini kullanmasını sağlar.

Hero Bölümü Stilleri:
width: 100%;: Hero bölümünün genişliğini %100 yapar.
height: 100vh;: Hero bölümünün yüksekliğini tam ekran yüksekliği yapar.
background-image: linear-gradient(rgba(12, 3, 51, 0.3), rgba(12, 3, 51, 0.3));: Hero bölümüne yarı saydam bir koyu mavi gradyan arka plan ekler.
position: relative;: Hero bölümünün konumlandırmasını göreceli yapar.
padding: 0 5%;: Sağ ve sol kenarlıklara %5 boşluk ekler.
display: flex;: Hero bölümünü esnek kutu yapısı kullanarak düzenler.
justify-content: center;: İçeriklerin yatayda ortalanmasını sağlar.
align-items: center;: İçeriklerin dikeyde ortalanmasını sağlar.

İçerik Bölümü Stilleri:
text-align: center;: İçerik bölümündeki metinlerin ortalanmasını sağlar.

Başlık Stilleri:
.content h1 {}: İçerik bölümündeki <h1> etiketleri için geçerlidir.
font-size: 160px;: Başlık metninin boyutunu 160 piksel yapar.
color: #fff;: Metin rengini beyaz yapar.
font-weight: 600;: Metin kalınlığını 600 (yarı kalın) yapar.
transition: 0.5s;: Tüm stil değişikliklerinin 0.5 saniye süresinde gerçekleşmesini sağlar.
.content h1:hover {}: Başlık üzerine gelindiğinde geçerli olur.
-webkit-text-stroke: 2px white;: Metne beyaz bir dış çizgi ekler.
color: transparent;: Metin rengini saydam yapar.

Bağlantı Stilleri:
.content a {}: İçerik bölümündeki <a> etiketleri için geçerlidir.
text-decoration: none;: Bağlantının altını çizer.
display: inline-block;: Bağlantıyı satır içi blok öğesi yapar.
color: #fff;: Bağlantı metninin rengini beyaz yapar.
font-size: 24px;: Metin boyutunu 24 piksel yapar.
border: 2px solid white;: 2 piksel kalınlığında beyaz bir kenarlık ekler.
padding: 14px 50px;: İçeriğe üst-alt 14 piksel, sağ-sol 50 piksel boşluk ekler.
margin-top: 20px;: Üst kenara 20 piksel boşluk ekler.
transition: 0.5s;: Tüm stil değişikliklerinin 0.5 saniye süresinde gerçekleşmesini sağlar.
.content a:hover {}: Bağlantı üzerine gelindiğinde geçerli olur.
background: #fff;: Arka plan rengini beyaz yapar.
color: #000;: Metin rengini siyah yapar.

Arka Plan Videosu Stilleri:
.back-video {}: Arka plan videosu için geçerlidir.
position: absolute;: Konumlandırmayı mutlak yapar.
right: 0;: Sağ kenara yaslar.
bottom: 0;: Alt kenara yaslar.
z-index: -1;: Videoyu diğer içeriklerin arkasına yerleştirir.
@media (min-aspect-ratio: 16/9) {}: Geniş ekranlar (en-boy oranı 16:9'dan büyük) için geçerlidir.
.back-video {}:
width: 100%;: Genişliği %100 yapar.
height: auto;: Yüksekliği otomatik yapar.
@media (max-aspect-ratio: 16/9) {}: Dar ekranlar (en-boy oranı 16:9'dan küçük) için geçerlidir.
.back-video {}:
width: auto;: Genişliği otomatik yapar.
height: 100%;: Yüksekliği %100 yapar.

Bu CSS kodları, sayfanın görsel olarak etkileyici ve kullanıcı dostu olmasını sağlar. Arka plan videosu, hero bölümünün öne çıkmasını sağlarken, metin ve bağlantılar kullanıcı etkileşimleri için tasarlanmıştır.

Hover Card index.html kodlarının açıklaması:
Bu HTML ve CSS kodları, üzerinde hover (fare üzerine geldiğinde) etkisi olan kartlar içeren bir web sayfası oluşturmak için kullanılır. Her kart, ön ve arka yüzlere sahip olup, fare ile üzerine gelindiğinde döner ve arka yüzü gösterir. Bu etkileyici tasarım özellikle bilgi kartları, portföyler veya benzeri içerik sunumları için kullanılabilir.

### HTML Kodu:

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HOVER CARD</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css">
```
- `<!DOCTYPE html>`: HTML5 belgesini tanımlar.
- `<html lang="en">`: Dili İngilizce olarak belirler.
- `<meta charset="UTF-8">`: Belge karakter setini UTF-8 olarak belirler.
- `<meta name="viewport" content="width=device-width, initial-scale=1.0">`: Mobil uyumluluğu sağlar.
- `<title>HOVER CARD</title>`: Sayfa başlığı.
- `<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css">`: Font Awesome kütüphanesini dahil eder.

```html
    <style>
        /* CSS kodları */
    </style>
</head>

<body>
    <div class="wrapper">
        <div class="cols">
            <!-- Kartlar burada olacak -->
        </div>
    </div>
</body>
</html>
```
- `<style>`: CSS kodlarını içeren bölüm.
- `<body>`: Sayfa içeriği burada başlar.
- `<div class="wrapper">`: Tüm kartların içinde bulunacağı ana konteyner.
- `<div class="cols">`: Kartları tutan sütunlar.

### CSS Kodu:

```css
* {
    margin: 0;
    padding: 0;
    -webkit-box-sizing: border-box;
    box-sizing: border-box;
}
```
- Tüm öğelerin kenar boşluklarını ve dolgu alanlarını sıfırlar. Box modelini sınırlar.

```css
body {
    background-color: #000;
}
```
- Sayfa arka planını siyah yapar.

```css
.wrapper {
    width: 90%;
    margin: 0 auto;
    max-width: 80rem;
}
```
- Wrapper genişliğini ve merkezlenmesini ayarlar.

```css
.cols {
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
    -ms-flex-wrap: wrap;
    flex-wrap: wrap;
    -webkit-box-pack: center;
    -ms-flex-pack: center;
    justify-content: center;
}
```
- Kartların yer aldığı sütunların esnek kutu modeli ile düzenlenmesini sağlar.

```css
.col {
    width: calc(25% - 2rem);
    margin: 1rem;
    cursor: pointer;
}
```
- Her kartın genişliğini ve kenar boşluklarını ayarlar.

```css
.container {
    -webkit-transform-style: preserve-3d;
    transform-style: preserve-3d;
    -webkit-perspective: 1000px;
    perspective: 1000px;
}
```
- 3D dönüşümleri mümkün kılar.

```css
.front,
.back {
    background-size: cover;
    box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.25);
    border-radius: 10px;
    background-position: center;
    -webkit-transition: -webkit-transform .7s cubic-bezier(0.4, 0.2, 0.2, 1);
    transition: -webkit-transform .7s cubic-bezier(0.4, 0.2, 0.2, 1);
    -o-transition: transform .7s cubic-bezier(0.4, 0.2, 0.2, 1);
    transition: transform .7s cubic-bezier(0.4, 0.2, 0.2, 1);
    transition: transform .7s cubic-bezier(0.4, 0.2, 0.2, 1), -webkit-transform .7s cubic-bezier(0.4, 0.2, 0.2, 1);
    -webkit-backface-visibility: hidden;
    backface-visibility: hidden;
    text-align: center;
    min-height: 280px;
    height: auto;
    border-radius: 10px;
    color: #fff;
    font-size: 1.5rem;
}
```
- Kartların ön ve arka yüzleri için stilleri tanımlar. 3D dönüşüm ve animasyon geçişlerini ayarlar.

```css
.front:after {
    position: absolute;
    top: 0;
    left: 0;
    z-index: 1;
    width: 100%;
    height: 100%;
    content: '';
    display: block;
    opacity: .6;
    background-color: #000;
    -webkit-backface-visibility: hidden;
    backface-visibility: hidden;
    border-radius: 10px;
}
```
- Ön yüzün üzerine yarı saydam siyah bir katman ekler.

```css
.container:hover .front,
.container:hover .back {
    -webkit-transition: -webkit-transform .7s cubic-bezier(0.4, 0.2, 0.2, 1);
    transition: -webkit-transform .7s cubic-bezier(0.4, 0.2, 0.2, 1);
    -o-transition: transform .7s cubic-bezier(0.4, 0.2, 0.2, 1);
    transition: transform .7s cubic-bezier(0.4, 0.2, 0.2, 1);
    transition: transform .7s cubic-bezier(0.4, 0.2, 0.2, 1), -webkit-transform .7s cubic-bezier(0.4, 0.2, 0.2, 1);
}
```
- Fare ile üzerine gelindiğinde kartın dönüşüm geçişini tanımlar.

```css
.container .back {
    -webkit-transform: rotateY(180deg);
    transform: rotateY(180deg);
    -webkit-transform-style: preserve-3d;
    transform-style: preserve-3d;
}
```
- Arka yüzün başlangıçta 180 derece döndürülmüş olduğunu belirler.

```css
.container .front {
    -webkit-transform: rotateY(0deg);
    transform: rotateY(0deg);
    -webkit-transform-style: preserve-3d;
    transform-style: preserve-3d;
}
```
- Ön yüzün başlangıçta 0 derece olduğunu belirler.

```css
.container:hover .back {
    -webkit-transform: rotateY(0deg);
    transform: rotateY(0deg);
    -webkit-transform-style: preserve-3d;
    transform-style: preserve-3d;
}
```
- Fare ile üzerine gelindiğinde arka yüzün 0 dereceye döndürülmesini sağlar.

```css
.container:hover .front {
    -webkit-transform: rotateY(-180deg);
    transform: rotateY(-180deg);
    -webkit-transform-style: preserve-3d;
    transform-style: preserve-3d;
}
```
- Fare ile üzerine gelindiğinde ön yüzün -180 derece döndürülmesini sağlar.

```css
.front .inner p {
    font-size: 2rem;
    margin-bottom: 2rem;
    position: relative;
}
```
- Kartın içindeki yazının boyutunu ve alt boşluğunu ayarlar.

```css
.front .inner p:after {
    content: '';
    width: 4rem;
    height: 2px;
    position: absolute;
    background: #C6D4DF;
    display: block;
    left: 0;
    right: 0;
    margin: 0 auto;
    bottom: -.75rem;
}
```
- Yazının altına dekoratif bir çizgi ekler.

```css
.front .inner span {
    color: rgba(255, 255, 255, 0.7);
    font-family: 'Montserrat';
    font-weight: 300;
}
```
- Kartın içindeki span öğesi için stil tanımlar.

```css
@media screen and (max-width: 64rem) {
    .col {
        width: calc(33.333333% - 2rem);
    }
}
@media screen and (max-width: 48rem) {
    .col {
        width: calc(50% - 2rem);
    }
}
@media screen and (max-width: 32rem) {
    .col {
        width: 100%;
        margin: 0 0 2rem 0;
    }
}
```
- Farklı ekran boyutları için duyarlı düzen sağlar. Ekran küçüldükçe kartların sayısını azaltır.

```css
/* -- YouTube Link  -- */

#source-link {
    top: 60px;
}
#source-link>i {
    color: rgb









