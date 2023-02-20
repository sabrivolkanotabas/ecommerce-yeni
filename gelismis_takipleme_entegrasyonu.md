## Konu Başlıkları
	1.0 | Gelişmiş E-Ticaret Takibi Entegrasyonu
	2.0 | User-ID Entegrasyonu
	3.0 | Gelişmiş Form Takibi Entegrasyonu
	4.0 | Enhanced Conversion Entegrasyonu

## 1.0 | Gelişmiş E-Ticaret Takibi Entegrasyonu

## 1.0.1 - view_item_list

<p>Kullanıcıya belirli bir kategorideki öğelerin listesi sunulduğunda çalışmalıdır.</p>

```
dataLayer.push({ ecommerce: null }); // Clear the previous ecommerce object.  
dataLayer.push({  
  event: "view_item_list",  
  ecommerce: {  
	  items: [{  
		  item_id: "SKU_12345",  
		  item_name: "Stan and Friends Tee",  
		  affiliation: "Google Merchandise Store",  
		  coupon: "SUMMER_FUN",  
		  currency: "USD",  
		  discount: 2.22,  
		  index: 0,  
		  item_brand: "Google",  
		  item_category: "Apparel",  
		  item_category2: "Adult",  
		  item_category3: "Shirts",  
		  item_category4: "Crew",  
		  item_category5: "Short sleeve",  
		  item_list_id: "related_products",  
		  item_list_name: "Related Products",  
		  item_variant: "green",  
		  location_id: "ChIJIQBpAG2ahYAR_6128GcTUEo",  
		  price: 9.99,  
		  quantity: 1  
	  },  
	  {  
		  item_id: "SKU_12346",  
		  item_name: "Google Grey Women's Tee",  
		  affiliation: "Google Merchandise Store",  
		  coupon: "SUMMER_FUN",  
		  currency: "USD",  
		  discount: 3.33,  
		  index: 1,  
		  item_brand: "Google",  
		  item_category: "Apparel",  
		  item_category2: "Adult",  
		  item_category3: "Shirts",  
		  item_category4: "Crew",  
		  item_category5: "Short sleeve",  
		  item_list_id: "related_products",  
		  item_list_name: "Related Products",  
		  item_variant: "gray",  
		  location_id: "ChIJIQBpAG2ahYAR_6128GcTUEo",  
		  price: 20.99,  
		  promotion_id: "P_12345",  
		  promotion_name: "Summer Sale",  
		  quantity: 1  
	  }]  
 }});
```
<br>

## 1.0.2 - select_item

<p>Kullanıcı, site içerisinde bir ürün tıklaması gerçekleştirdiğinde çalışmalıdır.</p>

```
dataLayer.push({ ecommerce: null }); // Clear the previous ecommerce object.  
dataLayer.push({  
  event: "select_item",  
  ecommerce: {  
  items: [{  
	  item_id: "SKU_12345",  
	  item_name: "Stan and Friends Tee",  
	  affiliation: "Google Merchandise Store",  
	  coupon: "SUMMER_FUN",  
	  currency: "USD",  
	  discount: 2.22,  
	  index: 0,  
	  item_brand: "Google",  
	  item_category: "Apparel",  
	  item_category2: "Adult",  
	  item_category3: "Shirts",  
	  item_category4: "Crew",  
	  item_category5: "Short sleeve",  
	  item_list_id: "related_products",  
	  item_list_name: "Related Products",  
	  item_variant: "green",  
	  location_id: "ChIJIQBpAG2ahYAR_6128GcTUEo",  
	  price: 9.99,  
	  quantity: 1  
  }] 
  }});
```

<br>

## 1.0.3 - view_item

<p>Kullanıcı, bir ürünü görüntülediğinde çalışmalıdır.</p>

```
dataLayer.push({ ecommerce: null });  // Clear the previous ecommerce object.
dataLayer.push({
  event: "view_item",
  ecommerce: {
    items: [
    {
      item_id: "SKU_12345",
      item_name: "Stan and Friends Tee",
      affiliation: "Google Merchandise Store",
      coupon: "SUMMER_FUN",
      currency: "USD",
      discount: 2.22,
      index: 0,
      item_brand: "Google",
      item_category: "Apparel",
      item_category2: "Adult",
      item_category3: "Shirts",
      item_category4: "Crew",
      item_category5: "Short sleeve",
      item_list_id: "related_products",
      item_list_name: "Related Products",
      item_variant: "green",
      location_id: "ChIJIQBpAG2ahYAR_6128GcTUEo",
      price: 9.99,
      quantity: 1
    }
    ]
  }
});
```

<br>

