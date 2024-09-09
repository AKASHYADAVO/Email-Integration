
Linking Your Website's Email with Web3Forms
This document outlines the steps to connect your website's email with Web3Forms to receive form submissions.
1. Get Your Web3Forms Access Key:
Head over to Web3Forms (https://web3forms.com/) and create a free account.
Upon signup, you'll receive an access key – this key is crucial for linking your form submissions to your email.
2. Craft the HTML Form:
Open your website's HTML file and insert a contact form. Here's an example:

HTML


<form action="https://api.web3forms.com/submit" method="POST">
  <input type="hidden" name="access_key" value="YOUR_ACCESS_KEY_HERE">
  <input type="text" name="name"    placeholder="Your Name" required>
  <input type="email" name="email" placeholder="Your Email" required>
  <textarea name="message" placeholder="Your Message" required></textarea>
  <button type="submit">Send</button>   
</form>


Important! Replace "YOUR_ACCESS_KEY_HERE" with the actual key you received from Web3Forms.
3. Customize Email Settings (Optional):
Want to personalize how form responses arrive in your email? Web3Forms allows configuring optional fields:
Redirect URL: Add <input type="hidden" name="redirect" value="https://your-website.com/thank-you"> to redirect users to a custom "Thank You" page after submitting the form.
Custom Subject Line: Add <input type="hidden" name="subject" value="New Contact Form Submission"> to set a specific subject line for the email notification.
4. Testing the Form:
Upload your updated HTML file to your web server.
Submit a test form entry and verify if it reaches your email.
Remember to check both your inbox and spam folder.
5. Styling and Enhancements:
Use CSS to style your form for a seamless integration with your website's design.
For extra features, consider integrating JavaScript to implement real-time form validation or display post-submission alerts.
6. Go Live!
Once you've tested the form thoroughly and everything functions smoothly, deploy your website or update the form on your live site.
Congratulations! You've successfully set up Web3Forms to efficiently and securely manage your website's email submissions.
