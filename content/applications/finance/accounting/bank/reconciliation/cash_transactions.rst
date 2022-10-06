===================
Cash reconciliation
===================

Overview
========

By default in Odoo, payments registered in the **cash journal** are automatically reconciled with an
**outstanding account** and their related invoices or bills marked as *In Payment* until they are
reconciled with a bank statement. It is possible to :ref:`bypass <bypass>` the *In Payment* status
for cash transactions, therefore removing the need to reconcile with a bank statement.

.. image:: cash_transactions/cash-inpayment-status.png
   :align: center
   :alt: In Payment status of invoice or bill.

Cash logs
=========

At the start of each day, create a **cash log**. To do so, click on :guilabel:`New transaction` in
the **cash** journal.

.. image:: cash_transactions/new-transaction.png
   :align: center
   :alt: Create a new cash log.

Enter the starting balance of your cash float in the :guilabel:`Starting Balance` field and save,
but do *not* post the entry yet. Create your invoice(s) in :menuselection:`Accounting dashboard -->
Customers --> Invoices` and select the :guilabel:`Cash` journal when registering the payment of an
invoice.

.. image:: cash_transactions/cash-payment-journal.png
   :align: center
   :alt: Select Cash journal upon payment registration.

Go back to the **accounting dashboard**, and click again on :guilabel:`New transactions`. Click on
the :guilabel:`Add a line` button in the :guilabel:`Transactions` tab, and enter the total of cash
earned during the day. Add a label name according to your needs. Input the amount of
:guilabel:`Computed Balance` in the :guilabel:`Ending Balance`, and make sure it matches your end
cash float.

Once certain the **computed balance** is correct, click :guilabel:`Save`, :guilabel:`Post`, and
finally :guilabel:`Reconcile`. This will take you to the **bank reconciliation** page.

Cash payments reconciliation
============================

On the **bank reconciliation** page, head to the **cash log** transaction you created earlier, and
match each cash payment with your cash log. To be able to match all cash payments, make sure no
**partner** is selected in the :guilabel:`Select Partner` field. If a **partner** is selected,
simply click on the field and pick the blank option from the drop-down menu. When you are done,
click on :guilabel:`Validate`.

.. image:: cash_transactions/cash-payment-reconciliation.png
   :align: center
   :alt: Cash payments reconciliation.

.. note::
   If your ending cash balance is **over** or **under** the computed balance, you will need to add
   another :guilabel:`Transaction` line corresponding to the **over** or **under** amount in order
   to match it later during reconciliation.

Cash reconciliation bypass
==========================

.. _bypass:

.. important::
   Bypassing the cash journal is recommended **only for organizations** that do not need a
   cash report or do not wish to reconcile cash.

To bypass the *In Payment* status, go to :menuselection:`Accounting dashboard --> Configuration -->
Journals` and select the **cash** journal. Click on the :guilabel:`Payments Configuration` tab and
set a `Cash` account in both fields :guilabel:`Outstanding Receipts Account` and
:guilabel:`Outstanding Payments Account`, then save. Payments registered in the **cash** journal now
bypass the *In Payment* status.

.. image:: cash_transactions/cash-payments-config.png
   :align: center
   :alt: Configuration tab of the cash journal.

.. tip::
   In case you use cash to pay expenses, advance employees, are required to keep record of cash
   flows, or use anything resembling a cash box, you can benefit from creating a second **cash
   journal** that *does* use the **outstanding accounts**. This way, you can both generate *and*
   reconcile bank statements when closing your POS session or your books at the end of the day.