## 1.0.4 - add_to_cart

<p>Kullanıcı, bir ürünü sepete eklediğinde çalışmalıdır.</p>

```
dataLayer.push({ ecommerce: null });  // Clear the previous ecommerce object.
dataLayer.push({
  event: "add_to_cart",
  ecommerce: {
    items: [
    {
      item_id: "SKU_12345",
      item_name: "Stan and Friends Tee",
      affiliation: "Google Merchandise Store",
      coupon: "SUMMER_FUN",
      currency: "USD",
      discount: 2.22,
      index: 0,
      item_brand: "Google",
      item_category: "Apparel",
      item_category2: "Adult",
      item_category3: "Shirts",
      item_category4: "Crew",
      item_category5: "Short sleeve",
      item_list_id: "related_products",
      item_list_name: "Related Products",
      item_variant: "green",
      location_id: "ChIJIQBpAG2ahYAR_6128GcTUEo",
      price: 9.99,
      quantity: 1
    }
    ]
  }
});
```

<br>

## 1.0.5 - add_to_wishlist

<p>Kullanıcı, bir ürünü favorilere eklediğinde çalışmalıdır.</p>

```
dataLayer.push({ ecommerce: null });  // Clear the previous ecommerce object.
dataLayer.push({
  event: "add_to_wishlist",
  ecommerce: {
    currency: "USD",
    value: 7.77,
    items: [
    {
      item_id: "SKU_12345",
      item_name: "Stan and Friends Tee",
      affiliation: "Google Merchandise Store",
      coupon: "SUMMER_FUN",
      currency: "USD",
      discount: 2.22,
      index: 0,
      item_brand: "Google",
      item_category: "Apparel",
      item_category2: "Adult",
      item_category3: "Shirts",
      item_category4: "Crew",
      item_category5: "Short sleeve",
      item_list_id: "related_products",
      item_list_name: "Related Products",
      item_variant: "green",
      location_id: "ChIJIQBpAG2ahYAR_6128GcTUEo",
      price: 9.99,
      quantity: 1
    }
    ]
  }
});
```

<br>

## 1.0.6 - view_cart

<p>Kullanıcı, sepeti görüntülediğinde çalışmalıdır.</p>

```
dataLayer.push({ ecommerce: null });  // Clear the previous ecommerce object.
dataLayer.push({
  event: "view_cart",
  ecommerce: {
    currency: "USD",
    value: 7.77,
    items: [
    {
      item_id: "SKU_12345",
      item_name: "Stan and Friends Tee",
      affiliation: "Google Merchandise Store",
      coupon: "SUMMER_FUN",
      currency: "USD",
      discount: 2.22,
      index: 0,
      item_brand: "Google",
      item_category: "Apparel",
      item_category2: "Adult",
      item_category3: "Shirts",
      item_category4: "Crew",
      item_category5: "Short sleeve",
      item_list_id: "related_products",
      item_list_name: "Related Products",
      item_variant: "green",
      location_id: "ChIJIQBpAG2ahYAR_6128GcTUEo",
      price: 9.99,
      quantity: 1
    }
    ]
  }
});
```

<br>

## 1.0.7 - remove_from_cart

<p>Kullanıcı, sepetten ürün kaldırdığında çalışmalıdır.</p>

```
dataLayer.push({ ecommerce: null });  // Clear the previous ecommerce object.
dataLayer.push({
  event: "remove_from_cart",
  ecommerce: {
    items: [
    {
      item_id: "SKU_12345",
      item_name: "Stan and Friends Tee",
      affiliation: "Google Merchandise Store",
      coupon: "SUMMER_FUN",
      currency: "USD",
      discount: 2.22,
      index: 0,
      item_brand: "Google",
      item_category: "Apparel",
      item_category2: "Adult",
      item_category3: "Shirts",
      item_category4: "Crew",
      item_category5: "Short sleeve",
      item_list_id: "related_products",
      item_list_name: "Related Products",
      item_variant: "green",
      location_id: "ChIJIQBpAG2ahYAR_6128GcTUEo",
      price: 9.99,
      quantity: 1
    }
    ]
  }
});
```

<br>

## 1.0.8 - begin_checkout

<p>Kullanıcı, ödeme adımlarını başlattığında çalışmalıdır.</p>

