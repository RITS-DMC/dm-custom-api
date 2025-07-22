**Step 1:**
Copy the project files to your BAS workspace.

**Step 2:**
Run the following commands to create the required services in Cloud Foundry:
cf create-service destination lite dm-custom-api-destination
cf create-service xsuaa application cap-custom-api-auth

**Step 3:**
Push the dm-custom-api to Cloud Foundry.

**Step 4:**
Create the service key SAP_DMC_DEFAULT_SERVICE_KEY in the Destination service.
Export this key from the RITS DMC tenant and import it into your BTP tenant.
This will authorize the service through the protected XSUAA instance.

**Step 5:**
Test the API using Postman and verify it works as expected before using it in the production process.
Note: test the API in Postman, provide the Client ID, Client Secret, and Token URL




