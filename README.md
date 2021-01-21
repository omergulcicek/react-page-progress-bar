# react-page-progress-bar

Sayfadaki konumu dairesel bir progress bar'da gösterir.

`React` component şeklinde geliştirilmiştir, farklı kütüphanelerde çalışmaz.


![react-page-progress-bar](http://omergulcicek.com/img/react-page-progress-bar.png)

## Yükle
```
$ npm install react-page-progress-bar
```
```
$ yarn add react-page-progress-bar
```

## Kullanımı
```js
import PageProgressBar from "react-page-progress-bar";

<PageProgressBar />

<PageProgressBar options={{ "color": "#26a69a", "size": "80px" }} />
```

## Özelleştir

**Sadece** değiştirmek istediğiniz değerleri göndermeniz yeterlidir. Hiçbir parametre göndermezseniz veya bazılarını yazmazsanız varsayılan olarak çalışacak ayarlar aşağıdaki gibidir;

```js
const defaultOptions = {
  "color": "#1b1b1b",
  "size": "48px",
  "strokeWidth": "5",
  "arrowColor": "#1b1b1b",
  "hidden": true,
  "top": "auto",
  "bottom": "100px",
  "left": "auto",
  "right": "40px"
}
```

### Parametre açıklamaları ve varsayılan değerleri

#### `color`: string
Çemberde ki progress barın rengi
- default: `#1b1b1b`

#### `size`: string
Çemberin genişliği (Yükseklik ve genişlik aynı değerleri alır)
- default: `48px`

#### `strokeWidth`: string
Çemberde ki progress barın kalınlığı
- default: `5`

#### `arrowColor`: string
Çember içerisindeki okun rengi
- default: `#1b1b1b`

#### `hidden`: boolean
Sayfa yukarı scroll ettiğinde çemberin gizlenip/gösterilmesi
Varsayılan olarak gizlenir, `false` yaparsanız, sayfa yukarı scroll etse bile çember gizlenmez.
- default: `true`

#### `top`: string
Çemberin yukarıdan konumu
Varsayılan olarak çember aşağıdadır. `top` değeri atamak isterseniz, `bottom` değerini `auto` olarak tanımlayın 
- default: `auto`

#### `left`: string
Çemberin soldan konumu
Varsayılan olarak çember sağdadır. `left` değeri atamak isterseniz, `right` değerini `auto` olarak tanımlayın 
- default: `auto`

#### `bottom`: string
Çemberin aşağıdan konumu
- default: `100px`

#### `right`: string
Çemberin sağdan konumu
- default: `40px`