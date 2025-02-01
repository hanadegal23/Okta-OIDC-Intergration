# Okta-OIDC-Integration
# Custom OIDC Application with Okta

## Project Overview

This project demonstrates the integration of a custom OpenID Connect (OIDC) application using Okta for authentication. The application is hosted on Glitch and showcases how to set up an OIDC flow, including retrieving ID and access tokens.

## Technologies Used
- **Okta**: Identity provider for OIDC.
- **OpenID Connect (OIDC)**: Authentication protocol.
- **HTML/CSS/JavaScript**: Frontend technologies for building the user interface.
- **Glitch**: Hosting platform for the web application.

## Step-by-Step Guide

### Step 1: Create OIDC Application in Okta
1. Log in to your Okta tenant.
2. Click on **Create Application Integration**.
    <p align="center">
OIDC App Selection via OIN: <br/>
<img src="https://i.imgur.com/YHlSoxz.png" height="80%" width="80%" alt="OIN App Creation"/>
<br />
<br />

3. Choose **OpenID Connect (OIDC)** as the sign-in method.
4. Select **Single Page Application** as the application type.
     <p align="center">
Create App Integration via OIN: <br/>
<img src="https://i.imgur.com/kn8hegO.png" height="80%" width="80%" alt="OIDC App Selection"/>
<br />
<br />  





### Step 2: Configure Application
1. Add a name for your application.
2. Choose the grant type as **Authorization Code**.

### Step 3: Set Redirect URIs
1. Accept the default name.
2. Add the redirect URIs required for your application.
3. Click **Next** to proceed.

### Step 4: Create a Glitch Account
1. Go to [Glitch](https://glitch.me).
2. Click on **Sign Up** or log in with your Google account.

### Step 5: Start a New Glitch Project
1. Open the following playlist: [Glitch Playlist](https://glitch.com/search?q=military-rounded-fabrosaurus).
2. Click on the project link.
3. Remix (clone) another project to generate a new URL.

### Step 6: Modify Project Files
1. In your Glitch project, navigate to `index.html` on the left sidebar.
2. Update the following in your project:
   - **client-id**: Replace with your Okta client ID.
   - **redirect URI**: Set it to your Glitch project URL.
   - **Okta tenant base URL**: Update with your Okta domain.

### Step 7: Update Redirect URI in Okta
1. Go back to your Okta tenant.
2. Replace the default/dummy redirect URI with the URI from your Glitch project.
3. Remember to click **Save**.

### Step 8: Add Trusted Origin
1. Navigate to **Security > API > Trusted Origins** in Okta.
2. Click **Add Origin** and paste your redirect URI.
3. Check the **CORS** and **Redirect** boxes, then click **Save**.

### Step 9: Test Your Application
1. Start your Glitch project.
2. Visit your Glitch project URL (e.g., `https://pleasant-economic-salad.glitch.me/`).
3. Click the login button to initiate the authentication process.

### Step 10: Explore Tokens
1. After logging in, you will receive an ID Token and an Access Token.
2. Copy the token and go to [JWT.io](https://jwt.io).
3. Paste the token in the debugger to inspect its contents.

### Note on Token Calls
- Observe how the tokens are retrieved and utilized in your application. This process is essential for ensuring secure communication between your application and Okta.

## Conclusion
This project successfully integrates a custom OIDC application with Okta, demonstrating how to configure the application and handle authentication flows securely. For any questions or further assistance, please feel free to reach out.

---

Feel free to modify any sections or add additional details specific to your project!
