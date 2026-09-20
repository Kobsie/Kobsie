Hi, I'm Kobe.

I'm a software engineer living in Nagoya, Japan. At work I write embedded C for
automotive systems: CAN bus, ISO-TP, UDS, on ESP32 and RP2040.

Away from that, I love building things with Laravel.

## What I've built

My family runs a lechon business back in Manila. I built its order system and
look after it outside of work hours.

Orders used to live in Messenger threads, payment screenshots, a to-do list, and
a nightly post to the kitchen group. Now they're one record that the staff, the
kitchen and my dad all share. It's been live since August 2026.

## How I build

The code is private, since it's a live business. So, briefly:

Nobody types a payment status. Paid, underpaid and refunded are worked out from
the actual payment records, down to the centavo, and every payment event goes
into a log that can't be edited or deleted. Money is the one thing you don't get
to be approximately right about.

Tests run before anything ships. The deploy script reads the diff, runs what the
change actually needs, and refuses to push if something's red.

Migrations only ever add. No dropped columns, and each one gets rehearsed
against a copy of the real database before it runs for real.

## Stack

PHP, Laravel, Tailwind, JavaScript, MariaDB, Pest, GitHub Actions.

Embedded C at my day job, mostly CAN bus work on ESP32 and RP2040.

English, Filipino, and Japanese (JLPT N4).
