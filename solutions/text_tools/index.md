---
layout: solution
title: Text Tools for Workdocs
image_path: "/assets/images/text_tools/text_tools3_1.png"
video_path: "/assets/media/text_tools/text_tools_full"
introduction: This app is designed to make formatting, editing, and working with text easier, faster, and more efficient.
whatyouget: With just a few clicks, you can
arguments:
  - name: Analyze Content
    arg: Quickly count words, characters and sentences. Estimate reading time to better target your audience.
  - name: Transform Text
    arg: Instantly convert selected text to UPPERCASE, lowercase, Sentence case, Title Case, or create URL-friendly slugs.
  - name: Find and Replace
    arg: Easily search and replace specific words or phrases inside your document without needing external tools.

images:
- path: "/assets/images/text_tools/Review_Screenshot.png"
  alt: Review feature
- path: "/assets/images/text_tools/Transform_uppercase_Screenshot.png"
  alt: Transform feature
- path: "/assets/images/text_tools/Replace_Screenshot.png"
  alt: Replace feature

monday_install_button: |-
  <a href="https://auth.monday.com/oauth2/authorize?client_id=dab9741df949b23c6aa8c5a333098f6a&response_type=install">
    <img
      alt="Add to monday.com"
      height="32"
      src="https://dapulse-res.cloudinary.com/image/upload/f_auto,q_auto/remote_mondaycom_static/uploads/Tal/4b5d9548-0598-436e-a5b6-9bc5f29ee1d9_Group12441.png"
    />
  </a>

monday_share_url:

pricing:
  f14d_trials: true
  plans:
  - name: Solo
    app_plan_id: solo
    seats: 5
    monthly: 0
    yearly: 0
    features:
    - Unlimited Reviews
    - Unlimited Transformations
    - Unlimited Replace text
  - name: Team
    app_plan_id: team
    seats: 15
    monthly: 5
    yearly: 3
    features:
    - Unlimited Reviews
    - Unlimited Transformations
    - Unlimited Replace text
  - name: Business
    app_plan_id: business
    seats: 50
    monthly: 8
    yearly: 5
    features:
    - Unlimited Reviews
    - Unlimited Transformations
    - Unlimited Replace text
  - name: Pro
    app_plan_id: pro
    seats: 250
    monthly: 13
    yearly: 8
    features:
    - Unlimited Reviews
    - Unlimited Transformations
    - Unlimited Replace text
  - name: Enterprise
    app_plan_id: enterprise
    seats: Unlimited
    monthly: 21
    yearly: 13
    features:
    - Unlimited Reviews
    - Unlimited Transformations
    - Unlimited Replace text

terms_of_service:
- section: Introduction
  arg_type: paragraph
  arg: Welcome to Find and Replace app ("the App"), a monday.com application that enables users to search and replace text in WorkDocs documents. By installing, accessing, or using the App, you agree to be bound by these Terms of Service ("Terms"). If you do not agree with these Terms, do not use the App.
- section: Acceptance of Terms
  arg_type: paragraph
  arg: By using the App, you affirm that you have the legal capacity to enter into these Terms and that you comply with all applicable laws and regulations. If you are using the App on behalf of an organization, you represent that you have the authority to bind that organization to these Terms.
- section: Description of Service
  arg_type: paragraph
  arg: The App provides a tool for users of monday.com to search for and replace text within WorkDocs documents. It does not store, retain, or modify content outside of the user's control within monday.com. The App requires appropriate permissions to access WorkDocs documents, and by using the App, you grant such permissions.
- section: User Responsibilities
  arg_type: list
  arg: You agree to
  args:
  - Use the App only for lawful purposes and in compliance with monday.com’s terms and policies. 
  - Ensure you have the necessary permissions to modify WorkDocs content. 
  - Not use the App to introduce harmful code, automate unauthorized modifications, or violate intellectual property rights.
- section: Data Privacy and Security
  arg_type: paragraph
  arg: The App does not store or collect user data outside of monday.com. All processing occurs within monday.com’s platform, and any changes made via the App remain within the user’s workspace. We do not share or sell user data. For more details on how monday.com handles data, please refer to monday.com’s privacy policy.
