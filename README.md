
The CoinSimple WP e-Commerce plugin is an extension of the WP e-Commerce plugin for Wordpress, and allows e-commerce stores, running on Wordpress and  WP e-Commerce, to accept bitcoin through CoinSimple.

<!--more-->

## Requirements

1. **Installed WP e-Commerce plugin on your Wordpress site**. (Installation instructions can be found at [www.getshopped.org](http://www.getshopped.org)).
2. **A Business ID and API key from CoinSimple.com**. To find your information, go to your [CoinSimple.com](http://coinsimple.com) dashboard, select your business, and go to "Settings". You will find your *Business ID* and *API key* under "Busines Information" and "API Credentials".

## Installation

*Do not attempt to install this plugin through the WordPress Plugins dashboard. Use the following instructions, instead.*

1. [Download a zip file of the plugin](https://github.com/coinsimple/coinsimple-wpecommerce/archive/v1.zip).
2. Log in to your WordPress site using ssh and copy the file  your ``wp-content/plugins/wp-e-commerce`` directory that contains the WP eCoomerce files. Unzip the file there.

At this point the plugin is installed and activated but it still needs to be enabled and configured.

## Configuration

1. Log into the WordPress dashboard and click "Settings" and then "Store".

  ![Select Settings then "Store"](/media/wpecommerce/wpecommerce-plugin-action-settings-store.png)

2. In the screen that appears click on "Payments".

  ![Payments with WP eCommerce](/media/wpecommerce/wpecommerce-plugin-screen-payments-coinsimple.png)

3. Select the checkbox to the left of "Bitcoin Payments by CoinSimple" and click Settings below the CoinSimple payment option. Change the "Display Name" if desired.  

  ![Bitcoin Payments by CoinSimple](/media/wpecommerce/wpecommerce-plugin-screen-payments-coinsimple-display_name.png)

5. Enter your CoinSimple.com business ID and API in the appropriate fields. Enter the URL of the page that your customers will be directed to after they make their payment. For WP e-Commerce, the default page is
`http://yourwebsite.com/products-page/transaction-results/`

  ![Business ID, API key and callback URL](/media/wpecommerce/wpecommerce-plugin-screen-payments-coinsimple-settings.png)

5. Click "Update".

## Use

- When a buyer selects "Bitcoin" as their payment method, an invoice is generated at CoinSimple.
- After the buyer pays, CoinSimple directs the buyer to the page that you selected in your Settings above.

## Support

### CoinSimple Support

* If you are having a problem with this plugin, please use [this Github issues page](https://github.com/coinsimple/coinsimple-wpecommerce/issues) to report your problem.

### WP e-Commerce Support

* [Homepage](http://getshopped.org/)
* [Documentation](http://docs.getshopped.org/)
* [Support Forums](https://wordpress.org/support/plugin/wp-e-commerce)

### Troubleshooting

* This plugin requires PHP 5.4 or higher to function correctly. Contact your webhosting provider or server administrator if you are unsure which version is installed on your web server.
* Ensure a valid SSL certificate is installed on your server. Also ensure your root CA cert is updated. If your CA cert is not current, you will see curl SSL verification errors.
* Verify that your web server is not blocking POSTs from servers it may not recognize. Double check this on your firewall as well, if one is being used.
* Check the system error log file (usually the web server error log) for any errors during CoinSimple payment attempts. If you contact CoinSimple support, they will ask to see the log file to help diagnose the problem.
* If all else fails, send an email describing your issue in detail to [support@coinsimple.com](mailto:support@coinsimple.com). In your support request, please provide:
	* Wordpress version
	* WP eCommerce version
	* PHP version
	* Other plugins installed
	* Configuration settings for the CoinSimple plugin
	* Screenshot of error messages, if any


## Contribute

To contribute to this project, please fork and submit a pull request.


## About CoinSimple

CoinSimple allows consultants and online merchants to **easily** accept bitcoins either through a bitcoin payment processor ([BitPay](http://bitpay.com), [Coinbase](http://coinbase.com), [GoCoin](http://gocoin.com)) or directly to their deterministic wallet ([Electrum](http://electrum.org), [Armory](http://bitcoinarmory.com), [Trezor](http://www.bitcointrezor.com/)) or to any non-deterministic bitcoin wallet. One can use the [CoinSimple web app](https://coinsimple.com) to issue invoices directly, Wordpress eCommerce (see [demo site](http://wordpress.coinsimple.com) or [plugin page](https://github.com/coinsimple/coinsimple-wpecommerce)), WooCommerce (see [demo site](http://woocommerce.coinsimple.com) or [plugin page](https://github.com/coinsimple/coinsimple-woocommerce)), Magento (see [demo site](http://magento.coinsimple.com) or [plugin page](https://github.com/coinsimple/coinsimple-magento)), to sell products through the respective online stores, or a "Pay in Bitcoin" button on any webpage to accept donations, payments or even sell products.

For more information about CoinSimple, please visit [CoinSimple.com](https://coinsimple.com).


## License

The MIT License (MIT)

Copyright (c) 2014-2015 CoinSimple

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
