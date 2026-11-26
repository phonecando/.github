# PhoneCanDo

**AI that can use your phone.** PhoneCanDo runs AI coding agents on your
Android phone, one or a whole crew. They work in a full terminal, and, once
you let them, read the screen and use your apps. No PC, no cloud relay.

**[Get it at phonecando.app →](https://phonecando.app)**

## Our repos

| Repo | What's inside |
| --- | --- |
| [**phone-control**](https://github.com/phonecando/phone-control) | The open part: the code that lets an agent see and touch your phone, and every gate it has to pass on the way. Read it, check it. |
| [**distribution**](https://github.com/phonecando/distribution) | The app's releases: APKs, update manifest, GPL sources, and the workflow that builds, signs and attests them. |
| [**feedback**](https://github.com/phonecando/feedback) | Bugs, agent requests, ideas and questions. No code, all ears. |
| [**.github**](https://github.com/phonecando/.github) | This page, and our defaults for the rest. |

## Closed app, open hands

The app is closed source. The part that can touch your phone isn't: every
step from an agent's call to a tap on your screen is in
[phone-control](https://github.com/phonecando/phone-control), and so is every
gate on the way: the control lock only your fingerprint arms, the apps you
allow, the hand-over, one agent on the screen at a time.

Each release is built from a phone-control commit on its `main` and attested,
so you can check that the APK you got came from our workflow:

```sh
gh attestation verify phonecando-<version>-full-arm64.apk --repo phonecando/distribution
```

## Say hi

Bugs and wishes go to [feedback](https://github.com/phonecando/feedback).
Security holes go privately: see [`SECURITY.md`](https://github.com/phonecando/.github/blob/main/SECURITY.md).
Anything else: hi@phonecando.app.
