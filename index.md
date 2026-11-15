# SMS Dove Privacy Policy

Last updated: November 15, 2026

SMS Dove is an Android app by TonyAppsLab that forwards newly received SMS messages matching your rules to Google Sheets in the Google account you choose. This policy explains the app's data handling and this policy website.

## 1. SMS messages and forwarding

With your SMS permission, Android delivers newly received SMS messages to SMS Dove. The app processes the sender, message text and reception time on your device to apply your rules. It does not scan your historical SMS inbox or send SMS messages.

When forwarding is enabled, matching messages are saved in a local queue. The full message text, sender, reception time, matching rule names and an app-generated forwarding identifier are sent over HTTPS to your configured Google Sheets destinations. Forwarding can run in the background while the app is closed, subject to Android's execution limits.

Choose rules and destinations carefully: messages can include verification codes, financial information or other sensitive content. Anyone with access to a destination spreadsheet may be able to read forwarded messages. TonyAppsLab does not operate a server that receives or stores your SMS messages.

## 2. Google account and spreadsheet access

You authorize a Google account through Google Play services. SMS Dove uses your Google account identifier and verified email address to identify the account, show the connection and keep each account's rules and queued work separate. The app does not receive your Google password. Authorization tokens are handled through Google Play services and used for Google API requests; SMS Dove does not save access or refresh tokens in its own databases.

The app requests basic account identification and email access, plus Google Drive's per-file access scope (drive.file). This enables it to create and manage the spreadsheets and tabs used by the app and check prior writes before retrying. It does not request unrestricted access to your entire Drive. Access applies to the authorized file, rather than only an individual spreadsheet tab.

