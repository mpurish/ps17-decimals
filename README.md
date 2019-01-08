# ps17-decimals

# Files to update:

# override/classes/Cart.php
# override/classes/CartRule.php
# override/classes/PaymentModule.php
# override/classes/Product.php
# override/classes/order/Order.php
# override/classes/order/OrderDetail.php
# override/classes/order/OrderHistory.php
# override/classes/order/OrderInvoice.php
# override/classes/order/OrderReturn.php
# override/classes/order/OrderSlip.php
# override/classes/stock/SupplyOrderDetail.php

# override/controllers/front/ProductController.php
# override/controllers/front/CartController.php
# override/controllers/admin/AdminOrdersController.php

# src/Core/Cart/CartRow.php
# src/Core/Product/ProductPresenter.php

# themes/_core/js/cart.js
# themes/_core/js/product.js

# themes/decimals/_dev/js/cart.js
# themes/decimals/_dev/js/listing.js
# themes/decimals/_dev/js/product.js

# admin-dev/themes/default/template/controllers/orders/_product_line.tpl



# DB tables to update updates:


# ALTER TABLE ps_cart_product MODIFY quantity FLOAT(12,2);
# ALTER TABLE	ps_cart_rule MODIFY quantity FLOAT(12,2);
# ALTER TABLE	ps_cart_rule MODIFY quantity_per_user FLOAT(12,2);

# ALTER TABLE  ps_cart_rule_product_rule_group MODIFY quantity FLOAT(12,2);
# ALTER TABLE	ps_customization MODIFY quantity FLOAT(12,2);
# ALTER TABLE	ps_customization MODIFY quantity_refunded FLOAT(12,2);
# ALTER TABLE	ps_customization MODIFY quantity_returned FLOAT(12,2);

# ALTER TABLE	ps_order_detail MODIFY product_quantity FLOAT(12,2);
# ALTER TABLE	ps_order_detail MODIFY product_quantity_in_stock FLOAT(12,2);
# ALTER TABLE	ps_order_detail MODIFY product_quantity_refunded FLOAT(12,2);
# ALTER TABLE	ps_order_detail MODIFY product_quantity_return FLOAT(12,2);
# ALTER TABLE	ps_order_detail MODIFY product_quantity_reinjected FLOAT(12,2);

# ALTER TABLE	ps_order_return_detail MODIFY product_quantity FLOAT(12,2);
# ALTER TABLE	ps_order_slip_detail MODIFY product_quantity FLOAT(12,2);

# ALTER TABLE	ps_pack MODIFY quantity FLOAT(12,2);

# ALTER TABLE	ps_product MODIFY quantity FLOAT(12,2);
# ALTER TABLE	ps_product MODIFY minimal_quantity FLOAT(12,2);

# ALTER TABLE	ps_product_attribute MODIFY quantity FLOAT(12,2);
# ALTER TABLE	ps_product_attribute MODIFY minimal_quantity FLOAT(12,2);

# ALTER TABLE	ps_product_attribute_shop MODIFY minimal_quantity FLOAT(12,2);

# ALTER TABLE	ps_product_sale MODIFY quantity FLOAT(12,2);

# ALTER TABLE	ps_product_shop MODIFY minimal_quantity FLOAT(12,2);

# ALTER TABLE	ps_specific_price MODIFY from_quantity FLOAT(12,2);
# ALTER TABLE	ps_specific_price_rule MODIFY from_quantity FLOAT(12,2);


# ALTER TABLE	ps_stock MODIFY physical_quantity FLOAT(12,2);
# ALTER TABLE	ps_stock MODIFY usable_quantity FLOAT(12,2);

# ALTER TABLE	ps_stock_available MODIFY quantity FLOAT(12,2);
# ALTER TABLE	ps_stock_available MODIFY physical_quantity FLOAT(12,2);
# ALTER TABLE	ps_stock_available MODIFY reserved_quantity FLOAT(12,2);

# ALTER TABLE	ps_stock_mvt MODIFY physical_quantity FLOAT(12,2);

# ALTER TABLE	ps_supply_order_detail MODIFY quantity_expected FLOAT(12,2);
# ALTER TABLE	ps_supply_order_detail MODIFY quantity_received FLOAT(12,2);

# ALTER TABLE	ps_supply_order_receipt_history MODIFY quantity FLOAT(12,2);