```
dataLayer.push({ ecommerce: null });  // Clear the previous ecommerce object.
dataLayer.push({
  event: "begin_checkout",
  ecommerce: {
    items: [
    {
      item_id: "SKU_12345",
      item_name: "Stan and Friends Tee",
      affiliation: "Google Merchandise Store",
      coupon: "SUMMER_FUN",
      currency: "USD",
      discount: 2.22,
      index: 0,
      item_brand: "Google",
      item_category: "Apparel",
      item_category2: "Adult",
      item_category3: "Shirts",
      item_category4: "Crew",
      item_category5: "Short sleeve",
      item_list_id: "related_products",
      item_list_name: "Related Products",
      item_variant: "green",
      location_id: "ChIJIQBpAG2ahYAR_6128GcTUEo",
      price: 9.99,
      quantity: 1
    }
    ]
  }
});
```

<br>

## 1.0.9 - add_shipping_info

<p>Kullanıcı, teslimat bilgilerini tamamladığında çalışmalıdır.</p>

```
dataLayer.push({ ecommerce: null });  // Clear the previous ecommerce object.
dataLayer.push({
  event: "add_shipping_info",
  ecommerce: {
    currency: "USD",
    value: 7.77,
    coupon: "SUMMER_FUN",
    shipping_tier: "Ground",
    items: [
    {
      item_id: "SKU_12345",
      item_name: "Stan and Friends Tee",
      affiliation: "Google Merchandise Store",
      coupon: "SUMMER_FUN",
      currency: "USD",
      discount: 2.22,
      index: 0,
      item_brand: "Google",
      item_category: "Apparel",
      item_category2: "Adult",
      item_category3: "Shirts",
      item_category4: "Crew",
      item_category5: "Short sleeve",
      item_list_id: "related_products",
      item_list_name: "Related Products",
      item_variant: "green",
      location_id: "ChIJIQBpAG2ahYAR_6128GcTUEo",
      price: 9.99,
      quantity: 1
    }
    ]
  }
});
```

<br>

## 1.0.10 - add_payment_info

<p>Kullanıcı, ödeme bilgilerini tamamladığında çalışmalıdır.</p>

```
dataLayer.push({ ecommerce: null });  // Clear the previous ecommerce object.
dataLayer.push({
  event: "add_payment_info",
  ecommerce: {
    currency: "USD",
    value: 7.77,
    coupon: "SUMMER_FUN",
    payment_type: "Credit Card",
    items: [
    {
      item_id: "SKU_12345",
      item_name: "Stan and Friends Tee",
      affiliation: "Google Merchandise Store",
      coupon: "SUMMER_FUN",
      currency: "USD",
      discount: 2.22,
      index: 0,
      item_brand: "Google",
      item_category: "Apparel",
      item_category2: "Adult",
      item_category3: "Shirts",
      item_category4: "Crew",
      item_category5: "Short sleeve",
      item_list_id: "related_products",
      item_list_name: "Related Products",
      item_variant: "green",
      location_id: "ChIJIQBpAG2ahYAR_6128GcTUEo",
      price: 9.99,
      quantity: 1
    }
    ]
  }
});
```

<br>

## 1.0.11 - purchase

<p>Kullanıcı, satın alma işlemini tamamladığında çalışmalıdır.</p>

```
dataLayer.push({ ecommerce: null });  // Clear the previous ecommerce object.
dataLayer.push({
  event: "purchase",
  ecommerce: {
      transaction_id: "T_12345",
      affiliation: "Google Merchandise Store",
      value: 25.42,
      tax: 4.90,
      shipping: 5.99,
      currency: "USD",
      coupon: "SUMMER_SALE",
      items: [
       {
        item_id: "SKU_12345",
        item_name: "Stan and Friends Tee",
        affiliation: "Google Merchandise Store",
        coupon: "SUMMER_FUN",
        currency: "USD",
        discount: 2.22,
        index: 0,
        item_brand: "Google",
        item_category: "Apparel",
        item_category2: "Adult",
        item_category3: "Shirts",
        item_category4: "Crew",
        item_category5: "Short sleeve",
        item_list_id: "related_products",
        item_list_name: "Related Products",
        item_variant: "green",
        location_id: "ChIJIQBpAG2ahYAR_6128GcTUEo",
        price: 9.99,
        quantity: 1
      },
      {
        item_id: "SKU_12346",
        item_name: "Google Grey Women's Tee",
        affiliation: "Google Merchandise Store",
        coupon: "SUMMER_FUN",
        currency: "USD",
        discount: 3.33,
        index: 1,
        item_brand: "Google",
        item_category: "Apparel",
        item_category2: "Adult",
        item_category3: "Shirts",
        item_category4: "Crew",
        item_category5: "Short sleeve",
        item_list_id: "related_products",
        item_list_name: "Related Products",
        item_variant: "gray",
        location_id: "ChIJIQBpAG2ahYAR_6128GcTUEo",
        price: 20.99,
        promotion_id: "P_12345",
        promotion_name: "Summer Sale",
        quantity: 1
      }]
  }
});
```

