=====================
django_localflavor_si
=====================

Country-specific Django helpers for Slovenia.

=======
WARNING
=======

This app has been superseded by the newly created django-localflavor_ app
which recombines all the different country locaflavors again (after having
been removed from Django). Development and maintenance of this app has
stopped and is only left online as a reminder for the users of those apps.
It will be removed after grace period of 1 Django release (~spring 2014).

.. _django-localflavor: https://github.com/django/django-localflavor/

What's in the Slovenia localflavor?
===================================

* forms.SIEMSOField: A form field that validates input as Slovenian personal
  identification number and stores gender and birthday to self.info dictionary.

* forms.SITaxNumberField: A form field that validates input as a Slovenian tax
  number. Valid input is SIXXXXXXXX or XXXXXXXX.

* forms.SIPhoneNumberField: A form field that validates input as a Slovenian
  phone number. Phone number must contain at least local area code with
  optional country code.

* forms.SIPostalCodeField A form field that provides a choice field of major
  Slovenian postal codes.

* forms.SIPostalCodeSelect: A ``Select`` widget that uses a list of major
  Slovenian postal codes as its choices.

See the source code for full details.

About localflavors
==================

Django's "localflavor" packages offer additional functionality for particular
countries or cultures.

For example, these might include form fields for your country's postal codes,
phone number formats or government ID numbers.

This code used to live in Django proper -- in django.contrib.localflavor -- but
was separated into standalone packages in Django 1.5 to keep the framework's
core clean.

For a full list of available localflavors, see https://github.com/django/
