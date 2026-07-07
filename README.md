# Scanveil Legal Pages

This repository hosts the public legal, privacy, account deletion, license, and app information pages for **Scanveil** using GitHub Pages.

Scanveil is a QR code scanning and QR information management app that allows users to scan, preview, save, organize, and optionally back up or synchronize QR code information.

---

## Public Pages

Once GitHub Pages is enabled, the following pages will be available publicly:

| Page                                 | File                             | Public URL                                                                        |
| ------------------------------------ | -------------------------------- | --------------------------------------------------------------------------------- |
| Legal Home                           | `docs/index.html`                | `https://your-github-username.github.io/scanveil-legal/`                          |
| Privacy Policy                       | `docs/privacy-policy.html`       | `https://your-github-username.github.io/scanveil-legal/privacy-policy.html`       |
| Terms & Conditions                   | `docs/terms-and-conditions.html` | `https://your-github-username.github.io/scanveil-legal/terms-and-conditions.html` |
| Account Deletion and Data Collection | `docs/account-deletion.html`     | `https://your-github-username.github.io/scanveil-legal/account-deletion.html`     |
| Legal and Licenses                   | `docs/legal-and-licenses.html`   | `https://your-github-username.github.io/scanveil-legal/legal-and-licenses.html`   |
| About Scanveil                       | `docs/about.html`                | `https://your-github-username.github.io/scanveil-legal/about.html`                |

Replace `your-github-username` with the actual GitHub username that owns this repository.

---

## Repository Structure

```text
scanveil-legal/
├── README.md
└── docs/
    ├── index.html
    ├── privacy-policy.html
    ├── terms-and-conditions.html
    ├── account-deletion.html
    ├── legal-and-licenses.html
    ├── about.html
    └── assets/
        └── styles.css
```

---

## Purpose of This Repository

This repository is used to host public pages required for:

* Google Play Console privacy policy submission
* Google Play Data Safety disclosures
* Google Play account deletion URL
* App Store Connect privacy policy URL
* In-app legal links
* In-app account deletion and data collection information
* Open-source license and legal notices
* About page for Scanveil

---

## GitHub Pages Setup

To enable GitHub Pages:

1. Open this repository on GitHub.
2. Go to **Settings**.
3. Open **Pages** from the sidebar.
4. Under **Build and deployment**, select:

```text
Deploy from a branch
```

5. Select branch:

```text
main
```

6. Select folder:

```text
/docs
```

7. Click **Save**.

After deployment, GitHub will provide the public site URL.

---

## Recommended App Links

Use these links inside the Scanveil app:

```dart
class AppLegalLinks {
  static const baseUrl =
      'https://your-github-username.github.io/scanveil-legal';

  static const privacyPolicy = '$baseUrl/privacy-policy.html';
  static const termsAndConditions = '$baseUrl/terms-and-conditions.html';
  static const accountDeletion = '$baseUrl/account-deletion.html';
  static const legalAndLicenses = '$baseUrl/legal-and-licenses.html';
  static const about = '$baseUrl/about.html';
}
```

---

## Google Play Console Links

Use the following pages in Google Play Console:

| Google Play Console Section   | Recommended Page             |
| ----------------------------- | ---------------------------- |
| Privacy Policy                | `privacy-policy.html`        |
| Data Safety Form Reference    | `privacy-policy.html`        |
| Account Deletion URL          | `account-deletion.html`      |
| Developer Website, optional   | `index.html` or `about.html` |
| Support Information, optional | `about.html`                 |

---

## App Store Connect Links

Use the following pages in App Store Connect:

| App Store Connect Field             | Recommended Page            |
| ----------------------------------- | --------------------------- |
| Privacy Policy URL                  | `privacy-policy.html`       |
| User Privacy Choices URL, if needed | `account-deletion.html`     |
| Support URL                         | `about.html`                |
| Marketing URL, optional             | `index.html` or app website |

---

## Updating Content

To update any legal page:

1. Open the file inside the `docs/` folder.
2. Edit the required content.
3. Update the **Last updated** date on the page.
4. Commit the changes to the `main` branch.
5. GitHub Pages will automatically redeploy the updated page.

The public URL will remain the same as long as the filename does not change.

Example:

```text
docs/privacy-policy.html
```

will continue to be available at:

```text
https://your-github-username.github.io/scanveil-legal/privacy-policy.html
```

---

## Recommended Commit Messages

Use clear commit messages when updating legal pages:

```text
Add privacy policy page
Add terms and conditions page
Add account deletion page
Update privacy policy for Firebase Analytics
Update account deletion instructions
Update support email
Update legal links
```

---

## Important Notes

Before publishing these links in Google Play Console, App Store Connect, or the Scanveil app, make sure:

* All placeholder emails are replaced with the real support or privacy email.
* The developer or business name is correct.
* The country is correct.
* The Privacy Policy matches the actual app behavior.
* The Data Safety form matches the Privacy Policy.
* The Account Deletion page explains how users can delete their account and associated data.
* The app includes an in-app path for account deletion if account creation is supported.
* Firebase services used by Scanveil are accurately disclosed.
* Cloud backup and synchronization behavior is accurately described.
* QR code content storage, history, favourites, backup, and sync behavior are accurately described.
* The app does not claim end-to-end encryption unless it is actually implemented and verified.

---

## Scanveil Data Areas to Review

When updating the legal pages, review whether Scanveil currently uses or stores:

* Email address
* Display name
* Firebase user ID
* QR code content
* Scan history
* Favourite QR records
* App preferences
* Backup and restore data
* Cloud synchronization metadata
* Crash reports
* Analytics events
* Device or installation identifiers
* Selected images used for QR scanning
* Exported text files or downloaded files

---

## License

This repository contains legal and informational content for Scanveil.

Unless otherwise stated, the content in this repository is maintained for the Scanveil app and should not be reused as legal advice.

---

## Contact

For questions, support, privacy requests, or account deletion requests:

```text
Email: thevishalswami@gmail.com
App: Scanveil
Country: India
```
