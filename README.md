# Minimal Reproduction (`npm i remix-validated-form` fails in Remix V2)

## Context

This repo is a fresh Remix V2 install (untouched apart from this README.md). It was installed as follows: 

```sh
npx create-remix@latest
```

## Minimal Reproduction steps

Step 1: attempt to install @clerk/remix

```sh
npm i remix-validated-form
```

## Expected behavior: 

remix-validated-form successfully installs


## Actual behavior:

remix-validated-form fails to install with the following error:

```
npm ERR! code ERESOLVE
npm ERR! ERESOLVE could not resolve
npm ERR!
npm ERR! While resolving: remix@undefined
npm ERR! Found: @remix-run/server-runtime@2.0.0
npm ERR! node_modules/@remix-run/server-runtime
npm ERR!   @remix-run/server-runtime@"2.0.0" from @remix-run/dev@2.0.0
npm ERR!   node_modules/@remix-run/dev
npm ERR!     dev @remix-run/dev@"^2.0.0" from the root project
npm ERR!   @remix-run/server-runtime@"2.0.0" from @remix-run/node@2.0.0
npm ERR!   node_modules/@remix-run/node
npm ERR!     @remix-run/node@"2.0.0" from @remix-run/express@2.0.0
npm ERR!     node_modules/@remix-run/express
npm ERR!       @remix-run/express@"2.0.0" from @remix-run/serve@2.0.0
npm ERR!       node_modules/@remix-run/serve
npm ERR!         peerOptional @remix-run/serve@"^2.0.0" from @remix-run/dev@2.0.0
npm ERR!         node_modules/@remix-run/dev
npm ERR!         1 more (the root project)
npm ERR!     @remix-run/node@"2.0.0" from @remix-run/serve@2.0.0
npm ERR!     node_modules/@remix-run/serve
npm ERR!       peerOptional @remix-run/serve@"^2.0.0" from @remix-run/dev@2.0.0
npm ERR!       node_modules/@remix-run/dev
npm ERR!         dev @remix-run/dev@"^2.0.0" from the root project
npm ERR!       1 more (the root project)
npm ERR!     1 more (the root project)
npm ERR!   1 more (@remix-run/react)
npm ERR!
npm ERR! Could not resolve dependency:
npm ERR! remix-validated-form@"*" from the root project
npm ERR!
npm ERR! Conflicting peer dependency: @remix-run/server-runtime@1.19.3
npm ERR! node_modules/@remix-run/server-runtime
npm ERR!   peer @remix-run/server-runtime@"1.x" from remix-validated-form@5.1.0
npm ERR!   node_modules/remix-validated-form
npm ERR!     remix-validated-form@"*" from the root project
npm ERR!
npm ERR! Fix the upstream dependency conflict, or retry
npm ERR! this command with --force or --legacy-peer-deps
npm ERR! to accept an incorrect (and potentially broken) dependency resolution.
```
