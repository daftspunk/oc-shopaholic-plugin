# Shopaholic

[![Build Status](https://travis-ci.org/lovata/oc-shopaholic-plugin.svg?branch=master)](https://travis-ci.org/lovata/oc-shopaholic-plugin)
[![Coverage Status](https://coveralls.io/repos/github/lovata/oc-shopaholic-plugin/badge.svg?branch=master)](https://coveralls.io/github/lovata/oc-shopaholic-plugin?branch=master)
[![Code Climate](https://codeclimate.com/github/lovata/oc-shopaholic-plugin/badges/gpa.svg)](https://codeclimate.com/github/lovata/oc-shopaholic-plugin)
[![Crowdin](https://d322cqt584bo4o.cloudfront.net/shopaholic-plugin-for-october/localized.svg)](https://crowdin.com/project/shopaholic-plugin-for-october)
[![SemVer](http://img.shields.io/SemVer/2.0.0.png)](http://semver.org/spec/v2.0.0.html)
[![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)

E-Commerce plugin by [LOVATA](https://lovata.com) for October CMS.

![Shopaholic Banner](assets/images/shopaholic-banner.png)

## Overview

Shopaholic is a scalable and highly flexible e-commerce ecosystem for [October CMS](https://octobercms.com). The core plugin is provided free of charge and includes the following set of features:

* Products and trade offers management.
* Product image gallery management.
* Products grouping by categories and brands.
* Multi-currency, taxes and price types management.
* Data import (product, offers, categories, brands) from a CSV file.
* Basic products filtering (by category, brand etc.) and sorting (by price, new additions etc.)

In order to cater to the growing scalability demands of a project, the ecosystem provides [extra plugins](https://octobercms.com/plugin/lovata-shopaholic#extensions) to extend the basic functionality. With these plugins sellers can:

* Manage multi-language content (via [RainLab.Translate](https://octobercms.com/plugin/rainlab-translate)).
* Sell online (via [Lovata.PayPalShopaholic](https://octobercms.com/plugin/lovata-paypalshopaholic)).
* Extend online payment options by adding additional payment providers (via [Lovata.OmnipayShopaholic](https://octobercms.com/plugin/lovata-omnipayshopaholic)).
* Create custom products filters by any essence (e.g. by _New additions_, _Discounts_, _In stock_ etc.) (via [Lovata.FilterShopaholic](https://octobercms.com/plugin/lovata-filtershopaholic)).
* Add custom properties to a product (via [Lovata.PropertiesShopaholic](https://octobercms.com/plugin/lovata-propertiesshopaholic)).
* Bind similar products to a certain one (via [Lovata.RelatedProductsShopaholic](https://octobercms.com/plugin/lovata-relatedproductsshopaholic)).
* Manage promo activities (via [Lovata.CouponsShopaholic](https://octobercms.com/plugin/lovata-couponsshopaholic), [Lovata.DiscountsShopaholic](https://octobercms.com/plugin/lovata-discountsshopaholic) and [Lovata.CampaignsShopaholic](https://octobercms.com/plugin/lovata-campaignsshopaholic)).
* Group products for SEO reasons (via [Lovata.TagsShopaholic](https://octobercms.com/plugin/lovata-tagsshopaholic)).
* Manage complex SEO issues (via [Lovata.MightySeo](https://octobercms.com/plugin/lovata-mightyseo)).
* Increase the revenue by assigning accessories to the products (via [Lovata.AccessoriesShopaholic](https://octobercms.com/plugin/lovata-accessoriesshopaholic)).
* Manage customers (via [Lovata.Buddies](https://octobercms.com/plugin/lovata-buddies) or [RainLab.User](https://octobercms.com/plugin/rainlab-user)).

Besides you can provide a better UX for the customer with the ability to:
* Sind the popular products ( via [Lovata.PopularityShopaholic](https://octobercms.com/plugin/lovata-popularityshopaholic)).
* Search for the products (via [Lovata.SearchShopaholic](https://octobercms.com/plugin/lovata-searchshopaholic) or [Lovata.SphinxShopaholic](https://octobercms.com/plugin/lovata-sphinxshopaholic)).
* Compare the products (via [Lovata.CompareShopaholic](https://octobercms.com/plugin/lovata-compareshopaholic)).
* Find the products they viewed before (via [Lovata.ViewedProductsShopaholic](https://octobercms.com/plugin/lovata-viewedproductsshopaholic)).
* Leave and read the reviews for the products (via [Lovata.ReviewsShopaholic](https://octobercms.com/plugin/lovata-reviewsshopaholic)).
* Postpone the products for the future purchases (via [Lovata.WishListShopaholic](https://octobercms.com/plugin/lovata-wishlistshopaholic)).

The development of Shopaholic’s ecosystem is guided by the similar philosophies of October CMS and Unix like operating systems, where the main focus is to create simple microarchitecture solutions that communicate with each other through smart APIs.

One one hand, this approach allows keeping performance, security, and functionality of the code to a high standard. On the other hand, it provides a clean and smooth back-end UI/UX that isn't over-bloated with the features.
## Installation

Using the Laravel’s CLI is the fastest way to get started. Just run the following commands in a project’s root directory:

```bash
php artisan plugin:install lovata.shopaholic
php artisan plugin:install lovata.toolbox
```

As for _[Toolbox plugin](https://octobercms.com/plugin/lovata-toolbox)_ it's a set of helpers required for a Shopaholic.

Once the plugin is installed take a look at the official documentation for the possible next steps.

## Documentation

The complete documentation of official ecosystem plugin can be found [here](https://github.com/lovata/oc-shopaholic-plugin/wiki).


## Performance

As an environment for a testing measurements was used simple Digital Ocean droplet with this configuration:
* Dual Core CPU
* 4 Gb RAM
* Ubuntu 18.04
* PHP 7.2.0
* Apache 2.4
* MySQL 5.7

| Products number     | Catalog page load time | Product list filtering time |
| ------------------: | ---------------------: | --------------------------: |
|                 210 |             100-150 ms |                   80-100 ms |
|              21 000 |            900-1100 ms |                  500-600 ms |

If you would like to know how our plugins perform with large catalogs of products, you can visit our [Large Catalog Live Demo](http://big-demo.shopaholic.one) that has 21 000 products, 68 000 offers and 210 000 variations of property values.

## Get involved

If you're interested in the improvement of this project you can help in the following ways:
* bug reporting and new feature requesting by creating issues on plugin [GitHub page](https://github.com/lovata/oc-shopaholic-plugin/issues);
* contribution to a project following these [instructions](https://github.com/lovata/oc-shopaholic-plugin/blob/master/CONTRIBUTING.md);
* localization to your language using [Crowdin](https://crowdin.com/project/shopaholic-plugin-for-october) service.

## License

© 2019, [LOVATA Group, LLC](https://github.com/lovata) under [GNU GPL v3](https://opensource.org/licenses/GPL-3.0).

Developed by [Andrey Kharanenka](https://github.com/kharanenka).
