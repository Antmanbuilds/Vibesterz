# How Vibesterz works

This is a high level overview for the curious. It describes the shape of the
product, not its internal implementation.

## The model runs on your device

When you open the workspace, Vibesterz loads a language model into your browser and
runs it on your GPU using WebGPU. The work of generating happens in the same tab
you are looking at. There is no remote server doing the thinking for you, and your
prompts and files are not uploaded to produce results.

The first time you use a model, it is downloaded to your machine and cached. After
that it loads from the cache, which is what lets the workspace keep working when you
are offline.

## Building an app

When you ask Vibesterz to build something, it does more than a single pass. At a
high level it plans the build, writes the code, reviews its own output for problems,
and polishes the result before showing it to you. You can watch progress as it
happens. The finished app renders in a live preview inside the same page.

You can choose how much effort goes into a build through a simple strategy setting,
trading speed for depth. Lighter hardware and mobile devices default to the fastest
path automatically.

## Offline first

Vibesterz is a progressive web app. The application shell and the tools are cached
so they keep working without a connection. You can install it to your device and
use it like any other app.

Storage is local. Your projects, your conversation history and the data your built
apps create live in your browser using its built in storage, not in a central
database.

## Apps you build can store data and have logins

Apps generated in Vibesterz can save data and support sign in, and they work fully
offline. Each generated app gets its own isolated local store, so two different
apps never mix their data. This all runs in the browser.

## The toolbox

Alongside the app builder, Vibesterz ships a catalog of focused tools for code,
writing, data, documents, vision, audio, knowledge, developer utilities and
privacy. Each tool runs the same way: on your device, with your content staying
local.

## A note on the network

To be precise about the few times Vibesterz uses a connection:

- Loading the application itself.
- Downloading a model the first time you use it.
- An optional proxy, used only when an app you build calls an external API, so that
  the call can succeed from the browser.
- The publish feature, used only if you choose to share an app you built.

Generating with the AI does not send your prompts or files to a server.
