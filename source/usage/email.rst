
Setup Email
###########

Need to config mail in Dashboard -> Email.

Support Mailgun, SendGrid, SES, Gmail, Sendmail... and other SMTP mail services. We suggest use Mailgun to send mail.

Make sure that you have saved settings (button Save settings at the bottom of page) before sending a test email.

.. image:: /images/settings.jpeg

Using Gmail
===========

Example:

.. image:: /images/settings_mail.jpeg

* Mail Driver: ``SMTP``
* Mail Host: ``smtp.gmail.com``
* Mail Port: ``587``
* Mail Encryption: ``tls``
* Mail Username: ``[your-gmail]``
* Mail Password: ``[password-app]`` (docs: https://support.google.com/mail/answer/185833?hl=en-GB )