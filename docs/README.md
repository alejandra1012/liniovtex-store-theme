# Store Linio

Linio store theme es una copia del ecommerce LINIO la cual implemente para capacitarme y entender mas sobre como funciona VTEX IO.
A continuacion voy a explicar paso a paso el proceso para crear un ecommerce con  la plataforma VTEX IO.

Pagina oficial [Linio](https://www.linio.com.co/?gclsrc=aw.ds&&adjust_t=1zira0_f1h7ws&adjust_google_network=g&adjust_google_placement=&adjust_campaign=LICO-LAB-AO-INSTI-LOC-00007-Brand_linio_absoluto-Ago21-GG-Search-Conversion-Brand&adjust_adgroup=51198174648&utm_term=&gclid=CjwKCAiAheacBhB8EiwAItVO2ystcnbn1Ml4d1-thpg7HyhW73g2ccdSbCknAyj64RiL-hXtns_W_RoCtpAQAvD_BwE#).

#### Home

![Linio](assets/img/readme__buttom-whatsApp.png)

## Configuracion

### Paso 1

Acceda a la guia basica de configuracion de [VTEX IO](https://vtex.io/docs/getting-started/build-stores-with-store-framework/1). Ademas de esto debera tener instalado el [CLI](https://developers.vtex.com/vtex-developer-docs/docs/vtex-io-documentation-vtex-io-cli-installation-and-command-reference) (Command Line Interface) de VTEX IO

### Paso 2 - Clonar el repositorio

[Clone](https://github.com/alejandra1012/liniovtex-store-theme/tree/master) este repositorio en tu maquina local para poder trabajar y accede a el por tu terminal.

### Paso 3 - Edite el `manifest.json`

Una vez clonado el repositorio hay que hacer unas cuantas modificaciones en el manifest.json del proyecto.

Tendrá que modificar valores de la propiedad `vendor` por el nombre de la cuenta en la que este trabajando. la propiedad `name` no es obligatoria modificarla para su uso pero puede cambiarla por el nombre que desee

```json
{
  "vendor": "storecomponents",
  "name": "my-test-theme"
}
```

### Paso 4 - Desinstalar el store-theme predeterminado

Al ejecutar `vtex list`, puede verificar si algún tema está instalado.

Es común tener ya instalado un `vtex.store-theme` cuando inicia el proceso de desarrollo frontal de la tienda.

Por lo tanto, si lo encuentra en la lista de aplicaciones, copie su nombre y version, luego utilícelo junto con el comando `vtex uninstall`. Por ejemplo:

```json
vtex uninstall vtex.store-theme@0.0.1
```

### Paso 6 - Ejecute un preview de la tienda

Entonces ha llegado el momento de cargar todos los cambios que realizó en sus archivos locales a la plataforma. Para eso, use el comando `vtex link`.

Si el proceso se ejecuta sin ningún error, se mostrará el siguiente mensaje: `Aplicación vinculada con éxito`. Luego, ejecute el comando `vtex browser` para abrir una ventana del navegador que tenga su tienda vinculada.

Esto le permitirá ver los cambios aplicados en tiempo real, a través de la cuenta y el espacio de trabajo en el que está trabajando.

## Store Components

```json
{
  "vtex.store": "2.x",
    "vtex.store-header": "2.x",
    "vtex.product-summary": "2.x",
    "vtex.store-footer": "2.x",
    "vtex.store-components": "3.x",
    "vtex.styleguide": "9.x",
    "vtex.slider": "0.x",
    "vtex.carousel": "2.x",
    "vtex.shelf": "1.x",
    "vtex.menu": "2.x",
    "vtex.minicart": "2.x",
    "vtex.product-details": "1.x",
    "vtex.product-kit": "1.x",
    "vtex.search-result": "3.x",
    "vtex.login": "2.x",
    "vtex.my-account": "1.x",
    "vtex.flex-layout": "0.x",
    "vtex.rich-text": "0.x",
    "vtex.store-drawer": "0.x",
    "vtex.locale-switcher": "0.x",
    "vtex.product-quantity": "1.x",
    "vtex.product-identifier": "0.x",
    "vtex.product-specification-badges": "0.x",
    "vtex.product-review-interfaces": "1.x",
    "vtex.telemarketing": "2.x",
    "vtex.order-placed": "2.x",
    "vtex.stack-layout": "0.x",
    "vtex.tab-layout": "0.x",
    "vtex.responsive-layout": "0.x",
    "vtex.slider-layout": "0.x",
    "vtex.iframe": "0.x",
    "vtex.breadcrumb": "1.x",
    "vtex.sticky-layout": "0.x",
    "vtex.add-to-cart-button": "0.x",
    "vtex.store-image": "0.x",
    "vtex.store-video": "1.x",
    "vtex.store-newsletter": "1.x",
    "vtex.store-link": "0.x",
    "vtex.search": "1.x",
    "vtex.store-icons": "0.x",
    "vtex.product-list": "0.x",
    "vtex.checkout-summary": "0.x",
    "vtex.disclosure-layout": "1.x",
    "vtex.product-price": "1.x",
    "vtex.modal-layout": "0.x",
    "vtex.product-specifications": "1.x",
    "vtex.overlay-layout": "0.x",
    "itgloberspartnercl.whatsapp-button": "0.x"
}
```
### Custom component

```json
{
  "{vendor}.whatsapp-button": "0.x"
}
```

#### Aplicaciones

| Nombre                                                                                                | Version |
| ----------------------------------------------------------------------------------------------------- | ------- |
| [{vendor}.whatsapp-button](https://github.com/alejandra1012/itgloberspartnercl-whatsapp-button)       | 0.x     |
