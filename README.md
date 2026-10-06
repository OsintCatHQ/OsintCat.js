# OsintCat.js (deprecated)

This client is deprecated and no longer works with the OsintCat API: it sends the key in a way the
API no longer accepts, and several of its endpoints have been removed.

Use the new official SDK instead, published under the same name:

```sh
npm install osintcat@latest
```

```typescript
import { OsintCatClient } from "osintcat";

const client = new OsintCatClient({ apiKey: process.env.OSINTCAT_API_KEY });
const breach = await client.breach.search({ query: "user@example.com" });
```

Version 2 and later are the new SDK; versions 1.x on npm are this old client and are marked deprecated.
Documentation: [docs.osintcat.net](https://docs.osintcat.net). API keys:
[Account > Developer](https://www.osintcat.net/account/developer).
