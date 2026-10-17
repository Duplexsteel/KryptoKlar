---
title: Kraken: koble til med API-nøkkel
date: 2026-10-16
summary: Lag en lesenøkkel på Kraken, og en egen nøkkel for Kraken Futures hvis du handler futures. Tar fem minutter.
order: 3
kind: guide
---
Med en API-nøkkel henter Kryptokompis alt fra Kraken av seg selv: handler, innskudd og uttak, staking og Earn, og futures. Nøkkelen kan bare lese - Kryptokompis kan aldri handle eller ta ut penger.

## 1. Lag spot-nøkkelen
1. Logg inn på Kraken (Kraken Pro i nettleseren).
2. Åpne profilmenyen øverst til høyre → **Settings** → **API** (kan hete *Connections & API*).
3. Velg **Create API key** og gi den et navn, for eksempel «Kryptokompis».
4. Huk av **bare** disse tilgangene:
    - **Query Funds**
    - **Query Open Orders & Trades** og **Query Closed Orders & Trades**
    - **Query Ledger Entries**
5. La alt som heter *Deposit*, *Withdraw*, *Create & Modify Orders* og *Cancel/Close Orders* være av.
6. Trykk **Generate key**. Kopier **API key** og **Private key** med en gang - den private nøkkelen vises bare én gang.

## 2. Futures (bare hvis du handler futures)
Kraken Futures har egne nøkler - spot-nøkkelen kan ikke lese futures.

1. Logg inn på Kraken Futures og åpne profilmenyen → **Settings** → **API Keys**.
2. Velg **Read-only** og lag nøkkelen.
3. Kopier begge nøklene.

## 3. Legg dem inn i Kryptokompis
1. **Data og oppsett** → **Børser og lommebøker** → **Legg til børs** → **Kraken**.
2. Lim inn API key og Private key. Futures-nøklene i de to valgfrie feltene.
3. Trykk **Test og lagre**. Kryptokompis sjekker nøkkelen og begynner å synke.

Nøklene lagres i Windows sitt eget nøkkellager på PC-en, ikke i en fil.

## Vanlige feil
- **«Børsen avviste nøkkelen»**: nøkkelen er ikke kopiert helt, eller den er slettet hos Kraken.
- **«Nøkkelen virker, men mangler lesetilgang»**: en av tilgangene over mangler. Rediger nøkkelen hos Kraken og huk den av.
- **Mangler futures?** Legg inn futures-nøkkelen - uten den hentes bare spot.
