# Conditionals

![Choose a branch of logic based on a condition.](../../.gitbook/assets/conditional.png)

{% hint style="info" %}
For an overview on conditionals in WayScript, refer to the [Introduction to Conditionals](../../getting_started/conditionals.md).
{% endhint %}

## ![](../../.gitbook/assets/conditional.png) Condition Block

You will use this block to define a logic expression.

To create a logic expression, you will typically define values for the two Variable fields and then select how you want to compare them using the Comparison field.

![The Condition Block consists of a Variable and a Comparison \(often to the value of another Variable\).](../../.gitbook/assets/screen-shot-2019-08-22-at-9.58.37-am.png)

{% hint style="info" %}
Some comparisons, such as "Has Increased," "Has Decreased," "Has a Value," or "Does Not Have a Value," do not require a second variable input.
{% endhint %}

## 🔎 Comparison Field

After defining a value for the first Variable, you can select an option for the Comparison field.

![Select a Comparison Option](../../.gitbook/assets/screen-shot-2019-08-22-at-10.00.00-am.png)

{% hint style="warning" %}
You will not be able to select a value for the Comparison field until a value for the first Variable has been defined.
{% endhint %}

### 🔢 Number Comparison Options

* Is The Same As
* Is Not The Same As
* Is Greater Than
* Is Greater Than or Equal To
* Is Less Than
* Is Less Than or Equal To
* Has Changed By
* Has Not Changed By
* Has Increased By
* Has Decreased By
* Has a Value
* Does Not Have a Value

### 🔤 Text and List Comparison Options

* Is The Same As
* Is Not The Same As
* Contains
* Is Contained In
* Is Not Contained In
* Shares any Items With
* Has Any Items
* Has Changed
* Has Not Changed
* Has a Value
* Does Not Have a Value

### 📆 Date Comparison Options

* Is The Same As
* Is Before
* Is After
* Has Changed By
* Has Not Changed By
* Has a Value
* Does Not Have a Value

### 🔠 Case Sensitive Comparison

For non-Number fields, you will have the option to compare in a Case Sensitive manner. \(Default comparison is Case Insensitive.\)

![](../../.gitbook/assets/screen-shot-2019-07-16-at-9.05.14-pm.png)

### 📈 "Changed By" Comparisons

For "Changed By," "Increased/Decreased By," and similar comparisons, you can optionally choose the amount by which you want to check the value has changed. You can also choose whether to compare to the Original Value of the variable, or the Last \(most recent\) Value.

![](../../.gitbook/assets/screen-shot-2019-08-22-at-10.01.50-am.png)

{% hint style="info" %}
To see the "Since" field, click the "Show Advanced Settings" checkbox.
{% endhint %}

## \*\*\*\*➕ **Adding Multiple Conditions**

By pressing the **+ Add Condition** button, you can add additional conditions.

### 💡 Logical Operators

* **And:** Use if you want your expression to evaluate to `True` only when _**both**_ conditions are `True`.
* **Or:** Use if you want your expression to evaluate to `True` when _**at least one**_ of your conditions are `True`.

![](../../.gitbook/assets/screen-shot-2019-08-22-at-10.09.45-am.png)

## ![](../../.gitbook/assets/conditional.png) **If / Else-If / Else**

The **If** branch will run if your logic expression evaluates to `True`.

The **Else-If** branch will run if the proceeding logic expression evaluates to `False`, but the logic expression in the current Else-If branch evaluates to `True`.

The **Else** branch will run if all of the proceeding logic expressions evaluate to `False`.

![](../../.gitbook/assets/screen-shot-2019-08-22-at-10.13.17-am.png)

In the image above, if Temperature is greater than or equal to 90, the first branch will run. Otherwise, if the temperature is less than or equal to 65, the second branch will run. Finally, if the temperature is less than 90, but greater than 65, the else branch will run.

Click the **+ Add "Else If"** button to add more Else-If conditions.

![](../../.gitbook/assets/screen-shot-2019-08-22-at-10.16.57-am.png)

## \*\*\*\*🌤 **Example**

In the below example, if the value of the variable "Temperature" is between 65 and 90, then the program will print _"It's a nice day!"_.

Else, if the "Temperature" variable is outside of this range, then the program will print _"It's too cold!"_.

The program will then continue to run the rest of the modules following the If / Else statement.

![](../../.gitbook/assets/example%20%281%29.png)

