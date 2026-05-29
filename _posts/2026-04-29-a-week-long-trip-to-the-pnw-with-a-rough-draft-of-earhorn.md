---
layout: post
title: "A Week-Long Trip to the PNW with a Rough Draft of EarHorn"
description: "I flew to the Pacific Northwest with a baby, no hardware monitor, and a buggy early build of EarHorn. Here's what travel taught me about the bugs you can't find at home — and why a baby monitor that fits in a pocket changed how I see the whole thing."
date: 2026-04-29
---

My wife and I flew up to the Pacific Northwest this spring to visit family — a full week away. And when you're flying with a baby, space isn't a luxury. It's the whole game. Every cubic inch of the carry-on is spoken for before you've even zipped it: diapers, the white noise machine, half a dozen stuffed animals, the bag of snacks that buys you twenty minutes of peace at the gate.

So when I looked at our hardware baby monitor — the camera, the parent unit, the tangle of chargers — I made a call. It wasn't coming. There was no room, and I wasn't about to check a bag over a baby monitor.

Instead I brought a spare phone and a charging cable. That's the entire monitor. It went in a side pocket and I forgot it was there until we needed it. I'd been building the app for months, but this was the first real test with no backup waiting at home.

## The bugs you only find on the road

Here's the honest part: it worked, but it wasn't perfect.

At home, on my own WiFi, in my own nursery, everything had always just worked. A week in an unfamiliar Airbnb is a different story — new router, new network quirks, a different room layout, a phone propped in a spot it had never sat before. Travel is exactly the situation that drags out the bugs you didn't know you had.

This one was sneaky. The Airbnb WiFi would blink out for about half a second at a time. Not enough for a human to notice — you'd never catch it loading a webpage, and a movie would buffer right through a hiccup that short. But EarHorn, at the time, treated every one of those blips as a full disconnect and started the pairing handshake over from scratch. The result was a few seconds of dead air every time the router so much as flickered.

And a few seconds of dead air on a baby monitor are exactly the few seconds you don't want to miss.

The fix was teaching it to ride out a brief gap — to reconnect quietly in the background instead of panicking and rebuilding the whole connection from the ground up. Simple in hindsight. Invisible until you're standing in someone else's guest room at night, depending on the thing to actually work.

There's no test suite like genuinely needing the app, far from home, with a sleeping kid down the hall.

## Late nights and a very quiet door

So the routine set in. Once the kiddo went down, I'd pull the laptop out at the kitchen table and dig in — find what was going wrong, write the fix, build a fresh version onto the phone.

Then came the tricky part. To actually test a fix, I had to swap the running app on the phone in the baby's room. Which meant creeping in, re-pairing the two phones in the dark, and creeping back out without waking anyone.

I got very good at opening that door slowly.

Every morning the app was a little better than it had been the night before.

## Hard mode

One day we decided to walk onto a ferry to visit yet more family across the water. No car this time — just two backpacks and a stroller, which is about as lean as travel with a baby gets.

<figure class="post-image">
    <img src="{{ '/assets/images/pnw-ferry-deck.jpeg' | relative_url }}" alt="The open upper deck of a ferry with rows of empty orange seats, snow-capped mountains and a small waterfront town across the water under a blue sky" loading="lazy">
    <figcaption>The view from the ferry deck — the whole nursery setup fit in a backpack.</figcaption>
</figure>

A hardware monitor would have been the first thing cut from that list. There's simply no room for one when you're carrying everything on your back.

The phone came along without a second thought. It weighs nothing, it takes up no space, and that night it set up in the spare bedroom in under a minute — exactly like it had back at the Airbnb. If the carry-on was hard mode, the ferry was hard mode with a hand tied behind my back, and the phone fit right in.

That was the leg of the trip where I stopped thinking of phone-as-monitor as a compromise and started seeing it as the whole point.

## What came home with me

Two things made the trip back.

The first was a noticeably more reliable app. Travel bugs are the worst kind — they make everything shakier everywhere — so fixing this one didn't just help me in one Airbnb. It helps every family who'll ever set EarHorn up somewhere unfamiliar, which, it turns out, is when you need a baby monitor most.

The second was quieter, and it stuck. The best baby monitor is the one you already own. And when you're flying, it's the one that barely takes up any space at all.

Thanks for reading.

*EarHorn is a convenience tool for audio monitoring and is not a substitute for attentive supervision.*
