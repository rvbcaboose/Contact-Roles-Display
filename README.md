Contact-Roles-Display
=====================

Display contact roles in Contact Detail SF page.

Components
===========
Two visualforce components are created for Account and Contact Roles:
        1. ContactAccountRoles
        2. ContactOpportunityRoles
These both take almost similar attributes, like
        * contactId [REQUIRED] : ID of Contact record
        * title [OPTIONAL] : If a title should be shown at rendered page block.
        * showAccountRecordType/showOppRecordType [OPTIONAL] : Boolean (true/false) to show / hide record type column for Account/Opp
        * noRolesMessage [OPTIONAL] : Boolean (true/false) to show message in case contact is not part of Opp or Account roles

ex. code :

<c:ContactOpportunityRoles contactId="{!Contact.Id}" showOppRecordType="true" noRolesMessage="true"/>

<c:ContactAccountRoles contactId="{!Contact.Id}"  title="Account Roles" showAccountRecordType="true" noRolesMessage="false"/>

Pages to include in Contact Detail
===================================
Here are two VF pages to include in contact detail layout
        1. ContactAccountRoles.page
        2. ContactOpportunityRoles.page

