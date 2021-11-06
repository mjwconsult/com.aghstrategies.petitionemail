# Petition Email

This extension allows the easy setup of automatic emails to a decision-maker upon signing a CiviCRM petition.

It uses the CiviCRM outbound email system, which makes it configurable, but for obvious reasons, deliverability is not guaranteed.  Likewise, this is for sending all messages for a given petition to the same email address.  This isn't going to find your member of Congress or anything.

## Usage

When creating or editing a petition, you can check a box to choose to have it deliver emails.
When you do so, you'll need to set the recipient's name and email, the custom field that will have the user's message,
the default message, and the message subject.  You will need to create the custom field first - it must be a Note/Textarea field that's in a custom data set that applies to activities (optionally limited to petition activities).  When you create the field, you should then add it to a profile that you will want to set as the activity profile on the petition.

When someone fills out the petition, they'll see the text box populated with your default message.  If they don't touch it or if they delete it entirely, the default message will be sent.  Otherwise, the message they type will be sent.  It will appear to come from the signer's name and email address, but you will have to be sure to include name and email fields in your contact profile on the petition.
