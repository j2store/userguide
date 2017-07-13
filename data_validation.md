# Data Validation

The data validation app is especially useful in the checkout page. With the data validation app you can create rules so that only valid data from the customer is accepted into the various checkout fields. A checkout field that requires the phone number of the customer can be configured to accept only a number input from the customer. You can also set it to reject special characters and alphabets. This way the customer will be informed to only enter a valid phone number, address or any other details in the checkout field.

## Requirements

1. Joomla 3.x
2. J2Store 3.2.5 or higher
3. PHP version 5.4 or higher

### Installation

1. Download Data validation app from our site and install it using Joomla installer.
2. After installing, from Joomla backend go to J2Store > Apps and find Data validation app.
3. Click on Enable to activate the app.
4. Click on Open to configure basic settings of the app.

#### Configuration

Opening the app will show you 3 coulmn table.

- Custom fields
- Rules Apply for
- Rules

**Custom Fields**

All the custom field you have in J2Store custom fields section (J2Store > Setup > Custom fields) will be listed in this column.

**Rules Apply for**

You can choose at which section (Billing, Shipping, Payment) the rule should be applied. Choose Billing or shipping or payment or all the three.

**Rules**

Click on "Add Rules" button will display the dropdown lists six types of rules. You can select the rule to be applied from the dropdown list.

Available rules are:

- Max.length
- Min.length
- Numeric
- Alphabet
- Alphanumeric
- Phone

You can add multiple rules to every individual field.

#### Example

If you would like to apply rules for the field "Mobile" so that customer should enter only number in the field.

Go to the field Mobile and navigate to the column **Rules Apply for** and choose the section where you actually would like to apply the rules. If you choose Billing, the validation rule will be applied only at Billing section.

Now move to the column "Rules" and click Add Rules button. Choose the rules from the dropdown list. In our case, choose Numeric and click save button.

#### Screenshots

![](./assets/images/data-validation-01.png)

![](./assets/images/data-validation-02.png)
