# grades-of-climbing-legal

Public legal documents of the Grades of Climbing Converter app (`com.etcho.grades_of_climbing_converter`), published with GitHub Pages at https://etcho.github.io/grades-of-climbing-legal/. Same structure as `mimica-legal`, without terms of use (the app has no account or cloud) and without purchase.

| Page | Source |
|---|---|
| https://etcho.github.io/grades-of-climbing-legal/privacy-policy/ | `privacy-policy/index.md` (English, prevails) |
| https://etcho.github.io/grades-of-climbing-legal/pt-BR/privacy-policy/ | `pt-BR/privacy-policy/index.md` |

The app opens these addresses from `privacyPolicyUrl` in `lib/core/platform/external_actions.dart` (menu ⋮ > Privacy policy): pt opens pt-BR, every other language opens English. The Play Console uses the English address.

## Changing the policy

1. Edit the English page: update **Version** and **Effective date** and add a line to **Version history**.
2. Update the translation in the same commit, so a language never shows an outdated text as current.
3. Menu names quoted in the texts must match the app's strings (`lib/core/l10n/app_<lang>.arb` in the app repository).
4. If the app starts collecting something new (a new SDK, an account, a purchase, a new event with user values), the policy and the Play Console "Data safety" form change in the same release.
