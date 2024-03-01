 
    // 1 . Main page actions
    mainPage.visitMainPage();
    mainPage.viewProduct();

    // 2. Product Details page actions
    productDetailsPage.addToCart();

    // 3. Cart View page actions
  viewCartPage.proceedToCheckout();

  // 4. System will ask to go to registration
  viewCartPage.jumpToRegister();

   // 5. Registration
  registrationPage.fillRegistrationForm(randomFirstName, randomLastName, randomEmail);
  
  // 6. The signup form 
  signupPage.fillSignupForm(randomFirstName, randomLastName, randomEmail, randomPassword, randomAddress, randomState, randomCity, randomZipcode, randomMobileNumber);

  //7. Validation of account created
  accountCreatedPage.validateAccountCreated();

  //8. Navigate from success to Cart
  mainPage.goToCart();

  // 9. From cart proceed to go to checkout
  viewCartPage.proceedToCheckout();

  //10 To verify if checkout loads fine
  checkoutPage.verifyCheckoutPage();

  //11 Placing the order after the checkout
  checkoutPage.placeOrder();

    
// 12 Redirected to payment, fill the form
   paymentPage.fillPaymentForm();
  
 // 13 Confirm the payment for the order   
  paymentPage.payAndConfirmOrder();

    // 14 Once the order is placed we verify existence
    orderPlacedPage.verifyOrderPlacedPage();

    //15 the download invoice optional
    orderPlacedPage.downloadInvoice();

    //16 process ends up after the button continue
     orderPlacedPage.continueShopping();
  
  });
});
