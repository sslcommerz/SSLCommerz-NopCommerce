# SSLCommerz - NopCommerce V4.20

### Prerequisites

1. .NET Core
2. [Sandbox Account](https://developer.sslcommerz.com/registration/ "SSLCommerz Sandbox Registration")

### Installation:
1.	Unzip SSLCommerz plugin file, you will get a folder named `Payments.SSLCommerz`
2.	Copy the folder to “Presentation\Nop.Web\Plugins” or your plugins directory
3.	Go to your administrator panel, Open the plugins configuration by going to `Configuration > Plugins > Local plugins`
4.	Find `SSLWireless / SSLCommerz` in the plugins list and click the install button on the right.

### Configuration:
1.	After installing you can see `Configure` Button right under the name of the plugin.
2.	Click Configure and you will find the configuration page where you need to give your merchant store ID and password for both sandbox(dummy) and live transactions. For sandbox please check the `Use Sandbox` checkbox.
3.	Now go to `Configuration > Payment > Payment Methods` Page, where you will see the list of payment methods available for your website. Click the edit button and select the “is active” check box to active SSLCommerz payment method. Also, you can set order to display the payment option to the customer if you have multiple payment options.
4.	Please ensure that you have not selected SSLCommerz as payment restriction for `Bangladesh` from `Configuration > Payment > Payment Restriction` as it will prevent to display SSLCommerz payment option to the customer.
5.	Now you are ready to take payment using SSLCommerz gateway. Please do some transaction to check if everything is working fine. Check the order details if payment is showing as `PAID` in both customer and admin side. 

### IPN Setting:
1.	Go to your merchant panel, given by our SSLCommerz manager whom you are contacting.
2.	There you will find an option to set IPN (Instant payment notification), It is used for instant payment notification to your website if by somehow your customer can not reach you after payment completion.
3.	Update your IPN URL by putting <Your store url>/Plugins/SSLCommerz/PaymentHandler
	Example: https://www.myonlinestore.com/Plugins/SSLCommerz/PaymentHandler
4.	Now you payment plugin can know about each transaction that your customer made even if they did not returned for complete the order.

> integration@sslcommerz.com
