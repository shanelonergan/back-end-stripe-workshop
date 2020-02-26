# Stripe API Workshop

## Goal

Integrate Stripe payment processing into a React-Rails project

*Note:* There are many, many ways to use the Stripe API. This way is simply one I found to be relatively straightforward.

## Tools

- React
- Ruby on Rails
- Dotenv
- React-stripe-checkout

## Safety

We are dealing with both API Keys and payment processing, so it is very important we keep safety in mind while working with Stripe. To do this be sure to remember three things:

1. Make sure your Stripe account is in Test mode (it comes in test mode by default), and you are using the Test API keys.
2. Make sure your API keys are properly hidden
3. Never use real CC information while testing

## Overview

1. Create Stripe Account, set up environment variables
2. Integrate Checkout in front-end, pass token to back-end
3. Set up controller in back-end to handle token and create Charge
4. Check stripe account for activity

Feel free to clone the starter repos and follow along:

- Front-end: https://github.com/shanelonergan/front-end-stripe-workshop
- Back-end: https://github.com/shanelonergan/back-end-stripe-workshop

## Front End

1. Set up dotenv
2. Install `react-stripe-checkout`
3. Add `<StripeCheckout />` component
4. Create `onToken` function

## Back End

1. Add gems (dotenv and stripe)
2. Set up dotenv
3. Create charge controller
4. Don't forget to add the route!
5. Bonus: error handling
