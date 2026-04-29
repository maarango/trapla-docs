# TraPla — Privacy Policy

**Effective date:** 2026-04-29
**App:** TraPla (`com.miguelarango.training_app_mobile`)
**Developer:** Miguel Arango

## Summary

TraPla is an on-device training tracker. **It does not run a server.** Your
activities, training plans, profile, wellness readings, and Strava
authentication tokens are stored only on your device. The developer never
receives any of your data. The only data that leaves your phone is what you
explicitly send to a third-party service you connect (e.g., when you log in
to Strava, TraPla talks directly to Strava's servers).

## Data we collect

**None.** TraPla has no backend. We do not operate any server that receives
your data, and we do not have analytics, advertising, or crash reporting
that transmits data off the device.

## Permissions and how they are used

| Permission | When it is used | Why |
|---|---|---|
| `CAMERA` | Only while you have the QR-scan screen open in Settings → Strava | To read a QR code containing your Strava `client_id` / `client_secret` from your computer screen. The camera frame is processed on-device by the Google ML Kit barcode scanner; no images leave your phone. |
| `INTERNET` | When you tap **Connect Strava** or **Sync activities** | To talk to `strava.com` for OAuth and to download your activity history. |
| Health Connect: `READ_EXERCISE`, `READ_HEART_RATE`, `READ_RESTING_HEART_RATE`, `READ_HEART_RATE_VARIABILITY`, `READ_SLEEP`, `READ_WEIGHT`, `READ_BODY_FAT`, `READ_LEAN_BODY_MASS`, `READ_STEPS`, `READ_DISTANCE`, `READ_TOTAL_CALORIES_BURNED`, `READ_ACTIVE_CALORIES_BURNED` | When you tap **Sync now** on the Health Connect screen, or via the daily 6 AM background sync | Read-only access to data that other apps you control (e.g., Garmin Connect, Fitbit, Samsung Health) have written to Android Health Connect. TraPla reads it into its local database to compute fitness curves and the daily Readiness score. The data is never transmitted off the device by TraPla. |

## Third-party services

TraPla integrates with two third-party services, **only when you opt in**:

- **Strava** — When you connect Strava, TraPla loads `https://www.strava.com/`
  inside an embedded WebView for authentication, then communicates directly
  with `https://www.strava.com/api/v3/` to download your activities. Use of
  Strava is governed by Strava's
  [Privacy Policy](https://www.strava.com/legal/privacy).
- **Android Health Connect** — TraPla reads data already in Health Connect.
  Health Connect is a Google-operated component that lets health/fitness apps
  share data on your device. See
  [Google's Privacy Policy](https://policies.google.com/privacy) for how
  Google handles that data.

TraPla itself does not transmit your activity, plan, profile, or wellness
data to any other service.

## Local storage

- A SQLite database on the device holds your activities, training plans,
  user profile, and daily wellness readings.
- `flutter_secure_storage` (an Android EncryptedSharedPreferences wrapper)
  holds your Strava `client_id`, `client_secret`, access token, and refresh
  token if you connected Strava.
- `SharedPreferences` holds small UI state (last-sync timestamp, plan draft,
  language choice).

## Data export and deletion

- **Export backup** in Settings writes a JSON file to a location you choose.
  The file is yours; it is not transmitted to us.
- **Delete all activities** in Settings clears the activity table.
- **Uninstalling TraPla** removes the entire SQLite database, secure storage,
  and preferences. There is no server-side data to delete because no
  server-side data exists.

## Children

TraPla is not directed to children under 13 and does not knowingly collect
data from anyone.

## Changes to this policy

If this policy changes, the "Effective date" at the top will be updated.

## Contact

Email: maarango@gmail.com

GitHub: <https://github.com/maarango/training-app-mobile>
