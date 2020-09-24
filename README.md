<h2 style="color:red">Filer On Sale Product / Discount Product </h2>
Ref:  https://lakewood.media/woocommerce-add-sales-filter/
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
