# Reverting back to 2.x after the migration

VERY IMPORTANT: Apply the following steps only if you migrated from 2.8.x to 3.x and then want to downgrade.
You should be familiar with Joomla tables and PhpMyAdmin operations.
Otherwise, **NEVER EVER** attempt this if you DO NOT understand any of the steps below.


**Step 1:** Backup your site using Akeeba Backup

**Step 2: ** Uninstall J2Store version 3

**Step 3:** Go to Phpmyadmin

You will see

a. Tables with the follwing prefix: 

```_v2_j2store_```  = These are your 2.x tables backed up by the migration tool

b. Tables with the prefix:
```_j2store_``` = these are J2Store 3.x tables

Delete the tables with the prefix ```_j2store_```

Rename the ```_v2_j2store_``` tables to ```_j2store_```

Example: ```_v2_j2store_orders``` to ```_j2store_orders```

**Step 4:** Install J2Store 2.8.x version