<br>

## 1.0.12 refund - (Kısmi Geri Ödeme)

<p>Kullanıcı, siparişindeki bir veya daha fazla ürün için iade işlemi gerçekleştirdiğinde çalışmalıdır.</p>

```
dataLayer.push({ ecommerce: null });  // Clear the previous ecommerce object.
dataLayer.push({
  event: "refund",
  ecommerce: {
    currency: "USD",
    transaction_id: "T_12345",
    value: 12.21,
    affiliation: "Google Merchandise Store",
    coupon: "SUMMER_FUN",
    shipping: 3.33,
    tax: 1.11,
    items: [
    {
      item_id: "SKU_12345",
      item_name: "Stan and Friends Tee",
      affiliation: "Google Merchandise Store",
      coupon: "SUMMER_FUN",
      currency: "USD",
      discount: 2.22,
      index: 0,
      item_brand: "Google",
      item_category: "Apparel",
      item_category2: "Adult",
      item_category3: "Shirts",
      item_category4: "Crew",
      item_category5: "Short sleeve",
      item_list_id: "related_products",
      item_list_name: "Related Products",
      item_variant: "green",
      location_id: "ChIJIQBpAG2ahYAR_6128GcTUEo",
      price: 9.99,
      quantity: 1
    }
    ]
  }
});
```

<br>

## 1.0.13 refund - (Tam Geri Ödeme)

<p>Kullanıcı, siparişi için iade işlemi gerçekleştirdiğinde çalışmalıdır.</p>

```
dataLayer.push({ ecommerce: null });  // Clear the previous ecommerce object.
dataLayer.push({
  event: "refund",
  ecommerce: {
    currency: "USD",
    transaction_id: "T12345" // Transaction ID. Required for purchases and refunds.
    value: 12.21,
    affiliation: "Google Merchandise Store",
    coupon: "SUMMER_FUN",
    shipping: 3.33,
    tax: 1.11
  }
});
```

<br>

## 1.0.14 - view_promotion

<p>Kullanıcı, web sitesindeki bir promosyonu görüntülediğinde çalışmalıdır.</p>

```
window.dataLayer = window.dataLayer || [];
window.dataLayer.push({
  event: 'view_promotion',
  ecommerce: {
    items: [{
      promotion_id: 'sc2021',
      promotion_name: 'summer_campaign_2021',
      creative_name: 'family_in_bathing_suits_1',
      creative_slot: 'featured_items',
      location_id: 'ChIJ4Us9pPryjUYRn1MzXbSQuPA',
      item_id: "SKU_12345",
      item_name: "Stan and Friends Tee",
      affiliation: "Google Merchandise Store",
      coupon: "SUMMER_FUN",
      currency: "USD",
      discount: 2.22,
      index: 0,
      item_brand: "Google",
      item_category: "Apparel",
      item_category2: "Adult",
      item_category3: "Shirts",
      item_category4: "Crew",
      item_category5: "Short sleeve",
      item_list_id: "related_products",
      item_list_name: "Related Products",
      item_variant: "green",
      price: 9.99,
      quantity: 1
    },{
      promotion_id: 'wc2020',
      promotion_name: 'winter_campaign_2020',
      creative_name: 'family_in_winter_clothes_1',
      creative_slot: 'featured_items_2',
      location_id: 'ChIJ4Us9pPryjUYRn1MzXbSQuPA',
      item_id: "SKU_12345",
      item_name: "Stan and Friends Tee",
      affiliation: "Google Merchandise Store",
      coupon: "SUMMER_FUN",
      currency: "USD",
      discount: 2.22,
      index: 0,
      item_brand: "Google",
      item_category: "Apparel",
      item_category2: "Adult",
      item_category3: "Shirts",
      item_category4: "Crew",
      item_category5: "Short sleeve",
      item_list_id: "related_products",
      item_list_name: "Related Products",
      item_variant: "green",
      price: 9.99,
      quantity: 1
    }]
  }
});
```

<br>

## 1.0.15 - select_promotion

<p>Kullanıcı, web sitesindeki bir promosyona tıklama gerçekleştirdiğinde çalışmalıdır.</p>

