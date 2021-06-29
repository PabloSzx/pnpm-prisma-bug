# pnpm-prisma-bug


Run:

```sh
pnpm i
```

All what I get is:


```
λ pnpm i
Scope: all 2 workspace projects
Lockfile is up-to-date, resolution step is skipped
Packages: +4
++++
Packages are hard linked from the content-addressable store to the virtual store.
  Content-addressable store is at: C:\Users\pablo\.pnpm-store\v3
  Virtual store is at:             node_modules/.pnpm
.../node_modules/@prisma/engines postinstall$ node download/index.js
Progress: resolved 4, reused 4, downloaded 0, added 4, done
.../node_modules/@prisma/engines postinstall: Done
.../prisma@2.26.0/node_modules/prisma preinstall$ node scripts/preinstall-entry.js
.../prisma@2.26.0/node_modules/prisma preinstall: Done
.../prisma@2.26.0/node_modules/prisma install$ node scripts/install-entry.js
.../prisma@2.26.0/node_modules/prisma install: Done
.../node_modules/@prisma/client postinstall$ node scripts/postinstall.js
.../node_modules/@prisma/client postinstall: prisma:warn The postinstall script automatically ran `prisma generate` and did not find your `prisma/schema.prisma`.
.../node_modules/@prisma/client postinstall: If you have a Prisma schema file in a custom path, you will need to run
.../node_modules/@prisma/client postinstall: `prisma generate --schema=./path/to/your/schema.prisma` to generate Prisma Client.
.../node_modules/@prisma/client postinstall: If you do not have a Prisma schema file yet, you can ignore this message.
.../node_modules/@prisma/client postinstall: Done
packages/db prepare$ prisma generate
packages/db prepare: Environment variables loaded from .env
packages/db prepare: Prisma schema loaded from prisma\schema.prisma
packages/db prepare: > prisma@2.26.0 preinstall C:\Users\pablo\new-pnpnm-prisma\packages\db\node_modules\prisma
packages/db prepare: > node scripts/preinstall-entry.js
packages/db prepare: > prisma@2.26.0 install C:\Users\pablo\new-pnpnm-prisma\packages\db\node_modules\prisma
packages/db prepare: > node scripts/install-entry.js
packages/db prepare: > @prisma/engines@2.26.0-23.9b816b3aa13cc270074f172f30d6eda8a8ce867d postinstall C:\Users\pablo\new-pnpnm-prisma\packages\db\node_modules\@prisma\engines
packages/db prepare: > node download/index.js
packages/db prepare: npm notice save prisma is being moved from dependencies to devDependencies
packages/db prepare: npm notice created a lockfile as package-lock.json. You should commit this file.
packages/db prepare: npm WARN db-example@0.0.1 No description
packages/db prepare: npm WARN db-example@0.0.1 No repository field.
packages/db prepare: + prisma@2.26.0
packages/db prepare: added 2 packages from 1 contributor, updated 1 package and audited 4 packages in 2.049s
packages/db prepare: found 0 vulnerabilities
packages/db prepare: > @prisma/client@2.26.0 postinstall C:\Users\pablo\new-pnpnm-prisma\packages\db\node_modules\@prisma\client
packages/db prepare: > node scripts/postinstall.js
packages/db prepare: npm WARN db-example@0.0.1 No description
packages/db prepare: npm WARN db-example@0.0.1 No repository field.
packages/db prepare: + @prisma/client@2.26.0
packages/db prepare: added 1 package from 1 contributor, updated 1 package and audited 4 packages in 2.812s
packages/db prepare: found 0 vulnerabilities
packages/db prepare: Error: Could not resolve @prisma/client despite the installation that we just tried.
packages/db prepare: Please try to install it by hand with npm install @prisma/client and rerun prisma generate 🙏.
packages/db prepare: Failed
 ERROR  Command failed with exit code 1.
```
