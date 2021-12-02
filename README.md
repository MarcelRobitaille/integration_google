# Google integration in Nextcloud

**This is a fork!!** Please see [the upstream](https://github.com/nextcloud/integration_google) or [the issue that prompted this fork](https://github.com/nextcloud/integration_google/issues/77).

This fork tries to fix two problems I had with the Google integration:
1. It only syncs stuff when you click the import button. It doesn't keep the imported stuff up to date
1. It only adds new data, it doesn't delete outdated data. Anytime someone on my team would reschedule something in our Google Calendar, I would have it multiple times in my Nextcloud calendar.

I have fixed both of these, at least for the Calendar (the only integration I use).

**USE AT YOUR OWN RISK!!** This is my first Nextcloud app and it is definitely not production-ready. For instance, I blindly add a new background job without checking if it already exists. I don't do logging correctly.

🇬 Google integration allows you to automatically import your Google calendars, contacts, photos and files into Nextcloud.

## 🔧 Configuration

### User settings

The account configuration and data migration happens in the "Data migration" user settings section.

### Admin settings

There also is a "Connected accounts" **admin** settings section that you must visit to configure a Google OAuth app to allow your Nextcloud users to authenticate to Google.
