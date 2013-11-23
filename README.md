ci-merchant-extended
======================================

Modified CI-Merchant Library

This library is modified by me!! (Paypal Express only). I managed to add "item list" to this library, so from single trasanction to multiple transaction is now possible.

Example code:

$params = array(
	'amount' => '10',
	'currency' => 'USD',
	'return_url' => site_url('thankyou'),
	'cancel_url' => site_url('cancelled'),
	'items' => array(
		'item_name' => $this->input->post('item_name'),
		'item_qty' => $this->input->post('qty'),
		'item_price' => $this->input->post('item_price')
	)
);

NOTE:
each post data are arrays