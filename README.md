# Crumb & Co. Bakery Website — BIT303 Capstone Prototype

A responsive front-end prototype for a bakery website. It includes a sample product menu, category filters, shopping bag, pick-up checkout, order reference numbers, order tracking, and a simple staff order dashboard.

## Run locally
1. Extract the ZIP file.
2. Open `index.html` in a modern browser, or open the folder in Visual Studio Code and use Live Server.
3. Browse the menu, add products to the bag, and place a test pick-up order using fictional details.
4. Track the order with its generated `CC-XXXXXX` reference.
5. Open the staff dashboard by adding `#admin` to the page URL (for example `http://127.0.0.1:5500/index.html#admin`).

## Current prototype limitations
- Orders are saved in browser `localStorage` only. They are not shared across devices or browsers.
- No live payments, real email notifications, or real authentication are connected.
- The bakery name, menu, prices, business address, and opening hours are sample content and should be confirmed with a real stakeholder before submission.
- Use fictional customer information while testing.

## Planned AWS architecture
- Amazon S3: static website hosting
- Amazon API Gateway: secure HTTP API endpoint
- AWS Lambda: order and menu business logic
- Amazon DynamoDB: persistent order and product data
- Amazon Cognito: staff sign-in (optional depending on final scope)
- AWS IAM: least-privilege permissions
- Amazon CloudWatch: logs and monitoring

The next implementation stage is to replace the local browser storage calls with API requests to API Gateway, backed by Lambda and DynamoDB. Do not deploy publicly or enter real customer details until authentication, validation, access controls, and privacy requirements have been implemented and tested.
