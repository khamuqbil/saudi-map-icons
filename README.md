# Saudi Arabia Province Map Icons

<div align="center">

![Saudi Map Icon](saudi-map-icon.svg)

**Open-source SVG icons for Saudi Arabia map and its 13 administrative provinces**

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

[English](#english) | [العربية](#العربية)

</div>

---

## English

### About

This project provides free, open-source SVG icons for Saudi Arabia, designed to fill the gap in icon libraries like Font Awesome that lack Saudi-specific regional icons. Perfect for:

- Web applications serving Saudi users
- Flight tracking systems (domestic vs international)
- Government and regional services
- Educational materials
- Any project needing Saudi geographic representation

### Files Included

| File | Description | Use Case |
|------|-------------|----------|
| `saudi-map-icon.svg` | Simplified Saudi Arabia silhouette | Icon libraries, buttons, badges |
| `saudi-map-provinces.svg` | Detailed map with all 13 provinces | Interactive maps, dashboards |
| `saudi-map-provinces-ar.svg` | Provinces with Arabic labels | Arabic interfaces |

### Installation

#### Direct Download
```bash
# Clone the repository
git clone https://github.com/khamuqbil/saudi-map-icons.git
```

#### CDN (coming soon)
```html
<img src="https://cdn.jsdelivr.net/gh/khamuqbil/saudi-map-icons/saudi-map-icon.svg" alt="Saudi Arabia">
```

### Usage

#### As an HTML Image
```html
<img src="saudi-map-icon.svg" alt="Saudi Arabia" width="32" height="32">
```

#### Inline SVG (recommended for styling)
```html
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 640 512" width="32" height="32">
  <path fill="currentColor" d="M322.1 252l0-1-51.2-65.8s-12..."/>
</svg>
```

#### CSS Background
```css
.saudi-icon {
  background-image: url('saudi-map-icon.svg');
  background-size: contain;
  width: 32px;
  height: 32px;
}
```

#### With Font Awesome (as custom icon)
```html
<!-- Use alongside Font Awesome -->
<i class="fas fa-globe-americas"></i> <!-- International -->
<img src="saudi-map-icon.svg" class="fa-icon-custom"> <!-- Domestic Saudi -->
```

#### Interactive Province Map (JavaScript)
```html
<object data="saudi-map-provinces.svg" type="image/svg+xml" id="saudi-map"></object>

<script>
document.getElementById('saudi-map').addEventListener('load', function() {
  const svg = this.contentDocument;
  const provinces = svg.querySelectorAll('.saudi-map-icons');

  provinces.forEach(province => {
    province.addEventListener('click', function() {
      const code = this.id;        // e.g., "SA-12"
      const name = this.getAttribute('title'); // e.g., "Al-jouf"
      console.log(`Clicked: ${name} (${code})`);
    });
  });
});
</script>
```

### Province Codes (ISO 3166-2:SA)

| Code | English | العربية |
|------|---------|---------|
| SA-01 | Riyadh | الرياض |
| SA-02 | Mecca | مكة المكرمة |
| SA-03 | Medina | المدينة المنورة |
| SA-04 | Eastern Province | المنطقة الشرقية |
| SA-05 | Al-Qassim | القصيم |
| SA-06 | Hail | حائل |
| SA-07 | Tabuk | تبوك |
| SA-08 | Northern Borders | الحدود الشمالية |
| SA-09 | Jazan | جازان |
| SA-10 | Najran | نجران |
| SA-11 | Al-Bahah | الباحة |
| SA-12 | Al-Jouf | الجوف |
| SA-13 | Asir | عسير |

### Styling Examples

#### Color Variants
```css
/* Green (Saudi flag color) */
.saudi-icon-green { color: #006C35; }

/* Gold accent */
.saudi-icon-gold { color: #C8A951; }

/* Dark mode */
.saudi-icon-dark { color: #ffffff; }

/* Light mode */
.saudi-icon-light { color: #1a1a1a; }
```

#### Highlight a Specific Province
```css
#SA-12 { /* Al-Jouf */
  fill: #006C35;
  stroke: #ffffff;
  stroke-width: 2;
}
```

### Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes, please open an issue first.

### License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

### Credits

Created by [Khalid Alkhaldi](https://github.com/khamuqbil) as part of the [Jouf App](https://www.jouf.app) project - Al-Jouf Airport Flight Radar.

---

## العربية

### نبذة

يوفر هذا المشروع أيقونات SVG مجانية ومفتوحة المصدر لخريطة المملكة العربية السعودية، مصممة لسد الفجوة في مكتبات الأيقونات مثل Font Awesome التي تفتقر إلى أيقونات سعودية إقليمية.

### الاستخدام

#### كصورة HTML
```html
<img src="saudi-map-icon.svg" alt="المملكة العربية السعودية" width="32" height="32">
```

#### كـ SVG مضمن (موصى به للتنسيق)
```html
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 640 512" width="32" height="32" dir="rtl">
  <path fill="currentColor" d="M322.1 252l0-1-51.2-65.8s-12..."/>
</svg>
```

### رموز المناطق

| الرمز | المنطقة |
|-------|---------|
| SA-01 | الرياض |
| SA-02 | مكة المكرمة |
| SA-03 | المدينة المنورة |
| SA-04 | المنطقة الشرقية |
| SA-05 | القصيم |
| SA-06 | حائل |
| SA-07 | تبوك |
| SA-08 | الحدود الشمالية |
| SA-09 | جازان |
| SA-10 | نجران |
| SA-11 | الباحة |
| SA-12 | الجوف |
| SA-13 | عسير |

### الترخيص

هذا المشروع مرخص بموجب رخصة MIT - راجع ملف [LICENSE](LICENSE) للتفاصيل.

### الشكر

تم إنشاؤه بواسطة [خالد الخالدي](https://github.com/khamuqbil) كجزء من مشروع [تطبيق الجوف](https://www.jouf.app) - رادار رحلات مطار الجوف.

---

<div align="center">

**Made with :heart: in Al-Jouf, Saudi Arabia**

</div>
