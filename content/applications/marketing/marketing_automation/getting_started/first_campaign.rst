====================
Marketing Automation
====================

The Odoo Marketing Automation application can automate a variety of marketing tasks, duties, posts,
and messages. Doing so provides more time to work on more important projects, without neglecting
marketing responsibilities.

Marketing templates
===================

Marketing templates quickly (and efficiently) create marketing campaigns in Odoo.

.. image:: first_campaign/marketing-template-sample.png
   :align: center
   :alt: A typical marketing template sample.

To create a new automated marketing campaign, open the :guilabel:`Marketing Automation` app and
click :guilabel:`Create`. On the :guilabel:`Campaign` page, there are the following smart buttons
and fields:

- :guilabel:`Templates`: represents the number of pre-configured mail templates being used in this
  particular campaign. (Templates can always be created on-the-fly as well).
- :guilabel:`SMS`: represents the number of personalized SMS messages connected to this campaign.
- :guilabel:`Clicks`: represents the number of times attached links have been clicked by recipients
  of this campaign.
- :guilabel:`Participants`: represents the number of contacts that have directly participated in
  this campaign.
- :guilabel:`Target`: this field is a drop-down menu to choose which model is targeted by this
  campaign (i.e., by Contacts, Sales Order, Lead/Opportunity, etc.).

Campaign filters
================

To add a filter to the target audience, click :guilabel:`Add Filter`, and a node field will
appear. In the node field, a custom equation can be configured for Odoo to use when filtering who
to include (and exclude) in this specific marketing campaign.

.. image:: first_campaign/filter-node.png
   :align: center
   :alt: A filter node in Odoo Marketing Automation.

Odoo provides users with the opportunity to customize their target audience by creating rules that
records must match in order to be involved in the marketing campaign.

When the first field of the node is clicked, a massive drop-down menu of options appears on the
screen, in which the user can choose which criteria best fits the needs of the campaign.

The remaining fields allow the user to further define the criteria that determines which records to
include (or exclude) in the execution of this campaign.

To add another node, simply click the :guilabel:`+ (plus sign)` icon to the right of the filtering
rule.

To add a branch of multiple nodes at the same time, click the :guilabel:`... (ellipses)` icon.

For further information on filters, refer to :doc:`this documentation page <target_audience>`.

.. note::
   :guilabel:`Records` represent the number of contacts in the system that fit the specified
   criteria for a campaign.
   
.. seealso::
   - :doc:`testing_running`
   - :doc:`workflow_activities`
   