- section: Limitation of Liability
  arg_type: paragraph
  arg: To the maximum extent permitted by law, [Company Name] is not liable for any indirect, incidental, special, or consequential damages, including but not limited to data loss, unauthorized modifications, or business disruptions resulting from the use of the App.
- section: Warranty Disclaimer
  arg_type: paragraph
  arg: The App is provided "as is" without any warranties, express or implied. We do not guarantee that the App will be error-free, uninterrupted, or meet your specific needs.
- section: Modification of Terms
  arg_type: paragraph
  arg: We reserve the right to update or modify these Terms at any time. Changes will be posted within the App or on our website, and continued use of the App after modifications constitutes acceptance of the revised Terms.
- section: Contact Information
  arg_type: paragraph
  arg: For any questions or concerns about these Terms, please contact us at montools@proton.me or visit our website at montools.github.io.

privacy_policy:
- section: Introduction
  arg: Welcome to Montools Find & Replace for WorkDocs ("the App").This Privacy Policy outlines how we handle user data when you use the App within monday.com.
- section: Data Collection & Usage
  arg: The App does not collect, store, or transmit any personal or document data outside of monday.com. All search and replace actions occur within the monday.com environment without external data processing.
- section: Permissions & Access
  arg: To function correctly, the App requires access to monday.com WorkDocs. This access is used solely for executing search and replace operations as initiated by the user. The App does not retain, analyze, or share document data.
- section: Data Security
  arg: We follow best practices to ensure that user data remains secure.  The App operates entirely within monday.com's infrastructure and does not introduce additional data storage, logging, or external processing.
- section: Third-Party Integrations
  arg: The App does not integrate with external third-party domains/services/products and does not transmit any user data outside of monday.com.
- section: User Rights & Control
  arg: As the App does not store any personal or document data, users do not need to request data deletion or modification. All content remains under the control of the user within their monday.com account.
- section: Changes to This Policy
  arg: We may update this Privacy Policy from time to time. Any changes will be communicated within the App or through our website. Continued use of the App after changes constitutes acceptance of the updated policy.
- section: Contact Information
  arg: For any questions regarding this Privacy Policy, please contact us at <email>montools@proton.me</email>.

faqs:
- question: What does this app do?
  answer: This app enhances text editing in monday.com Workdocs by offering formatting tools and text analysis directly in the contextual toolbar.

- question: Where can I access the app?
  answer: The app becomes visible when you select text in a Workdoc. It appears in the contextual toolbar above the selection.

- question: How this app calculates the sentences count? I get some differences when comparing with other tools.
  answer: |
    Yeap, different tools could arise different counts depending how they process the information. 
    The process in this app is the following: 
    <ol style="padding-left: 20px;">
      <li>trim the spaces from the text</li> 
      <li>then split the text by the delimiters '.!?' using the regular expression <b>`/([.!?]\s*)/g`</b></li>
      <li>and finally counting the result, which is considered the count of sentences</li>
    </ol>

- question: How this app calculates the words count? I get some differences when comparing with other tools.
  answer: |
    Yeap, different tools could arise different counts depending how they process the information. 
    The process in this app is the following:
    <ol style="padding-left: 20px;">
     <li>trim the spaces from the text</li>  
    <li>then split the text by set of consecutive alphabetical characters joining '/' and '-' symbols (for including composed words like "third-party" and "XLS/CSV") using the regular expression <b>`/\b[a-zA-Z]+(?:[-/][a-zA-Z]+)*\b/g`</b></li> 
    <li>and finally counting the result, which is considered the count of words</li> 

- question: What formatting options are available?
  answer: You can convert selected text to UPPERCASE, lowercase, Sentence case, Title Case, Slug, or Snake case format.

- question: What analysis features does the app include?
  answer: The app provides word count, character count, sentence count, and estimated reading time.

- question: Can I find and replace text with this app?
  answer: |
    Yes. The app includes a simple find-and-replace feature for modifying the selected content.

- question: Does this app change the entire document?
  answer: No. The app only affects the portion of text you have selected.

- question: Is the app available in all monday.com accounts?
  answer: Yes. It works inside any Workdoc as long as the app is installed in your monday.com workspace.

- question: Is my data secure when using this app?
  answer: Yes. The app processes text locally within your document and does not store or transmit your data externally.

- question: Who can I contact for support or feedback?
  answer: You can reach out to montools@proton.me, we'll be happy to know about you!
---