Google API data is used to operate the account and spreadsheet features you request. We do not use that data for advertising, sell it or use it to train generalized AI models. Our use and transfer of Google API data follows the [Google API Services User Data Policy](https://developers.google.com/terms/api-services-user-data-policy), including its Limited Use requirements. Google's own processing is described in the [Google Privacy Policy](https://policies.google.com/privacy).

## 3. Other data stored on your device

SMS Dove stores your settings, Google account identifier and email address, forwarding rules, destination identifiers and names, pending messages, delivery results and operational error records on your device. Rule tests process the sample sender and message you enter locally and do not write them to Google Sheets.

The separate Dove balance records the forwarding expiry time, observed device time, reward identifiers, reward timestamps and reminder status. Pending earned rewards may be saved locally until they are credited. This balance does not contain SMS text, sender numbers, Google identity or an advertising identifier. Reward records remain until you clear the app's data; the history screen displays only the most recent 20 entries.

## 4. Permissions

- **Receive SMS:** allows Android to deliver incoming SMS for local rule matching and forwarding. Turning off forwarding prevents new messages from entering the queue, but does not revoke the Android permission. Revoke the SMS permission in Android settings to stop delivery to the app.
- **Internet and network state:** enable Google authorization, spreadsheet transfers, connection checks and advertising services when available.
- **Notifications:** optional permission for operational problems and Dove time reminders. SMS Dove's notification messages do not include the SMS text or sender.
- **Advertising identifiers:** advertising SDK dependencies can use advertising and app identifiers when advertising is enabled, as described below. This is separate from SMS permission.

The app does not request contacts, camera, microphone, precise-location or SMS-sending permissions.

## 5. Rewarded advertising and Feed

Feed is designed to let you choose to watch a rewarded ad to add Dove forwarding time. The integrated mediation service is Unity LevelPlay, with Unity Ads and Liftoff Monetize (formerly Vungle) as the configured ad sources. We do not provide SMS content, sender numbers, Google account data, rules or spreadsheet contents to these advertising services.

Advertising is optional. Before initializing the advertising service, SMS Dove explains the processing and asks you to choose “Use non-personalized ads” or “Do not use ads”. Closing the explanation without choosing does not authorize ad requests. The app requests contextual (non-personalized) ads only and sends the providers signals declining GDPR personalization consent and opting out of sale or sharing for targeted advertising. Non-personalized ads still involve data processing.

When advertising is enabled, providers may process advertising or app/device identifiers, IP address and approximate location inferred from it, device and operating-system details, language, network information, ad impressions and clicks, reward events, diagnostics and privacy choices. These support contextual ad delivery, measurement and fraud prevention. SMS Dove does not offer personalized ads. The app does not request precise-location permission for ads.

Provider practices and choices are explained in the [Unity Game Player and App User Privacy Policy](https://unity.com/legal/game-player-and-app-user-privacy-policy) and [Liftoff Privacy Policy](https://liftoff.ai/privacy-policy/). Providers apply their own retention periods; the app's 30-day delivery-summary rule does not apply to their records. Provider-wide policies may describe additional advertising uses; SMS Dove sends the opt-out signals described above rather than authorizing personalized advertising.

The app manages this contextual-ad choice itself; it does not use AdMob or Google's User Messaging Platform. Settings → Advertising data options (設定 → 廣告資料選項) is always available. Choosing “Do not use ads” stops the app from loading or showing new ads and discards its current loaded-ad reference. It cannot recall requests already sent, erase provider records or undo earlier processing. Your choice, disclosure version and update time are stored locally until app storage is cleared or the app is uninstalled; a changed disclosure version requires a new choice. This is an app-managed choice, not an IAB TCF consent-management platform. You can also use Android's advertising-privacy controls where available and the providers' privacy-request options.

Choosing not to watch ads does not delete your existing messages or rules. If Dove time expires, outward forwarding and retries pause. When the main forwarding switch remains on, newly matching SMS messages can still enter the local queue and be sent after time is replenished. Turning the main switch off stops new intake and pauses existing work.

## 6. Retention and security

- **Queued SMS and sender data:** retained locally until every destination for that message has succeeded or been manually cancelled. There is no automatic time limit for unfinished work. Disabling a rule, disconnecting Google, going offline or running out of Dove time does not delete queued data.
- **Completed delivery summaries:** retained for 30 days after completion, then removed during app cleanup. They contain timing, rule, destination and result information, but not the cleared SMS text or sender.
- **Settings, rules, destinations and account records:** kept locally until you remove the relevant information where supported, clear app storage or uninstall. Disconnecting Google is an authorization action, not a full local-data deletion.
- **Dove and reward records:** kept locally until app storage is cleared or the app is uninstalled; temporary earned-reward receipts are removed after successful local crediting.
- **Google Sheets copies:** remain under your Google account and spreadsheet sharing settings until you delete them there. Local cleanup does not delete remote copies.

The app uses Android's app-private storage and HTTPS for Google API requests. It does not add a separate application-level encryption layer to its local databases. App data is excluded from Android cloud-backup and device-transfer rules. Device manufacturers and Android versions can differ, so do not treat these settings as a guarantee against all copies or forensic recovery. No storage or transmission system is completely secure.

## 7. Your controls and deletion

You can pause forwarding, disable or edit rules, revoke Android permissions, cancel pending destination work and disconnect the Google account. A request already sent to Google may finish even after you pause or cancel; cancellation cannot recall a remote write.

Clear SMS Dove's storage in Android settings, or uninstall it, to remove its local settings, message queue, account records, summaries and Dove balance. Remove its access separately through your [Google account's third-party connections](https://myaccount.google.com/connections). Delete forwarded rows or spreadsheets in Google Sheets or Drive and review any sharing or exported copies separately. These actions do not delete messages from your phone's SMS app or delete your Google account.

SMS Dove does not create a separate TonyAppsLab-hosted user account. Detailed steps, including how to contact us about data we hold directly, are on the [SMS Dove Data Deletion page](sms-dove-delete-data/).

## 8. Support communications

If you email TonyAppsLab, we receive your email address and the information you choose to send. We use it to answer your request and retain it only as needed for support and applicable legal obligations. Do not send SMS contents, verification codes, passwords or Google authorization tokens. We cannot inspect your device's private app storage or remove rows from your Google Sheets on your behalf.

## 9. International processing and privacy rights

Google and advertising providers may process data in countries other than yours under their own policies. Depending on where you live, you may have rights to access, correct or delete personal data, restrict or object to processing, withdraw consent or opt out of certain advertising uses, and complain to a privacy regulator. Contact us about information TonyAppsLab holds directly; use the relevant provider's privacy controls for its records. We may need proportionate information to verify a request, but will not ask for your password or SMS contents.

## 10. Children

SMS Dove is not directed to children under 13. We do not knowingly seek personal information from children under 13 through our support channels. If you believe a child has provided us personal information, contact us so we can address it. Any higher age or consent requirements in your region still apply.

## 11. This policy website

This static website is hosted on GitHub Pages. We do not add advertising, analytics scripts, tracking pixels, cookies, external fonts or data-entry forms to these pages. GitHub may process IP addresses and ordinary request information to deliver and secure the website under the [GitHub Privacy Statement](https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement). Email links open your email application; sending an email is a separate action.

## 12. Changes and contact

We will update this page and its last-updated date when our practices change. Material changes will be communicated in the app where appropriate before the changed processing begins.

Developer: **TonyAppsLab**. For privacy questions or requests, email [tonyappslab@gmail.com](mailto:tonyappslab@gmail.com) with the subject “SMS Dove privacy”.
