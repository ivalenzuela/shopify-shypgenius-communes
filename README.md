# Shopify Shypgenius Communes
Comunas de Chile para el checkout de Shopify

#### Circle CI Status
[![CircleCI](https://circleci.com/gh/brunocalderon/shopify-communes-cl/tree/master.svg?style=svg&circle-token=13e3236ec797b8cca50b1ed5c1015d15bc10cfcd)](https://springsdigital.com/code-compliance)

#### Ghost Inspector Status:
[![GhostInspector](https://api.ghostinspector.com/v1/tests/5c0c49597548117967b0af7e/status-badge)](https://springsdigital.com/code-compliance)


## Requisitos
* Código de Google Analytics Activado

## Guia de Activación de la librería
1.- Ingresa al apartado **Sales Channels** -> **Online Store** -> **Preferences**

1. Ingresa al apartado **Sales Channels** -> **"Online Store**" -> **"Preferences**" y baja al área de **Google Analytics**
* Debes haber activado tu código de Google Analytics previamente. Si no lo haz echo, sigue esta guía:
> https://help.shopify.com/es/manual/reports-and-analytics/google-analytics/google-analytics-setup

2. Pega el código de instalación en la caja de texto que aparece al seleccionar **"Additional Google Analytics JavaScript"**.

```
if(window.location.href.indexOf('checkout')>-1){let _scripts=['https://code.jquery.com/jquery-3.3.1.min.js','https://maps.googleapis.com/maps/api/js?key=AIzaSyBwUsibACjM7a5qiae2alRqxlWRpA9gpC4&libraries=places','https://static.shypgenius.com/master/checkout.js'];function createScriptTag(){let script=_scripts.shift();if(!script)return;let js=document.createElement('script');js.type='text/javascript';js.src=script;js.onload=(event)=>{createScriptTag();};let s=document.getElementsByTagName('script')[0];s.parentNode.insertBefore(js,s);}createScriptTag()}
```

Eso es todo!

**Happy Shopifying!**
