## Konular
	# 1.0 E-Ticaret
	# 2.0 User-ID
	# 3.0 Formlar
## E-Ticaret Dökümantasyonu

## view_item_list

> Site içerisinde bir ürün listesi görünümünde çalışmalıdır

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
<h2>select_item</h2>
<p>Site içerisinde bir ürün tıklandığında çalışmalıdır</p>

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
<h2>view_item</h2>
<p>Kullanıcı bir ürün görüntüleme işlemi yaptığında çalışmalıdır.</p>

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
<h2>add_to_cart</h2>
<p>Kullanıcı bir ürünü sepete eklediğinde çalışmalıdır.</p>

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
<h2>add_to_wishlist</h2>
<p>Kullanıcı bir ürünü favorilere eklediğinde çalışmalıdır.</p>

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