# Algorithmic Tweet Highlighter

A (tiny) Chrome extension to fix an annoying problem with Twitter's new algorithmic timeline.

## Outline

Twitter recently started showing a selection of algorithmically sorted tweets at the top of users' timelines. The implementation of this feature on Twitter's web interface has an unfortunate design flaw — it's difficult to tell where the non-chronological, algorithmic tweets end and the usual chronologically sorted tweets begin.

This project provides a simple Chrome extension that resolves this ambiguity by highlighting the non-chronological, algorithmic tweets on [twitter.com](https://twitter.com).

## Specifics

Algorithmically sorted tweets are marked by Twitter with certain `<div>` tag attributes. This extension injects a (very) small amount of CSS onto Twitter's main timeline that identifies and highlights these tweets. Specifically, "algorithmic" tweets are given a thin gray bar that runs down their left edge (see below), connecting them into an easily identifiable "algorithmic timeline" block.

![screenshot 1](screenshot-1.png?raw=true "Algorithmic (top) vs. Chronological (bottom)")

## Installing

The actual extension code is contained within the `extension/` sub-directory. For now, follow the instructions on Chrome's developer site for [loading an unpacked extension](https://developer.chrome.com/extensions/getstarted#unpacked).

