# fingerprint2 broken server side render

For discussion on this issue see https://github.com/Valve/fingerprintjs2/pull/378

## How to use

```bash
git clone https://github.com/alexhayes/fingerprint2-broken-ssr.git
cd fingerprint2-broken-ssr
yarn
yarn dev
```

Then browse to http://localhost:3000

You should see a message that states: `Internal Server Error`

## Applying the fix

```
yarn remove fingerprintjs2
yarn add git+https://github.com/alexhayes/fingerprintjs2.git#feature/dont-break-server-side-render
yarn dev
```

Then browse to http://localhost:3000 and things should be fixed.
