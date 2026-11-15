# SMS Dove Data Deletion

Last updated: November 15, 2026

SMS Dove is provided by TonyAppsLab. Its message queue and settings are stored on your Android device; forwarded copies are stored in the Google Sheets destinations you chose. Follow the steps for each location below.

## 1. Stop new forwarding

Turn off the main forwarding switch on SMS Dove's Home screen. Existing queued work pauses and new messages do not enter the queue. For Android to stop delivering new SMS to the app, also revoke SMS permission in Android settings.

A network request already sent may still complete. Stopping forwarding does not undo earlier writes or delete queued messages.

## 2. Cancel individual pending messages

Open Activity (活動), select a pending destination item and choose the cancellation action. Cancel each outstanding destination associated with the message. The local full message and sender are cleared once all destinations for that message have either succeeded or been cancelled. Cancelling one destination does not cancel other destinations or remove their Google Sheets rows.

A completed or cancelled result summary can remain locally for 30 days. To remove all local summaries immediately, clear app storage as described next.

## 3. Delete all SMS Dove data on your device

In Android settings, open Apps → SMS Dove → Storage (or Storage & cache) → Clear storage / Clear data. Labels vary by phone. Alternatively, uninstall SMS Dove.

This removes the app's local rules, destinations, account records, pending SMS, result summaries, Dove balance and reward records. Pending work cannot be recovered through SMS Dove after local data is cleared. The app excludes its data from Android backup and device-transfer rules, but cannot erase copies created outside its control or guarantee physical erasure from flash storage.

Clearing storage or uninstalling does not delete your phone's original SMS messages, your Google account, Google Sheets data or data already held by advertising providers.

## 4. Revoke Google access

In SMS Dove's Settings (設定), choose “Disconnect and revoke access” (中斷連接並撤銷授權) and confirm. You can also remove SMS Dove from your [Google account's third-party connections](https://myaccount.google.com/connections).

If you plan to clear storage or uninstall, revoke access first or use Google's page afterward. Revoking access stops the app's authorized Google operations; it does not delete spreadsheets or clear all local records. Reconnecting the same account may allow remaining queued work to resume.

## 5. Delete forwarded Google Sheets copies

Open each destination spreadsheet in Google Sheets and delete the relevant rows, or delete the spreadsheet in Google Drive. Review Drive's Trash and permanently delete the file there if that is your intention. For a shared spreadsheet, contact its owner if you lack permission.

Other people may have exported or copied data. Sharing settings, version history and any retained copies are controlled by Google and the relevant account or file owner. SMS Dove cannot recall them. Delete original phone messages separately in your SMS app if desired.

## 6. Advertising-provider records

The current prerelease does not initialize or request ads while privacy messaging setup is incomplete. If you use a version with advertising enabled, clearing app storage does not delete records already held by its providers.

Use the privacy-request and advertising-choice instructions in the [Unity Game Player and App User Privacy Policy](https://unity.com/legal/game-player-and-app-user-privacy-policy) and [Liftoff Privacy Policy](https://liftoff.ai/privacy-policy/). Those providers control verification, retention and deletion of their own records. Android's advertising-privacy controls may provide additional choices, depending on your device. Do not send advertising identifiers or other sensitive details to TonyAppsLab unless needed for a specific, explained support request.

## 7. Request deletion of information held by TonyAppsLab

Email [tonyappslab@gmail.com](mailto:tonyappslab@gmail.com?subject=SMS%20Dove%20data%20deletion) with the subject “SMS Dove data deletion”. Describe the information you want deleted, such as a support conversation, and preferably use the email address associated with it. Do not include SMS contents, verification codes, passwords or authorization tokens.

We will assess requests about information we hold directly and explain any applicable legal retention requirement. We cannot access your local queue, delete your Google account or delete Google Sheets or advertising-provider records for you. SMS Dove has no separate TonyAppsLab-hosted account to close.

[Read the SMS Dove Privacy Policy](../).
