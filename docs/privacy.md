# Privacy at Vibesterz

Vibesterz is built around a simple idea: the AI should come to your data, not the
other way around. This page explains what that means in practice.

## What stays on your device

- **Your prompts.** What you type to the AI is processed in your browser.
- **Your code and files.** Anything you paste, upload or open is handled locally.
- **What the AI produces.** Generated apps, text, images and other output are
  created on your machine.
- **Your projects and history.** These are saved in your browser using its built in
  storage, not in a central account.

## No accounts

There is no sign up and no sign in. There is no password to manage and no user
profile stored on a server. You open the workspace and start working.

Because there is no account, there is also no central record of who you are or what
you have built sitting in a database somewhere.

## When the network is used

Being honest about this matters more than a tidy slogan. Vibesterz uses a
connection in a small number of clear situations:

1. **Loading the app.** Like any website, the application has to load.
2. **Downloading a model.** The first time you use a given model, it is downloaded
   and then cached on your device for offline use.
3. **An optional API proxy.** If an app you build calls an external API, that call
   can be routed through a proxy so it succeeds from the browser. This only happens
   for apps that make such calls.
4. **Publishing.** If you choose to publish an app you built, that action sends it
   so it can be shared. This only happens when you ask for it.

Running the AI to generate something does not upload your prompts or files.

## Verify it yourself

You do not have to take our word for it.

1. Open your browser developer tools.
2. Go to the Network tab.
3. Load a model once.
4. Ask the AI to build or generate something.

The generation step does not make network calls that carry your prompt or your
files to a server.

## Tools that help you protect data

The toolbox includes tools built specifically for privacy, all running on your
device: a redactor for stripping sensitive data out of documents, a metadata
stripper for photos, a data anonymizer for spreadsheets, a secret scanner, a
file encryption vault and more.
