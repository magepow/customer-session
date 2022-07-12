## Magento 2 CustomerSession Extension Free
In Magento 2, we can't get customer session from \Magento\Customer\Model\Session when varnish cache is enable so we use \Magento\Framework\App\Http\Context instead. But by default, \Magento\Framework\App\Http\Context only gives the value of customer_group and customer_logged_in.
**CustomerSession extension free by Magepow** allows you to get more than just customer_group and customer_logged_in is customer id, name, email and other customer attributes if set.

## How to install Magento 2 CustomerSession extension Free
### ✓ Install Magepow CustomerSession via composer (recommend)
Run the following command in Magento 2 root folder:

```
composer require magepow/customersession
php bin/magento setup:upgrade
php bin/magento setup:static-content:deploy -f
```

## Magepow CustomerSession user guide
### Example:
#### 1. Get customer_logged_in
```
$ObjectManager= \Magento\Framework\App\ObjectManager::getInstance();
$context = $ObjectManager->get('Magento\Framework\App\Http\Context');
$isLoggedIn = $context->getValue(\Magento\Customer\Model\Context::CONTEXT_AUTH);
```
#### 1. Get customer_group
```
$ObjectManager= \Magento\Framework\App\ObjectManager::getInstance();
$context = $ObjectManager->get('Magento\Framework\App\Http\Context');
$isLoggedIn = $context->getValue(\Magento\Customer\Model\Context::CONTEXT_GROUP);
```
#### 1. Get customer id
```
$ObjectManager= \Magento\Framework\App\ObjectManager::getInstance();
$context = $ObjectManager->get('Magento\Framework\App\Http\Context');
$isLoggedIn = $context->getValue('customer_id');
```
#### 1. Get customer name
```
$ObjectManager= \Magento\Framework\App\ObjectManager::getInstance();
$context = $ObjectManager->get('Magento\Framework\App\Http\Context');
$isLoggedIn = $context->getValue('customer_name');
```
#### 1. Get customer email
```
$ObjectManager= \Magento\Framework\App\ObjectManager::getInstance();
$context = $ObjectManager->get('Magento\Framework\App\Http\Context');
$isLoggedIn = $context->getValue('customer_email');
```

To get more customer attributes you have to edit method **aroundDispatch** in \Magepow\CustomerSession\Plugin\CustomerSessionContext.php

## Donation

If this project help you reduce time to develop, you can give me a cup of coffee :) 

[![paypal](https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif)](https://www.paypal.com/paypalme/alopay)


**Free Extensions List**

* [Magento 2 Recent Sales Notification](https://magepow.com/magento-2-recent-sales-notification.html)

* [Magento 2 Categories Extension](https://magepow.com/magento-categories-extension.html)

* [Magento 2 Sticky Cart](https://magepow.com/magento-sticky-cart.html)

**Premium Extensions List**

* [Magento 2 Pages Speed Optimizer](https://magepow.com/magento-speed-optimizer.html)

* [Magento 2 Mutil Translate](https://magepow.com/magento-multi-translate.html)

* [Magento 2 Instagram Integration](https://magepow.com/magento-2-instagram.html)

* [Magento 2 Lookbook Pin Products](https://magepow.com/lookbook-pin-products.html)

**Featured Magento Themes**

* [Expert Multipurpose responsive Magento 2 Theme](https://1.envato.market/c/1314680/275988/4415?u=https://themeforest.net/item/expert-premium-responsive-magento-2-and-1-support-rtl-magento-2-/21667789)

* [Gecko Premium responsive Magento 2 Theme](https://1.envato.market/c/1314680/275988/4415?u=https://themeforest.net/item/gecko-responsive-magento-2-theme-rtl-supported/24677410)

* [Milano Fashion responsive Magento 2 Theme](https://1.envato.market/c/1314680/275988/4415?u=https://themeforest.net/item/milano-fashion-responsive-magento-1-2-theme/12141971)

* [Electro responsive Magento 2 Theme](https://1.envato.market/c/1314680/275988/4415?u=https://themeforest.net/item/electro-responsive-magento-1-2-theme/17042067)

* [Pizzaro Food responsive Magento 2 Theme](https://1.envato.market/c/1314680/275988/4415?u=https://themeforest.net/item/pizzaro-food-responsive-magento-1-2-theme/19438157)

* [Biolife Organic responsive Magento 2 Theme](https://1.envato.market/c/1314680/275988/4415?u=https://themeforest.net/item/biolife-organic-food-magento-2-theme-rtl-supported/25712510)

* [Market responsive Magento 2 Theme](https://1.envato.market/c/1314680/275988/4415?u=https://themeforest.net/item/market-responsive-magento-2-theme/22997928)

* [Kuteshop responsive Magento 2 Theme](https://1.envato.market/c/1314680/275988/4415?u=https://themeforest.net/item/kuteshop-multipurpose-responsive-magento-1-2-theme/12985435)

**Featured Magento Services**

* [PSD to Magento 2 Theme Conversion](https://magepow.com/psd-to-magento-theme-conversion.html)

* [Magento Speed Optimization Service](https://magepow.com/magento-speed-optimization-service.html)

* [Magento Security Patch Installation](https://magepow.com/magento-security-patch-installation.html)

* [Magento Website Maintenance Service](https://magepow.com/website-maintenance-service.html)

* [Magento Professional Installation Service](https://magepow.com/professional-installation-service.html)

* [Magento Upgrade Service](https://magepow.com/magento-upgrade-service.html)

* [Customization Service](https://magepow.com/customization-service.html)

* [Hire Magento Developer](https://magepow.com/hire-magento-developer.html)

**[Our Shopify Themes](https://themeforest.net/user/alotheme)**

* [Dukamarket - Multipurpose Shopify Theme](https://1.envato.market/c/1314680/275988/4415?u=https://themeforest.net/item/dukamarket-multipurpose-shopify-theme/36158349)

* [Ohey - Multipurpose Shopify Theme](https://1.envato.market/c/1314680/275988/4415?u=https://themeforest.net/item/ohey-multipurpose-shopify-theme/34624195)

* [Flexon - Multipurpose Shopify Theme](https://1.envato.market/c/1314680/275988/4415?u=https://themeforest.net/item/flexon-multipurpose-shopify-theme/33461048)

**[Our Shopify App](https://apps.shopify.com/partners/maggicart)**

* [Magepow Size Chart](https://apps.shopify.com/magepow-size-chart)

**[Our WordPress Theme](https://themeforest.net/user/alotheme/portfolio)**

* [SadesMarket - Multipurpose WordPress Theme](https://1.envato.market/c/1314680/275988/4415?u=https://themeforest.net/item/sadesmarket-multipurpose-wordpress-theme/35369933)
