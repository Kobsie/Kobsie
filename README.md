Hi, I'm Kobe.

I'm a Laravel developer living in Nagoya, Japan. I build ordering and booking
systems for food businesses back home in the Philippines, the kind that take
payment before anything gets delivered.

## What I've built

**Chicky'Oink Manila** sells lechon belly out of three branches. Before, staff
ran everything through Messenger. Every order got typed again into a to-do app,
GCash screenshots were checked by eye, and someone rebuilt the kitchen's list
by hand every night.

I built them one system to replace all four tools. It went live on 12 August
2026 and I still run it.

Its first 38 days:

- 359 orders
- 290 customers on record
- 52% of orders placed on the website, with nobody typing them in
- 260 payments checked and accepted

## How I build

The code is private, since it's a business's live system. So, briefly:

Nobody types a payment status. Paid, underpaid and refunded are worked out from
the actual payment records, down to the centavo, and every payment event goes
into a log that can't be edited or deleted. Money is the one thing you don't
get to be approximately right about.

Tests run before anything ships. The deploy script reads the diff, runs what
the change actually needs, and refuses to push if something's red.

Migrations only ever add. No dropped columns, and each one gets rehearsed
against a copy of the real database before it runs for real.

## Stack

PHP, Laravel, Tailwind, JavaScript, MariaDB, Pest, GitHub Actions.

I also write embedded C at my day job, mostly CAN bus work on ESP32 and RP2040.

English, Filipino, and Japanese (JLPT N4).

## Get in touch

kobericafrente2001@gmail.com
