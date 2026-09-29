# Awesome WhatsApp to Telegram Bridges

A curated, honest list of ways to send messages between WhatsApp and Telegram, in both directions, from quick manual tricks to fully managed services. There is no native way to forward between the two apps, so this guide compares every realistic option, including open-source projects and paid competitors. Maintained by the team behind [wa2tg.app](https://wa2tg.app); we list our own service and every alternative we know of, with honest pros and cons. Pull requests welcome.

## The problem

WhatsApp and Telegram do not talk to each other. There is no "forward to the other app" button. To move messages from Telegram to WhatsApp (or WhatsApp to Telegram) automatically, with photos, videos and voice notes, you need a bridge. The realistic options, with trade-offs, are below.

## Manual methods (free)

Copy / paste and Share. Fine for one or two messages; free; loses nothing, but does not scale.

Export chat. WhatsApp and Telegram chat exports drop most media and formatting; a one-off dump, not a live sync.

## Managed services (run for you, no server)

[wa2tg.app](https://wa2tg.app). Managed WhatsApp to Telegram bridge. Mirrors a WhatsApp group and a Telegram group both ways (text and media), and clones channels one way. No code, no QR, no server; about a 2-minute setup, running on its own number rather than yours. Free plan, then 20 USD one-time for 30 days. Guides: [Telegram to WhatsApp](https://wa2tg.app/send-telegram-messages-to-whatsapp), [WhatsApp to Telegram](https://wa2tg.app/how-to/send-whatsapp-messages-to-telegram), [clone a Telegram channel](https://wa2tg.app/how-to/clone-telegram-channel-to-whatsapp), [is it safe](https://wa2tg.app/security).

## No-code automation (you build the flow)

Zapier / Make / n8n. Connect triggers and actions, but you still need the WhatsApp Business API on the WhatsApp side, and you build and maintain the flow. Good for custom logic; hours to set up.

## Official APIs (build it yourself, per-message pricing)

WhatsApp Business API (Meta Cloud API). Official and powerful, but weeks of setup, approval and per-message fees.

Twilio for WhatsApp. Hosted access to the API; per-message fees; you write the bridge.

WHAPI.cloud and Wassenger. Hosted unofficial WhatsApp APIs; flat per-number fee; you still build the bridge.

## Open source (self-hosted)

Free, but you host and maintain a server and link a WhatsApp session on your own number.

[matterbridge](https://github.com/42wim/matterbridge). Bridges many chat platforms, including Telegram and WhatsApp via a connector; flexible and self-hosted.

[mautrix-whatsapp](https://github.com/mautrix/whatsapp) and [mautrix-telegram](https://github.com/mautrix/telegram). Matrix bridges; powerful, but you run a Matrix homeserver.

## Unified inbox apps

Not a bridge between two separate groups; these put multiple chat apps into one client.

[Beeper](https://www.beeper.com/). One inbox for many messengers. Great for reading everything in one place, but it does not mirror a Telegram group into a separate WhatsApp group.

## How to choose

One or two messages: copy and paste. A group or channel, both ways, with media, set up in minutes and nothing to maintain: a managed service such as [wa2tg.app](https://wa2tg.app). Custom automation with a developer on hand: the WhatsApp Business API plus Zapier, Make or n8n. Full control and comfortable running a server: matterbridge or the mautrix bridges.

---

Not affiliated with Meta, WhatsApp, or Telegram. Links to other projects and services are provided for comparison; do your own due diligence. Corrections and additions are welcome via pull request.
