# Shopping Cart

Thanks for checking out this cool shopping cart project! Read the steps below to learn how to set up your local environment so that you can use it to log your grocery purchases and get a receipt sent to your email.

## Prerequisites

+ Anaconda 3.7+
+ Python 3.7+

## Installation

Fork this [remote repository](https://github.com/zky44/shopping-cart) under your own control, then clone your remote copy onto your local computer.

Next, navigate there from the command line (subsequent commands assume you are running them from the local repository's root directory):

```sh
cd shopping-cart
```

If you haven't done so yet, use anaconda to create and activate a new virtual environment. A suggestion would be to call it "shopping-env":

```sh
conda create -n shopping-env python=3.8
conda activate shopping-env
```

From inside the virtual environment, install package dependicies:

```sh
pip install -r requirements.txt
```

> NOTE: if this command throws you an error, make sure you are running it from the repository's root directory where the requirements.txt file exists. Refer back to the initial `cd` step above

## Updating Your Inventory Prior to Use

In the "Products" list on the shopping_cart.py file, you can add, remove, or change the name, department, aisle, or price of different grocery items.  

## Email Receipt Setup (Optional)

If you want to receive an email with a receipt of your purchases, you will have to set up a secret file to store your email and API code. In the root directory of your local respository, create a new file called ".env", and update the contents of the file to specify your desired email and API code (directions above). An example line of code is shown below:

```sh

PLAYER_NAME ="Tom Brady"
```

>IMPORTANT: the ".env" file is usally the place for passing configuration options and secret credentials, so as a best practrice we don't upload this file to version control. Make sure that you add the code in this [.gitignore](/.gitignore) file, most importantly line 2, to your ".gitignore" file.

## Using the Shopping Cart Software

To use the software, run the code below in your command line editor:

```py
python shopping_cart.py

Then, insert each product you bought according to its product "id" number in the products list of the shopping_cart.py file.
When you are finished, type the text "DONE." You will see your receipt. If you set up receiving email receipts in the step above, you will also receive a digital copy of your receipt in your chosen email inbox.
