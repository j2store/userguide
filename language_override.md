## Language overrides in Joomla (with examples using J2Store)

To change text in core Joomla or in an extension (other than installing a new language) it is advised to perform a language override in Joomla. To do this you need to go into the admin backend then in the menu under "Extensions" click on "Language Manager"

Let us assume that you want to change the Firstname (in billing address fields) to My Name.

Step 1: Go to Joomla admin->Extensions Manager->Language Manager->Overrides.

> VERY IMPORTANTANT:    
Before creating the override, set the Filter to ADMINISTRATOR (of the language that you wanted to create override. Say, your language is german. Then you should select the German (de-DE) Administrator in the filter)

![Location Filter](./assets/images/location_filter.png)

Step 2: Click new to create a override

> VERY IMPORTANT   
1. Make sure you have checked the For both locations   
2. Make sure the location points to ADMINISTRATOR   

![Language override screen](./assets/images/override_screen.png)

Step 3: You can either search or directly enter the constant (if you knew already) to create the override.

Method 1: Searching

Under the Search text you want to change, enter the following text (as you see in the site): Firstname and hit search.
You will get the constant: J2STORE_FIRST_NAME

Method 2: Find the constant from the language file.

Let us take J2Store as example. All the language constants of J2Store can be found in the following file
/administrator/language/en-GB/en-GB.com_j2store.ini

Step 4: Now you have the constant. Enter the constant in the Language Constant box.

Step 5: Enter your value (in our example My Name) in the Text box.

Step 6: Save.

You can create as many overrides as you like in this method.

#### Video tutorials

**[Method 1](https://www.j2store.org/support/video-tutorials/language-override-by-searching-language-constant.html)**

**[Method 2](https://www.j2store.org/support/video-tutorials/language-override-by-referring-language-file.html)**