## Konu Başlıkları
	# 1.0 Gelişmiş E-Ticaret Takibi Entegrasyonu
	# 2.0 User-ID Entegrasyonu
	# 3.0 Gelişmiş Form Takibi Entegrasyonu

## 1.0 | Gelişmiş E-Ticaret Takibi Entegrasyonu

## 1.0.1 view_item_list

> Kullanıcıya belirli bir kategorideki öğelerin listesi sunulduğunda çalışmalıdır.

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

## 1.0.2 select_item

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

## 1.0.3 view_item

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

## 1.0.4 add_to_cart

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

## 1.0.5 add_to_wishlist

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

## 1.0.6 view_cart

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

## 1.0.7 remove_from_cart

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

## 1.0.8 begin_checkout

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

## 1.0.9 add_shipping_info

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

## 1.0.10 add_payment_info

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

## 1.0.11 purchase

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

## 1.0.12 refund (Kısmi Geri Ödeme)

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

## 1.0.13 refund (Tam Geri Ödeme)

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

## 1.0.14 view_promotion

<p>Kullanıcı, web sitesindeki bir promosyonu görüntülediğinde çalışmalıdır.</p>

```
dataLayer.push({ ecommerce: null });  // Clear the previous ecommerce object.
dataLayer.push({
  event: "view_promotion",
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

## 1.0.15 select_promotion

<p>Kullanıcı, web sitesindeki bir promosyona tıklama gerçekleştirdiğinde çalışmalıdır.</p>

```
dataLayer.push({ ecommerce: null });  // Clear the previous ecommerce object.
dataLayer.push({
  event: "select_promotion",
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




//Form tamamlandığında
window.dataLayer = window.dataLayer || [];
dataLayer.push({
    event: "user_form_submit",
    formID: "2", //Formun id bilgisi girilmeli
    formCategory: "Araç Form", //Formun kategorisi girilmeli
    formStep: 2, //Form eğer ki birden fazla adımlı ise adım bilgisi girilmeli
});

//Form input tıklandığında
window.dataLayer = window.dataLayer || [];
dataLayer.push({
    event: "user_form_click",
    formID: "2", //Formun id bilgisi girilmeli
    formCategory: "Araç Form", //Formun kategorisi girilmeli
    formStep: 2, //Form eğer ki birden fazla adımlı ise adım bilgisi girilmeli
    formInput: "email" //Form içerisinde kullanıcının tıkladığı input değeri girilmelidir. 
});
