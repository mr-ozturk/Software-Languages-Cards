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