```
window.dataLayer = window.dataLayer || [];
window.dataLayer.push({
  event: 'select_promotion',
  ecommerce: {
    items: [{
      promotion_id: 'sc2021',
      promotion_name: 'summer_campaign_2021',
      creative_name: 'family_in_bathing_suits_1',
      creative_slot: 'featured_items',
      location_id: 'ChIJ4Us9pPryjUYRn1MzXbSQuPA',
      item_id: "SKU_12345",
      item_name: "Stan and Friends Tee",
      affiliation: "Google Merchandise Store",
      coupon: "SUMMER_FUN",
      currency: "USD",
      discount: 2.22,
      index: 0,
      item_brand: "Google",
      item_category: "Apparel",
      item_category2: "Adult",
      item_category3: "Shirts",
      item_category4: "Crew",
      item_category5: "Short sleeve",
      item_list_id: "related_products",
      item_list_name: "Related Products",
      item_variant: "green",
      price: 9.99,
      quantity: 1
    }]
  }
});
```

<br>

## 2.0 | User-ID Entegrasyonu

## 2.0.1 - login

<p>Kullanıcı, web sitesinde oturum açtığında - sitede bulunan gtm.js öncesinde - çalışmalıdır.</p>

```
window.dataLayer = window.dataLayer || []; 
window.dataLayer.push({ 
'event' : 'login',
'email_permission' : {{dinamik değer}},
'sms_permission' : {{dinamik değer}},
'userId' : {{dinamik değer}} //gönderilen değer, CRM panelindeki ‘üye id’ ile eşdeğer olmalıdır. 
})

```

<br>

## 2.0.2 - sign_up

<p>Kullanıcı, web sitesinde kayıt işlemi gerçekleştirdiğinde - sitede bulunan gtm.js öncesinde - çalışmalıdır.</p>

```
window.dataLayer = window.dataLayer || []; 
window.dataLayer.push({ 
'event' : 'sign_up',
'email_permission' : {{dinamik değer}},
'sms_permission' : {{dinamik değer}},
'userId' : {{dinamik değer}} //gönderilen değer, CRM panelindeki ‘üye id’ ile eşdeğer olmalıdır. 
})

```

<br>


## 2.0.3 - user_data

<p>Kullanıcının web sitesinde üye girişi sağladıktan sonra bulunduğu bütün sayfalarda - sitede bulunan gtm.js öncesinde - çalışması gerekmektedir.</p>

```
window.dataLayer = window.dataLayer || []; 
window.dataLayer.push({ 
'event' : 'user_data',
'userId' : {{dinamik değer}} //gönderilen değer, CRM panelindeki ‘üye id’ ile eşdeğer olmalıdır. 
})

```

<br>

## 3.0 | Gelişmiş Form Takibi Entegrasyonu

## 3.0.1 - form_submission

<p>Kullanıcı, web sitesinde bulunan formları tamamladığında çalışmalıdır.</p>

```
window.dataLayer = window.dataLayer || [];
dataLayer.push({
    event: "form_submision",
    formID: "2345", //Form için bir ID değeri gönderilmelidir.
    formCategory: "İletişim Formu", //Formun kategori değeri gönderilmelidir.
    formStep: "2", //Formda bulunulan adımın değeri gönderilmelidir.

});

```

<br>

## 3.0.2 - form_step

<p>Web sitesinde bulunan formlarda birden fazla adım bulunduğu durumlarda her bir adımda çalışmalıdır.</p>

```
window.dataLayer = window.dataLayer || [];
dataLayer.push({
    event: "form_step",
    formID: "2345", //Form için bir ID değeri gönderilmelidir.
    formCategory: "İletişim Formu", //Formun kategori değeri gönderilmelidir.
    formStep: "2", //Formda bulunulan adımın değeri gönderilmelidir.
});

```

<br>

## 3.0.3 - form_click

<p>Web sitesinde bulunan formlarda her bir input değeri girildiğinde çalışmalıdır.</p>

```
window.dataLayer = window.dataLayer || [];
dataLayer.push({
    event: "form_click",
    formID: "2345", //Form için bir ID değeri gönderilmelidir.
    formCategory: "İletişim Formu", //Formun kategori değeri gönderilmelidir.
    formStep: 2, //Formda bulunulan adımın değeri gönderilmelidir.
    formInput: "email" //Form içerisinde kullanıcının tıkladığı input alanı girilmelidir. 
});

```

<br>

## 4.0 | Enhanced Conversion Entegrasyonu

## 4.0.1 - enhanced_conversion_data

<p>Kullanıcı, web sitesinde ilgili dönüşümü tamamladığında çalışmalıdır.</p>

```
'enhanced_conversion_data': {
        "email": 'E-mail adresi',
        "phone_number": '+90 555 111 22 33',
        "address": {
            "first_name": 'İsim',
            "last_name": 'Soyisim',
            "street": 'Sokak',
            "city": 'İl',
            "region": 'İlçe',
            "postal_code": 'Posta Kodu',
            "country": 'Ülke'
        }
    };

```

<br>
