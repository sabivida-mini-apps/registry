<p><img src="https://raw.githubusercontent.com/sabivida-mini-apps/.github/main/assets/social-registry.png" alt="SabiVida partner registry: the public list of genuine SabiVida partner apps." width="100%"></p>

# SabiVida partner registry

The public list of partner apps that SabiVida has reviewed and opened to its members. A mini app runs inside SabiVida, so anyone could claim to be one. This list lets members, partners and journalists check the claim.

## Is this app genuine?

When an app runs in SabiVida, SabiVida's own bar sits above it and shows the app's name, a verified or unverified mark and its **host**. The app can't draw or change that bar.

1. Find the app's name in [`apps.json`](apps.json) or in the table below.
2. The host in SabiVida's bar must be exactly the `origin` listed here, with no extra letters, dots or look-alike characters.
3. An app not on this list isn't a SabiVida partner, whatever it says. SabiVida never asks for your passkey, recovery codes or one-time codes inside an app.

Seen something pretending to be a SabiVida partner? [Report it](../../issues/new?template=report-fake-app.yml).

## Listed apps

No partner app is listed yet. SabiVida is starting with a few invited partners serving Cape Verdean families at home and abroad.

| App | Publisher | Origin | Verified publisher | Listed since |
| --- | --- | --- | --- | --- |

## `apps.json`

```json
{
  "schema": 1,
  "apps": [
    {
      "id": "consular-appointments",
      "name": "Consular appointments",
      "publisher": "Example Lda",
      "origin": "https://apps.example.org",
      "category": "paperwork",
      "verified": true,
      "listedSince": "2026-11-02"
    }
  ]
}
```

- `id` is the app's address in SabiVida: `https://sabivida.com/apps/<id>`.
- `category` is one of `paperwork`, `money`, `travel`, `community`, `work`, `learning`, `health`.
- `verified` means SabiVida has checked the publisher's legal identity.

The SabiVida team updates this file when an app is listed, suspended or removed, or changes owner or origin (which sends it back to review). Each change is a commit, so the history shows when it happened.

## Become a partner

Partners are invited and reviewed. To ask, open a [partner application](../../issues/new?template=apply.yml) with your organisation's name and the service you have in mind, and nothing confidential. The team replies with a private channel.

To build one, see the [partner kit](https://github.com/sabivida-mini-apps/partner-kit) and start from [first-app](https://github.com/sabivida-mini-apps/first-app).
