# Shared Privacy Policy Template

Version: 1.0 / Created: 2026-11-15
English translation of privacy-policy.ja.md, version 1.0.

This document is a drafting template. Each app's official policy is published at site/<service-slug>/privacy-policy/index.html.
This template is visible in the public repository, but templates is not included in the GitHub Pages deployment.
Replace all {{...}} placeholders and remove drafting notes before incorporating the text into a published policy.
Do not publish by changing only the app name. Check the implementation, SDKs, form settings, and store disclosures. Do not claim that information is not collected when this has not been verified.

## What to check before drafting

- App name, operating system, version, operator, and contact details
- Types of data, purposes, storage locations, recipients, retention periods, and deletion methods
- SDKs and actual settings for advertising, analytics, diagnostics, purchases, authentication, and cloud synchronization
- Device permissions, OS backups, and user-initiated sharing
- Google Forms questions, required fields, email collection, attachments, and automatic attachments
- Any additional disclosures or consent needed for the intended age groups and distribution regions
- Consistency with in-app information and store disclosures

Keep verification evidence and internal specifications in each app's private repository.

---

# {{App name}} Privacy Policy

This policy explains how information is handled in "{{App name}}" for {{operating system}} (the "App"). The provider of the App, {{operator name and public profile}}, is referred to below as the "Operator."

Effective date: {{YYYY-MM-DD}}
Last updated: {{YYYY-MM-DD}}

## 1. Information Handled by the App

We process and store {{types of data}} in {{storage and processing locations, such as the device or a server}} for {{specific purposes}}.

{{Example wording — use only if verified: No account registration is required to use the App. The App does not automatically transmit records you enter to the Operator's servers.}}

{{If data is transmitted, specify the information, recipients, purposes, and circumstances in which transmission occurs. Also explain user-initiated sharing.}}

## 2. Retention and Deletion

{{For each type of information, describe the retention period or criteria used to determine it, in-app deletion methods, account deletion methods, and any information retained after deletion, including the reasons and retention period.}}

{{For on-device storage, explain whether the Operator holds the data, what uninstalling the App removes, and whether data may remain in OS backups or synchronized storage. Match the implementation; do not make a blanket statement that uninstalling deletes everything.}}

## 3. External Services and Disclosure to Third Parties

{{For each service used, list its name, provider, types of information, purposes, transmission conditions, and official privacy policy URL. Remove items that do not apply.}}

- Advertising: advertising SDKs, personalization settings, and how to give or change consent and preferences
- Analytics and diagnostics: transmitted usage or crash information and how to disable collection
- Purchases: purchase-processing providers, purchase information received by the App or Operator, and handling of payment information
- Authentication and synchronization: account information, stored data, service providers, retention, and deletion
- Other disclosures and outsourced processing: information shared, recipients, purposes, and applicable conditions

{{State that no external services are used only after checking the implementation, including SDKs. Non-personalized advertising may still involve processing information.}}

## 4. Device Permissions

{{If the App uses notifications, photos, the camera, location, or other permissions, explain the purpose of each permission, how information is stored or transmitted, and how to change permission settings. Remove this section if it does not apply.}}

## 5. Information Received Through Support Requests

We use Google Forms for support requests. We use {{information actually received, such as the message, reply email address, and device or app details}} to respond to inquiries, investigate issues, and improve the App.

Submitted information is stored on Google's services. Please provide only necessary information and do not include sensitive information such as passwords or credit card numbers.

We retain support information according to {{retention period or specific criteria for determining it}} and delete information that is no longer needed in accordance with {{deletion procedures}}. To request access to, correction of, or deletion of your information, please contact us using the form below. {{Describe actual identity-verification procedures and the scope of requests that can be handled.}}

{{Check the form settings and explain whether an email address is optional or required, whether email addresses are automatically collected, and whether the App automatically attaches information. If deleting on-device data does not delete previously submitted support information, explain this distinction.}}

For information about how Google handles information, see the [Google Privacy Policy](https://policies.google.com/privacy?hl=en).

## 6. About This Website

This policy is hosted on GitHub Pages. When you visit this page, GitHub may process access information, such as your IP address, in accordance with its policies. For details, see the [GitHub General Privacy Statement](https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement).

{{If the website uses additional analytics, cookies, or similar technologies, describe their handling here.}}

## 7. Changes to This Policy

We review this policy when the App's features, services, or information-handling practices change and publish updates on this page with the revision date. {{Describe how significant changes will be communicated and how consent will be obtained when needed, in accordance with actual procedures.}}

## 8. Contact

For questions about the App or how information is handled, please use the [{{App name}} support form]({{respondent form URL}}).

---

## Pre-publication Checklist

- Replace all {{...}} placeholders and remove drafting notes and inapplicable provisions.
- Confirm consistency with the implementation, SDK settings, and form settings.
- Ensure retention and deletion statements describe procedures that can actually be followed.
- Confirm consistency with store privacy disclosures.
- Preserve existing public URLs and check links and mobile display.
- Confirm deployment before checking in-app and store links.
- Record the reasons for changes and affected apps in the commit or pull request.

Changes to this template do not automatically update individual apps. Select affected apps, review the differences, and apply the changes.
Before each app release, check whether its information-handling practices have changed.

## References

- [Apple App Review Guidelines: Privacy](https://developer.apple.com/app-store/review/guidelines/#privacy)
- [Google Play: User Data](https://support.google.com/googleplay/android-developer/answer/10144311)
