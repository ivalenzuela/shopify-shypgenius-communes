# Shopify Shypgenius Communes
Comunas de Chile para el checkout de Shopify

## Requisitos
* código de Google Analytics Activado

## Guia de Activación de la librería
1.- Ingresa al apartado **Sales Channels** -> **Online Store** -> **Preferences**

1. Ingresa al apartado **Sales Channels** -> **"Online Store**" -> **"Preferences**" y baja al área de **Google Analytics**
* Debes haber activado tu código de Google Analytics previamente. Si no lo haz echo, sigue esta guía:
> https://help.shopify.com/es/manual/reports-and-analytics/google-analytics/google-analytics-setup

2. Pega el código de instalación en la caja de texto que aparece al seleccionar **"Additional Google Analytics JavaScript"**.

```
if (window.location.href.indexOf('checkout') > -1) {
  var maps = document.createElement('script');
  maps.src = 'https://maps.googleapis.com/maps/api/js?key=AIzaSyBwUsibACjM7a5qiae2alRqxlWRpA9gpC4&libraries=places';
  document.head.appendChild(maps);
  var script = document.createElement('script');
  script.src = 'https://static.shypgenius.com/common/checkout.js';
  document.head.appendChild(script);
}
```

Eso es todo!

**Happy Shopifying!**
