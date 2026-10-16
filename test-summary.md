# Test Summary — E-commerce Web Application

## Objective and scope

This independent portfolio project evaluates key customer-facing workflows on an e-commerce storefront using black-box testing. Coverage includes homepage/navigation, product browsing and search, cart and wishlist behavior, registration/login, checkout and order summary, and basic UI/usability checks. Testing was performed through the visible interface without source-code or backend-log access.

## Execution overview

The accompanying workbook records 57 test cases with scenarios, steps, expected and actual results, status, and notes. The bug-report workbook contains 10 findings. Statuses reflect the observations recorded during testing. Some scenarios are marked as needing verification where the behavior was ambiguous or the feature could not be fully exercised.

## Key observations

- **Product image rendering:** Some product images displayed broken-image indicators, while others remained in an indefinite loading state.
- **Cart and account state:** Browser Back/Forward navigation after a brand search appeared to change the visible sign-in and cart state.
- **Checkout pricing:** The displayed subtotal, tax, shipping, and total appeared inconsistent in the observed checkout flow. The actual amount charged was not verified because payment was left pending.
- **Shipping threshold:** Free-shipping behavior appeared inconsistent after the cart value changed. The exact threshold rule should be confirmed before classifying the behavior as a defect.
- **Input validation:** Address, phone, and postal-code/location combinations raised validation questions that need clear requirements and repeatable evidence.
- **Search edge cases:** Searches using special characters returned the same large result count; further checks are needed to determine whether the search was ignored or a full-catalog fallback was intended.
- **Repeated cart action:** Ten Add to Cart clicks from a wishlist resulted in one cart row with quantity 10. This remains a potential usability concern unless expected button behavior is established.

## Areas that appeared to work in the tested examples

Navigation and normal refresh behavior; product detail navigation; selected product information, filters, sorting, and pagination; basic cart quantity changes; several registration/login checks; empty-cart and required-field checks; and opening the checkout/payment flow.

These observations are limited to the scenarios exercised and do not establish complete feature coverage.

## Limitations and follow-up

- No source code, server logs, or backend data were available.
- Payment was not completed, so the actual charged amount was not verified.
- Expected business rules should be confirmed for shipping thresholds, tax inclusion, search fallback, and repeated Add to Cart actions.
- Additional screenshots, browser/device details, repeat runs, and regression tests would improve confidence.
- Findings should be reclassified as confirmed defects only after the expected behavior is established and the issue is reproducible.

## Conclusion

The exercise demonstrates a structured approach to manual QA: mapping workflows, writing test cases, exploring edge cases, recording observed behavior, and clearly flagging uncertainty instead of overstating conclusions.
