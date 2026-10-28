# Lab Practical Timer

A station rotation timer for lab practicals. Students see **Work Time** while they are at a station and **Rotate to Next Station** when it is time to move. It includes three themes: Classic, Histology and Fetal Pig. Each theme remembers its own station count and times.

There is no build step. It is plain HTML, so GitHub and Vercel can host it as-is.

## What is in this folder

| File | What it does |
| --- | --- |
| `index.html` | The whole app |
| `manifest.webmanifest` | Lets Chrome, Edge and Safari install it like an app |
| `sw.js` | Saves the app so it still opens if the school Wi-Fi drops |
| `icons/`, `favicon.svg` | App and browser tab icons |
| `vercel.json` | Small hosting settings for Vercel |

## Put it on GitHub (website upload)

1. Go to github.com and click **New repository**. Name it `lab-practical-timer`, leave everything else as is, and click **Create repository**.
2. On the new repository page, click **uploading an existing file**.
3. Open this folder on your computer, select everything inside it (including the `icons` folder), and drag it onto the upload area.
4. Click **Commit changes**.

## Host it on Vercel

1. Go to vercel.com and click **Add New… → Project**.
2. Find `lab-practical-timer` in your GitHub list and click **Import**.
3. Leave **Framework Preset** on **Other** and leave the build settings empty.
4. Click **Deploy**. Vercel gives you an address like `lab-practical-timer.vercel.app`.

From then on, any file you change on GitHub is published to that address automatically within a minute.

## Install it on your laptop

Open the Vercel address in Chrome or Edge and click the install icon at the right end of the address bar. It then opens in its own window without browser tabs, which is ideal for projecting.

## Keeping the laptop awake

While the timer is running or paused, the app asks the browser to block sleep. A green **Laptop stays awake** badge at the top confirms it worked. This works in current Chrome, Edge, Safari and Firefox on an `https://` address such as your Vercel link.

The browser releases the lock if you switch to a different tab or minimize the window, and the app grabs it again as soon as the timer is back in front. Closing the laptop lid will still put it to sleep.

## Keyboard shortcuts

Space start or pause · → skip · ← back · + add 15 seconds · F big screen · S settings · T switch theme · M sound on or off · R twice to start over
