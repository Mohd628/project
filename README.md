# QR-vCard



### __Summary__

For my **CS50P** [Final Project](https://cs50.harvard.edu/python/2022/project/), I decided to create a single purpose, cross-platform desktop application with a functional GUI that generates vCards in QR code format.

### __Video Demo__

For my **CS50P** [Final Project](https://cs50.harvard.edu/python/2022/project/), I decided to create a single purpose, cross-platform desktop application with a functional GUI that generates vCards in QR code format.
## video Demo: 

## CREATED BY
   *MOHD RAZZAK*

### Description

This is a single purpose desktop application that allows a user to enter contact details into a GUI that then generates a quick response code image. These QR code images can be scanned by most modern mobile devices that have a camera. QR code images allow for the ability to embed contact details on business cards, resumes, or even artwork.

The reason I chose this project was to learn how to create micro-applications for niche use-cases, and in turn learn more lightweight ways of presenting code functionality to end-users in non-technical settings. My reasoning being that good programmers should be able to help non-programmers solve problems by creating tools that simplify tasks and processes.

</br>
<hr>
</br>

#### Requirement of Libraries __



***qrcode*** 
Generating QR codes
***Pillow***  Image formatting support
         
***DearPyGui*** Cross-platform GUI framework 

***DearPyGui-Ext*** Bundled light theme for DearPyGui


### __vCard Format__

The vCard, or otherwise known as the VCF (Virtual Contact File) format is essentially a container format for contact information that can be shared between electronic devices, notably mobile phones.

With every entry on a new line, the `.vcf` format must always begin with `BEGIN:VCARD`, followed immediately by the version identifier `VERSION:4.0`, and must end with `END:VCARD`.

#### Example layout

```bash
BEGIN:VCARD
VERSION:4.0
KIND:individual
EMAIL;TYPE=work:j.appleseed@acmeappleco.bar
EMAIL;TYPE=work:j.appleseed@foo.bar
TITLE:Apple Seed Distributor
ROLE:Project Leader
FN:Johnny Appleseed
BDAY:19850412
ADR;TYPE=HOME:pobox;ext;street;locality;region;code;country
TEL;TYPE=CELL:+123 12 123 1234
TEL;TYPE=WORK:+123 12 12 1234
TEL;TYPE=HOME:+123 12 12 1234
TEL;TYPE=FAX:+123 12 12 1234
URL: https://www.example.com
TZ: Africa/Windhoek
ORG: ACME Apple Co. - Will take precedence over Full Name.
NOTE: optional note, keep it short
END:VCARD
```

</br>
<hr>
</br>

### __Testing and Development Dependencies__

To set up a development environment for this project with `pipenv`:

``` bash
make dev
```

To perform unittests with `pytest`:

``` bash
make tested
```

Or, if you don't have `build-essential` installed.

```bash
# install development dependencies
pipenv install --dev

# perform unittest
pipenv run pytest
```

</br>
<hr>
</br>

### __Acknowledgements__

Thank you to David Malan and his entire team for helping to make Harvard's CS50 accessible to anyone who wants to learn.


