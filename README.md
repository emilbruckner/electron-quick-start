# electron-quick-start with Drift

**Clone and run for a quick way to see Electron with Drift in action.**

This is a fork of [Electron Quick Start](https://github.com/electron/electron-quick-start).

## To Use

To clone and run this repository you'll need [Git](https://git-scm.com) and [Node.js](https://nodejs.org/en/download/) (which comes with [npm](http://npmjs.com)) installed on your computer. From your command line:

```bash
# Clone this repository
git clone https://github.com/emilbruckner/electron-quick-start
# Go into the repository
cd electron-quick-start
# Install dependencies
npm install
# Run the app
npm start
```

Note: If you're using Linux Bash for Windows, [see this guide](https://www.howtogeek.com/261575/how-to-run-graphical-linux-desktop-applications-from-windows-10s-bash-shell/) or use `node` from the command prompt.

# Testing Drift

What doesn't work for me
(If it somehow works for you, I'll write some tests):

If I do

```javascript
drift.identify(
  'test', 
  {email: 'tester@hans.com'}
)
```

in the console, or anywhere else in the code, there are two possible outcomes:

1) The identify call does nothing
2) No more messages can be sent

This repo's code only includes the basic Drift snippet (with my drift id), but no `.identify`.
