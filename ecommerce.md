## Konular
	# 1.0 E-Ticaret
	# 2.0 User-ID
	# 3.0 Formlar

## 1.0 | E-Ticaret Dökümantasyonu

## 1.0.1 view_item_list

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
## 1.0.2 select_item
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
## 1.0.3 view_item
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
## 1.0.4 add_to_cart
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
## 1.0.5 add_to_wishlist
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
