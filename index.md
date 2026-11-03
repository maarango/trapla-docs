# TraPla — Privacy Policy

**Effective date:** 2026-11-02
**App:** TraPla for Android (`com.miguelarango.training_app_mobile`) and the
TraPla web app at <https://maarango.github.io/trapla-docs/app/>
**Developer:** Miguel Arango

## Summary

- On Android, TraPla works without an account, and your data stays on your
  phone unless you turn on one of the features below.
- If you create a **TraPla account**, your activities, training plans and
  profile are stored on a server so they sync between your phone and the web
  app. Sleep and other daily wellness readings, and workouts that came only
  from Health Connect, are never uploaded to it.
- If you use the **AI coach**, the data needed for your request is sent to
  the AI provider (Anthropic or Google) to produce an answer.
- If you connect **Garmin Connect**, TraPla downloads your data from it.
- TraPla does not connect to Strava. See [Strava](#3-strava) below.
- TraPla has no advertising, no analytics and no crash reporting. Your data
  is not sold and is not used for advertising.

## What leaves your device, and when

### 1. TraPla account and sync (optional on Android, required on the web)

When you create an account or sign in, TraPla uses
[Supabase](https://supabase.com/privacy) to run the account and store synced
data. The server is hosted in the European Union.

What is stored on the server:

- **Your account:** email address, a securely hashed password (TraPla never
  sees or stores it in readable form), an account ID, and sign-in times. If
  you sign in with Google, Google shares your email address and name with
  the account service.
- **Activities:** date, sport, distance, duration, calories, average and
  maximum heart rate, pace, power, elevation gain, and treadmill incline.
  This includes activities from Garmin Connect, and activities you
  added or imported yourself. No GPS tracks or locations are stored.
- **Training plans** you create, import or edit.
- **Your profile:** sex, date of birth, resting and maximum heart rate,
  weight, FTP, and heart-rate zones, as you entered them.

What is **not** uploaded: daily wellness readings (sleep, HRV, resting heart
rate, weight, stress, Body Battery, steps), workouts known only through
Health Connect, and your Garmin or AI keys and tokens. These stay on
the phone.

A phone holds one person's data, so it can only be linked to one account.

### 2. AI coach (optional)

AI features run only when you use them, for example when you build or adjust
a plan, ask for coach insights, chat with the coach, import another app's
plan, or ask for target paces on a race route. TraPla then sends the request
directly to the AI provider you chose:

- **Anthropic (Claude)** — [Privacy Policy](https://www.anthropic.com/legal/privacy)
- **Google (Gemini)** — [Privacy Policy](https://policies.google.com/privacy)

Depending on the request, it can include your plan settings and goal, your
profile, a summary of recent activities, recent daily wellness readings
(HRV, resting heart rate, sleep, stress, Body Battery, weight), your chat
messages, the plan file you are importing, and a race route's per-kilometre
elevation and grade (not its coordinates). **This can include data that
TraPla read from Health Connect**, and it is sent only to answer the request
you made.

The providers process this data under their API terms, which do not allow
them to use it to train their models. They may keep it for a limited time
for abuse and safety monitoring. TraPla does not store your requests on any
server of its own.

**Voice input:** the microphone button in the coach chat uses your phone's
built-in speech recognition. Depending on your phone's settings, the speech
service (usually Google) may process your voice to turn it into text. TraPla
receives only the text and does not record or keep audio.

### 3. Strava

TraPla no longer connects to Strava, and it has deleted the Strava data it
held. Version 1.7.1 and later remove TraPla's Strava connection, revoke
TraPla's access on Strava when they can, and delete every activity that came
from Strava from the phone. Strava activities synced to a TraPla account
are deleted from the server too. If the Strava app writes your workouts to Health Connect,
TraPla reads them there like any other Health Connect data.

### 4. Garmin Connect (optional)

When you connect Garmin, you sign in on Garmin's own page. TraPla never sees
your Garmin password. It downloads your activities and daily wellness data
from Garmin Connect and keeps the Garmin login tokens on your phone, in
encrypted storage. See Garmin's
[Privacy Policy](https://www.garmin.com/privacy/connect/).

### 5. Web hosting

The web app is served by GitHub Pages, which may log technical details such
as your IP address. See
[GitHub's Privacy Statement](https://docs.github.com/site-policy/privacy-policies/github-general-privacy-statement).

## Health Connect

TraPla reads data from Android Health Connect only after you grant
permission, and only to show your activities, fitness curves and daily
Readiness score, and to give the AI coach the context for your requests. It
reads only and never writes to Health Connect.

| Permission | What TraPla uses it for |
|---|---|
| Exercise, distance, steps, calories (active and total) | Your activity history and training load |
| Heart rate, resting heart rate, heart rate variability | Training load, heart-rate zones and Readiness |
| Sleep | Readiness and recovery |
| Weight, body fat, lean body mass | Your wellness history and the AI coach's context |

Data read from Health Connect:

- is stored in TraPla's database on your phone;
- is **not** uploaded to the TraPla account server;
- is sent to an AI provider only when you use an AI feature, as described
  above;
- is never sold, never used for advertising, and never shared with anyone
  else.

TraPla's use of information received from Health Connect is meant to follow
Google Play's
[health permissions policy](https://support.google.com/googleplay/android-developer/answer/12991134).

## Other permissions

| Permission | Why |
|---|---|
| Internet | To sync your account and to talk to Garmin and the AI providers when you use them |
| Microphone (`RECORD_AUDIO`) | Only while you use voice input in the coach chat, as described above |

## Storage on your device

- On Android, a database on the phone holds your activities, plans, profile
  and daily wellness readings. Encrypted storage holds your Garmin
  tokens, any AI keys you entered, and your account session.
- In the web app, the browser stores your synced data and account session.
  When a different account signs in, the browser's copy is cleared. If you
  use a shared computer, use **Sign out** when you are done.

## Your choices: export and deletion

- **Export backup** (Android) writes a JSON file to a place you choose. It is
  not sent to us.
- **Delete all activities** (Android) clears your activities on the phone.
- **Disconnect Garmin** removes its tokens from the phone.
- **Delete account:** sign in, then open **Settings → TraPla account →
  Delete account**, on the phone or in the web app at
  <https://maarango.github.io/trapla-docs/app/>. This deletes your account
  and every record stored for it on the server immediately. Data on your
  phone stays there until you delete it or uninstall the app. If you can no
  longer sign in, email the address below from the account's email address
  and your account will be deleted within 30 days.
- **Uninstalling** the Android app removes everything stored on the phone.

## Retention

Synced data is kept for as long as your account exists, and is deleted when
you delete the account. TraPla keeps no backups of it on other servers.

## Security

All connections use HTTPS. Each account can read and change only its own
records on the server.

## Children

TraPla is not directed to children under 13, and accounts are not intended
for them.

## Changes to this policy

If this policy changes, the effective date at the top will be updated.

## Contact

Email: maarango@gmail.com
