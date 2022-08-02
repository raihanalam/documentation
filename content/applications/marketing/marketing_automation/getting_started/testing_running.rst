Testing & running a campaign
============================

Odoo gives users the ability to test marketing campaigns (and mailings) before officially running
them.

First, open the :guilabel:`Marketing Automation` application and click on the campaign. Make sure
the campaign already has activities configured on it. To start a test, click the :guilabel:`Launch a
Test` button at the top of the template form.

.. image:: testing_running/launch-test.png
   :align: center
   :alt: Launch a test button in Odoo Marketing Automation.

When clicked, a pop-up appears, in which the user can choose a specific record to run the test on,
or the user can create a brand new record to test.

.. image:: testing_running/launch-test-popup.png
   :align: center
   :alt: Launch test popup in Odoo Marketing Automation.

Once the record is selected, click :guilabel:`Continue`, and Odoo will redirect to the campaign
test page.

.. image:: testing_running/test-screen.png
   :align: center
   :alt: Test screen in Odoo Marketing Automation.

Here, the name of the :guilabel:`Record` being tested is visible, along with the precise time this
test workflow was started. Beneath that is the first activity (or activities) in the workflow.

To start a test, click the :guilabel:`Run` icon beside the first activity in the workflow. When
clicked, the page will reload, and Odoo will show the various results (and analytics) connected to
that specific activity.

.. image:: testing_running/workflow-test-progress.png
   :align: center
   :alt: Workflow test progress in Odoo Marketing Automation.

Once all the workflow activities are completed, the test will end and be moved to the
:guilabel:`Completed` stage. To stop a test before all the workflow activities are completed, click
the :guilabel:`Stop` button.
