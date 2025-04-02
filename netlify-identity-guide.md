# Netlify Identity Setup Guide

## 1. Go to Your Netlify Site Dashboard

After deploying your site, go to your Netlify dashboard and click on your site name.

## 2. Enable Identity

1. Click on the "Identity" tab in the top navigation
   ![Identity Tab](https://i.imgur.com/VrZnGq3.png)

2. Click the "Enable Identity" button
   ![Enable Identity](https://i.imgur.com/vXQkVFW.png)

3. Once enabled, you'll see the Identity dashboard
   ![Identity Dashboard](https://i.imgur.com/OkQj3Xs.png)

## 3. Configure Registration Settings

1. Under "Registration" click "Edit settings"
   ![Registration Settings](https://i.imgur.com/QAmgSEa.png)

2. Select "Invite only" to secure your CMS
   ![Invite Only](https://i.imgur.com/cexh5Le.png)

3. Click "Save"

## 4. Enable Git Gateway

1. Scroll down to "Services" section
   ![Services Section](https://i.imgur.com/HRKM0hC.png)

2. Click "Enable Git Gateway"
   ![Enable Git Gateway](https://i.imgur.com/VrU6NGP.png)

3. Confirm by clicking "Enable Git Gateway"
   ![Confirm Git Gateway](https://i.imgur.com/j1rJXQF.png)

## 5. Invite Users (Yourself)

1. Go back to the top of the Identity page
2. Click "Invite users"
   ![Invite Users](https://i.imgur.com/JSk55NU.png)

3. Enter your email address
   ![Enter Email](https://i.imgur.com/9kH7fhB.png)

4. Click "Send" to send the invitation

## 6. Accept the Invitation

1. Check your email for the invitation
2. Click the "Accept the invite" button in the email
   ![Accept Invite](https://i.imgur.com/RxCKxTG.png)

3. You'll be taken to your site to set a password
   ![Set Password](https://i.imgur.com/4yv9Tmb.png)

4. Create a password and click "Sign up"

## 7. Access the CMS

1. Go to your site URL followed by "/admin/" 
   (e.g., `https://your-site-name.netlify.app/admin/`)

2. Log in with your email and password

3. You should now see the Netlify CMS dashboard where you can edit your site
   ![CMS Dashboard](https://i.imgur.com/IuRoWvz.png)

## Troubleshooting

- **Can't see the Identity tab?** Make sure you're logged into Netlify and viewing your site's dashboard
- **Didn't receive invitation email?** Check your spam folder or resend the invitation
- **"Git Gateway Error"?** Make sure you've enabled Git Gateway and that your GitHub account has the correct permissions 