---
title: "Easy, Quick and Seamless Incident Response Process"
date: 2022-01-10T14:17:16-05:00
draft: false
toc: true
images:
tags:
  - incident-response
---

{{< image src="/images/posts/easy-quick-and-seamless-incident-response-process.jpg" alt="graphic-person-pointing-at-lock" position="center" style="border-radius: 8px;" >}}

Incident response should be easy, quick and seamless. Anyone should have the ability to manage an incident with-in your organization with only a few minutes of training. I know sounds simple and well it is, the problem starts when we add decision makers to the equation. Everyone has ideas, experience and opinions about how incidents should be handled, but few have actually increased the productivity and efficiency of an incident response team. The only focus when building a new incident response process (or fixing an old one) is to keep it ridiculously simple and avoid over complicating the process.

I have provided my basic incident response process and it should only be added to or changed when absolutely necessary. I'm serious, everyone keeps trying to re-invent the wheel but guess what, its really not worth the resources. I have used the process below as seen for well over five years and it has never failed me or anyone I have delegated it to.

## The Simple Incident Response Process

1. Create a **PRIVATE** slack channel using the [incident naming convention](#incident-naming-convention).

2. Paste the following into the slack channel and pin it  
   `⚠️ THIS IS STRICTLY CONFIDENTIAL AND SHOULD NOT BE SHARED OUTSIDE THIS CSIRT TEAM ⚠️`

3. Using the [incident management folder structure](#incident-management-folder-structure) create a new folder for the new incident. Be sure to continue using the [incident naming convention](#incident-naming-convention)

4. Add the Incident Log Template to the new incident folder and rename it `YYYYMMDD-X - Incident Report`

5. Link the new Incident Log to the slack channel and pin it

6. Optional: Create a `Artifacts` folder with-in the new incident folder to neatly store any screenshots, logs, emails, etc.

## Incident Naming Convention

I use the following naming convention as it makes the incident ambiguous but standardized. If you want the naming convention to be even more ambiguous use a random word generator and combine two random words (ex. `duck-reading`). I personally like to use the date to help keep incidents in chronological order (hint: thats why I use the year, month, day format).

```asciidoc
YYYYMMDD-X
|   |  | |
|   |  | +-- [X] Increment when multiple incident occur in a single day
|   |  |
|   |  +-- [DD] Day
|   |
|   +-- [MM] Month
|
+-- [YYYY] Year
```

## Incident Management Folder Structure

This is an example of what the folder structure should look like to manage incidents. It is extremely important to stay organized as much as possible to make finding information later much easier.

```asciidoc
/
+-- Incidents
  |
  +-- 20220110-1
  | |
  | +-- 20220110-1 - Incident Report
  | +-- Artifacts
  |   |
  |   +-- screenshot-1.jpg
  |   +-- screenshot-2.jpg
  |   +-- screenshot-3.png
  |
  +-- 20220101-1
    |
    +-- 20220101-1 - Incident Report
    +-- Artifacts
      |
      +-- screenshot-1.jpg
      +-- log-01-01-2022.json

```
