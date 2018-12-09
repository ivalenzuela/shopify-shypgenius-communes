# Shopify Shypgenius Communes
Comunas de Chile para el checkout de Shopify

| Version | Build | Code Quality | Tests | Uptime |
|:---|:---|:---|:---|:---|
|[![CircleCI](https://img.shields.io/badge/checkout-0.9-blue.svg)](https://springsdigital.com/code-compliance)|[![CircleCI](https://img.shields.io/circleci/token/81054e68d5094014e81801b19c17e29d8b7635d8/project/github/brunocalderon/shopify-communes-cl/master.svg)](https://springsdigital.com/code-compliance)|[![Codacy Badge](https://img.shields.io/codacy/grade/ff8963e332314fd8b233daff50187af7.svg)](https://springsdigital.com/code-compliance)|[![GhostInspector](https://api.ghostinspector.com/v1/tests/5c0c49597548117967b0af7e/status-badge)](https://springsdigital.com/code-compliance)|[![Uptime](https://img.shields.io/uptimerobot/ratio/7/m778918918-3e92c097147760ee39d02d36.svg)](http://status.shypgenius.com)

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
