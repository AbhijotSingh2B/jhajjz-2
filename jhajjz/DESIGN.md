---
name: Jhajj'z
description: The arrival porch. Chauffeur-driven luxury cars and coaches, lit like exhibits on one night-black field.
colors:
  night: "#0d0c0a"
  porch-floor: "#16140f"
  surface: "#1d1a15"
  bone: "#eeece7"
  stone: "#b3aea5"
  sign-red: "#c41f12"
  sign-red-hover: "#d92a1a"
  on-red: "#ffffff"
typography:
  display:
    fontFamily: "Switzer, Helvetica Neue, Helvetica, Arial, sans-serif"
    fontSize: "clamp(2.5rem, 1.2rem + 4.4vw, 4.25rem)"
    fontWeight: 300
    lineHeight: 1
    letterSpacing: "-0.04em"
  heading:
    fontFamily: "Switzer, Helvetica Neue, Helvetica, Arial, sans-serif"
    fontSize: "clamp(1.875rem, 1.3rem + 1.9vw, 2.875rem)"
    fontWeight: 400
    lineHeight: 1.08
    letterSpacing: "-0.03em"
  lead:
    fontFamily: "Switzer, Helvetica Neue, Helvetica, Arial, sans-serif"
    fontSize: "clamp(1.25rem, 1.1rem + 0.7vw, 1.625rem)"
    fontWeight: 400
    lineHeight: 1.3
    letterSpacing: "-0.02em"
  body:
    fontFamily: "Switzer, Helvetica Neue, Helvetica, Arial, sans-serif"
    fontSize: "clamp(1.0625rem, 1rem + 0.25vw, 1.1875rem)"
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: "-0.01em"
  small:
    fontFamily: "Switzer, Helvetica Neue, Helvetica, Arial, sans-serif"
    fontSize: "clamp(0.8125rem, 0.79rem + 0.1vw, 0.875rem)"
    fontWeight: 400
    lineHeight: 1.5
  marque:
    fontFamily: "Switzer, Helvetica Neue, Helvetica, Arial, sans-serif"
    fontSize: "clamp(110px, 19vw, 330px)"
    fontWeight: 500
    lineHeight: 0.8
    letterSpacing: "-0.06em"
rounded:
  none: "0px"
spacing:
  gutter: "clamp(16px, 2.2vw, 32px)"
  section: "clamp(120px, 14vw, 220px)"
  stack: "24px"
components:
  button-primary:
    backgroundColor: "{colors.sign-red}"
    textColor: "{colors.on-red}"
    typography: "{typography.small}"
    rounded: "{rounded.none}"
    padding: "0 1.4em"
    height: "52px"
  button-primary-hover:
    backgroundColor: "{colors.sign-red-hover}"
  switch:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.stone}"
    typography: "{typography.small}"
    rounded: "{rounded.none}"
    padding: "12px 16px"
    height: "44px"
  switch-on:
    backgroundColor: "{colors.bone}"
    textColor: "{colors.night}"
  fleet-row-active:
    backgroundColor: "{colors.sign-red}"
    textColor: "{colors.on-red}"
---

# Design System: Jhajj'z

## Overview

**Creative North Star: the arrival porch.** Every Jhajj'z job ends the same way: a car pulling up under the lights of a hotel porch at night. The page is one dark driveway where the fleet stands lit, from the Rolls-Royce to the coach. Cars and photographs are the only bright things on any screen; type is light, sparse and set in one neo-grotesk. The red of the Jhajj'z sign is the only colour that acts.

Anti-references: the stock luxury-rental template (hero photo, fleet card grid, icon service tiles), gold-on-black "premium" chrome, cream-and-serif hospitality pages.

## Colors

- **Night** (`night`, #0d0c0a): the single page ground, warm-neutral black, top to bottom. No section bands except the red cities field.
- **Porch floor** (`porch-floor`, #16140f): the floor band the cars stand on and the alternate fleet rows. A tone step, never a line.
- **Surface** (`surface`, #1d1a15): resting switches, and the giant car name behind the line-up.
- **Bone** (`bone`, #eeece7) for text and **Stone** (`stone`, #b3aea5) for secondary notes. Both pass 8:1 or better on Night.
- **Sign red** (`sign-red`, #c41f12): taken from the Jhajj'z showroom sign and the wedding ribbons. Used only for the one action (WhatsApp), the active fleet row, and one full field (the cities ticker). Never decorative.

## Typography

One family, Switzer (self-hosted, 300/400/500). Five steps: display (the h1, light 300), heading, lead, body, small. The marque (the current car's short name, 19vw, weight 500, in Surface) sits behind the line-up as scenery, not text. Tracking tightens with size (-0.01em body to -0.06em marque). Sentence case everywhere; no uppercase labels, no monospace.

## Layout

One pair of outer margins (`gutter`) and a 12-column grid. Sections sit `section` apart. The hero is a drag row: cut-out cars on a shallow arc, scroll-snapped, the centre car about 44vw on desktop with siblings 30% smaller and a quarter darker per step. The occasions section pins one darkened photograph for about 2.4 screens while photo plates cross it. The fleet list keeps its middle column empty for a car that travels down it and changes per row. Phones get their own compositions: no pin, stacked plates, the gallery alternating 100% and 84% widths.

## Elevation & Depth

Flat. No shadows on anything at rest. Depth comes from light: a warm porch-light pool under the centre car, a tyre contact shadow and a faint floor reflection under every car, and photographs dimmed slightly so they sit in the dark. Real Jhajj'z cut-outs are graded down (brightness 0.86, saturation 0.88) to share the night key with the studio renders.

## Shapes

Square corners everywhere: buttons, switches, photographs, the contact plate. No pills, no rounded cards, no outlines.

## Components

- **Primary button**: flat sign-red rectangle, 52px tall, white label, WhatsApp glyph. One per screen at most. Its link carries a pre-filled message naming the car on the porch.
- **Occasion switch**: flat surface rectangle; the pressed one turns bone with night text. Pressing one drives the line-up to its car.
- **Line-up car**: a button holding a transparent cut-out; scale, lift and brightness are set from its distance to the centre. Each states whether its picture is illustrative or photographed at the yard.
- **Fleet row**: full-width band, name and models left, best use right; the row under the travelling car turns sign-red.
- **Photo plate**: photograph over a ground-coloured text plate, no tint, no frame.

## Do's and Don'ts

- Do show the cars large and lit; every section leads with a vehicle or a real Jhajj'z photograph.
- Do label model pictures that are illustrative, and never present a stock render as the client's own car.
- Do keep red for action and the one cities field.
- Don't add cards with tinted panels, eyebrow labels, numbered sections, gradients as decoration, glass, or glows beyond the porch light and floor shadows.
- Don't invent proof: no reviews, client logos, prices or fleet counts until the client supplies them.

Not canonized: the giant marque deliberately sits behind a car (allowed as scenery only, never for headings or copy).
