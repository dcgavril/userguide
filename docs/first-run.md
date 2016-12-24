If you've just finished installing DomainMOD and are wondering how to start using it, this section is for you. We'll walk you through the first few steps you need to take with a new installation, and after completing the steps below you'll be ready to start adding your domains.

If you haven't yet installed DomainMOD, please see the [Getting Started](getting-started.md) section.

Login
-----
The first thing you need to do is login to your new DomainMOD installation. The default username and password are "admin", and after you login for the first time you'll be prompted to change your password, which you should do immediately.

The admin account that gets created during installation has full control of your DomainMOD installation, so you should store the password in a safe place.

Assets
-------
After you've logged in you'll need to add a couple pieces of information to the system before you can start adding your domains. We'll refer to these pieces of information as Assets, and they're the building blocks of DomainMOD. Assets include things like the domain registrars that you use, your domain registrar accounts, the categories you want to use for grouping similar domains, and so on.

Since every domain must have an owner and belong to a domain registrar and domain registrar account, these are the first Assets that we'll need to add to DomainMOD. The easiest way to proceed with the next steps is to think of one of your domain registrar accounts, and use its details as you walk through the below sections. 

Add An Owner
---------------
Although recommended, adding an owner at this stage is optional. If you don't add one now you can use the default owner "[no owner]" for the remaining steps on this page, and you can then go back later and edit the default owner.

The owner should be whoever owns the registrar account that you're going to add, whether it's your personal name or a company name. 

1. Click on **Assets** on the main menu.

2. Click on **Account Owners** on the Assets list.

3. Click on the **Add Owner** button.

4. Enter the Owner's Name. 

5. Click the **Add Owner** button.

Add A Domain Registrar
------------------------
1. Click on **Assets** on the main menu.

2. Click on **Domain Registrars** on the Assets list.

3. Click on the **Add Registrar** button.

4. Enter the Registrar's Name. (Optional) Fill in the other fields on the page.

5. If you have access to this domain registrar's API you should select the registrar on the dropdown list in the **API Support** section.

6. Click the **Add Domain Registrar** button.

Add A Domain Registrar Account
---------------------------------
1. Click on **Assets** on the main menu.

2. Click on **Domain Registrar Accounts** on the Assets list.

3. Click the **Add Registrar Account** button.

4. Choose the domain registrar and account owner that this registrar account belongs to, and enter the registrar account's username. (Optional) Fill in the other fields on the page.

    **NOTE:** The registrar account password is currently stored in plain text in the database, and for security reasons we don't actually recommend saving it here, though we give you the option for your convenience.

5. If you have access to this registrar's API you can fill in your API access information in the **API Credentials** section. 

6. Click the **Add Registrar Account** button.

Start Adding Domains
----------------------
Congratulations, you've added all of the required Assets and you're ready to start adding your domains to DomainMOD! The software gives you a few options for adding your domains, so you should read through the below sections to determine which will work best for you.

**Domain Queue**  
The easiest option for adding domains is to use the Domain Queue, which allows you to supply a list of domains and let DomainMOD take care of the rest. This option uses your domain registrar's API to retrieve information required to add domains, so unfortunately it only works if your registrar has an API and support for it has been built into DomainMOD. Before using this option make sure your API credentials have been saved with your registrar account.

Currently Supported Registrars: DNSimple, Dynadot, eNom, Fabulous, GoDaddy, Internet.bs, Name.com, NameBright, Namecheap, NameSilo, OpenSRS, ResellerClub

**NOTE:** In order to use the Domain Queue you must first [setup the cron job](getting-started.md#cron-job) that comes with DomainMOD.

[Click here to add domains using the Domain Queue &raquo;](domain-queue.md)

**Bulk Updater**  
The Bulk Updater also allows you to supply a list of domains to be added, however you need to manually choose the options for the domains you're adding, and all of the domains will have the same settings. The Bulk Updater generally works best if you're adding a list of newly registered domains, since they will have the same expiry date and will generally have the same settings.

[Click here to add domains using the Bulk Updater &raquo;](bulk-updater.md) 

**Manually**  
Domains can also be added one-by-one, which allows you to choose custom settings for each domain.

[Click here to add domains manually &raquo;](adding-content.md#add-a-domain)
