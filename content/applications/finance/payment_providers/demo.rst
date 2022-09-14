=====================
Demo payment provider
=====================

Odoo's **Demo Payment Provider** is an online payment provider intended to test business flows
involving online transactions without requiring real banking credentials.

.. seealso::
   :doc:`../payment_providers`

Installation
------------

From Odoo's main dashboard, go into the **Apps** application, search for `demo`, and install the
:guilabel:`Demo Payment Provider` module. If the search gives no result, make sure no search filters
are applied.

.. image:: demo/demo-payment-icon.png
   :align: center
   :alt: Demo Payment Provider icon.

Features
--------

Payment outcome
~~~~~~~~~~~~~~~

Upon checkout or when paying a bill online, you can choose the payment outcome when using the demo
payment provider. To do so, simply click on the :guilabel:`Payment Status` drop-down menu and select
the desired outcome.

.. image:: demo/demo-payment-outcome.png
   :align: center
   :alt: Payment status outcomes.

Transaction state
~~~~~~~~~~~~~~~~~

You can change the state of a transaction straight from its view form.

.. image:: demo/demo-view-form.png
   :align: center
   :alt: Transaction's status view form.

To access a transaction's view form, activate the :ref:`developer mode <developer-mode>`, press
**CTRL/⌘ + K** and search for `/transactions`. Click either on
:guilabel:`Accounting/Configuration/Payments/Payments Transactions` or
:guilabel:`Website/Configuration/eCommerce/Payment Transactions`. Change the status of a transaction
by clicking on the state (:guilabel:`Draft, Pending, Authorized, Confirmed, Canceled, Error`).

Displayed as
~~~~~~~~~~~~

Enter the name you wish the **Demo Provider** to appear as during the test. Leave the field blank if
you prefer to leave it as default *(Demo Payment Provider)*.

Supported payment icons
~~~~~~~~~~~~~~~~~~~~~~~

Select the icons of the supported payment methods you want to display, such as *VISA, PayPal, etc*.

Allow saving payment methods
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Also known as **tokenization**, this option allows to save the payment method for future
transactions. Check the :guilabel:`Allow Saving Payment Methods` box to enable the feature.

.. note::
   In the case of real transactions, you remain fully PCI-compliant when enabling this feature as
   Odoo does not store the card details directly. Instead, it creates a payment token that only
   holds a reference to the card details stored on the payment provider’s server.

Manual capture
~~~~~~~~~~~~~~

This feature allows testing payment captures in two steps instead of one. When you authorize a
payment, the funds are (in the case of real transactions) reserved on the customer's payment method
but they are not immediately charged. The charge is only made when you manually decide to capture
the payment at a later date.

Check the :guilabel:`Capture Amount Manually` box to enable the feature.

Refunds
~~~~~~~

You can refund payments directly from Odoo, it does not need to be enabled first. To refund a
payment, navigate to it by going to :menuselection:`Accounting --> Customers --> Payments`, and then
click on the :guilabel:`Refund` button.

Fees
~~~~

Under the :guilabel:`Fee` tab, you can find the option to add **extra fees** on transactions. Once
the :guilabel:`Add Extra Fees` box checked, the following options are available:

- **Fixed** fees are determined by the amount entered in the field. The amount is then added to the
  tax-included price.

- **Variable** fees are determined by the percentage entered in the field. The percentage is
  calculated on the tax-included price and then added to the price.

- **Domestic fees** are applied only to transactions occurring within the country of the company
  configured in the :menuselection:`General Settings --> Companies`.

- **Variable** fees are applied only to transactions occurring outside of the country of the
  company.