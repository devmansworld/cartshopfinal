 
    //1. Main page actions
    mainPage.visitMainPage();  
    : expected that this routine as a starter, opens main page 
    mainPage.viewProduct();    
    : expected that this test selects one product and displays its data correctly

    //2. Product Details page actions
    productDetailsPage.addToCart();  
    :expected that we find using the word "sleeve" to add thirty units of it to the cart 

    //3. Cart View page actions
     viewCartPage.proceedToCheckout(); 
     : expected that this action of clicking button, leads to checkout page

    //4. System will ask to go to registration
    viewCartPage.jumpToRegister();   
    : expected that this action shall bring up the registration form

    //5. Registration
    registrationPage.fillRegistrationForm(randomFirstName, randomLastName, randomEmail);
        : expected to fill up the form correctly with random generated data
        
    //6. The signup form 
    signupPage.fillSignupForm(randomFirstName, randomLastName, randomEmail, randomPassword,randomAddress, randomState,           randomCity, randomZipcode, randomMobileNumber);
       : expected this also generates random data to fill up the sign up form , then submit

    //7. Validation of account created
    accountCreatedPage.validateAccountCreated();
       : expected this shall ensure that account has been created

    //8. Navigate from success to Cart
    mainPage.goToCart();
      : expected that after creating the account we go to cart

    //9. From cart proceed to go to checkout
    viewCartPage.proceedToCheckout();
      : expected that in the cart the checkout button leads to checkout

    //10. To verify if checkout loads fine
    checkoutPage.verifyCheckoutPage();
      : expected that the checkout page loads ok

    //11. Placing the order after the checkout
    checkoutPage.placeOrder();
      : expected that after the checkout we generate a shop order

    
    //12. Redirected to payment, fill the form
     paymentPage.fillPaymentForm();
     : expected to fill in the payment form using random data
     
    //13. Confirm the payment for the order   
    paymentPage.payAndConfirmOrder();
     : expected to submit the order with its payment ok

    //14. Once the order is placed we verify existence
    orderPlacedPage.verifyOrderPlacedPage();
     : expected to find a order placed message with details

    //15. the download invoice optional
    orderPlacedPage.downloadInvoice();
      : expected to get us a text file with purchase information as an invoice

    //16. process ends up after the button continue
     orderPlacedPage.continueShopping();
      : expected to generate movement bring user back to main page
  
 
