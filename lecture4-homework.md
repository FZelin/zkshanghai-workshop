# 第4课 课后作业

## Check out https://semaphore.appliedzkp.org/ and set up a starter project!


按照步骤做了，好像是报了solidity插件错误。。
```shell

chaomi@chaomideMBP zkwork % npx @semaphore-protocol/cli@latest create my-app --template monorepo-ethers

 ✔ Your project is ready!

 Please, install your dependencies by running:

   cd my-app
   npm i

 Available scripts:

   npm run dev
   npm run dev:web-app
   npm run dev:contracts
   npm run lint
   npm run prettier
   npm run prettier:write
   npm run copy:contract-artifacts
   npm run prepublish

 See the README.md file to understand how to use them!

chaomi@chaomideMBP zkwork % cd my-app
chaomi@chaomideMBP my-app % npm i
npm WARN deprecated mkdirp-promise@5.0.1: This package is broken and no longer maintained. 'mkdirp' itself supports promises now, please switch to that.
npm WARN deprecated request-promise-native@1.0.9: request-promise-native has been deprecated because it extends the now deprecated request package, see https://github.com/request/request/issues/3142
npm WARN deprecated rollup-plugin-terser@7.0.2: This package has been deprecated and is no longer maintained. Please use @rollup/plugin-terser
npm WARN deprecated har-validator@5.1.5: this library is no longer supported
npm WARN deprecated fsevents@2.1.3: "Please update to latest v2.3 or v2.2"
npm WARN deprecated sourcemap-codec@1.4.8: Please use @jridgewell/sourcemap-codec instead
npm WARN deprecated debug@3.2.6: Debug versions >=3.2.0 <3.2.7 || >=4 <4.3.1 have a low-severity ReDos regression when used in a Node.js environment. It is recommended you upgrade to 3.2.7 or 4.3.1. (https://github.com/visionmedia/debug/issues/797)
npm WARN deprecated uuid@2.0.1: Please upgrade  to version 7 or higher.  Older versions may use Math.random() in certain circumstances, which is known to be problematic.  See https://v8.dev/blog/math-random for details.
npm WARN deprecated uuid@2.0.1: Please upgrade  to version 7 or higher.  Older versions may use Math.random() in certain circumstances, which is known to be problematic.  See https://v8.dev/blog/math-random for details.
npm WARN deprecated multicodec@1.0.4: This module has been superseded by the multiformats module
npm WARN deprecated uuid@3.4.0: Please upgrade  to version 7 or higher.  Older versions may use Math.random() in certain circumstances, which is known to be problematic.  See https://v8.dev/blog/math-random for details.
npm WARN deprecated uuid@3.3.2: Please upgrade  to version 7 or higher.  Older versions may use Math.random() in certain circumstances, which is known to be problematic.  See https://v8.dev/blog/math-random for details.
npm WARN deprecated workbox-cacheable-response@6.6.0: workbox-background-sync@6.6.0
npm WARN deprecated request@2.88.2: request has been deprecated, see https://github.com/request/request/issues/3142
npm WARN deprecated multibase@0.6.1: This module has been superseded by the multiformats module
npm WARN deprecated multibase@0.7.0: This module has been superseded by the multiformats module
npm WARN deprecated multicodec@0.5.7: This module has been superseded by the multiformats module
npm WARN deprecated cids@0.7.5: This module has been superseded by the multiformats module
npm WARN deprecated snarkjs@0.4.13: Sucurity bug fixed

> @semaphore-protocol/cli-template-monorepo-ethers@3.10.1 prepublish
> tar -czf files.tgz .gitignore .yarn .yarnrc.yml apps


added 1566 packages, and audited 1569 packages in 4m

191 packages are looking for funding
  run `npm fund` for details

30 vulnerabilities (19 moderate, 8 high, 3 critical)

To address issues that do not require attention, run:
  npm audit fix

To address all issues possible (including breaking changes), run:
  npm audit fix --force

Some issues need review, and may require choosing
a different dependency.

Run `npm audit` for details.
chaomi@chaomideMBP my-app % cd apps/contracts
chaomi@chaomideMBP contracts % npm test

> monorepo-ethers-contracts@1.0.0 test
> hardhat run scripts/download-snark-artifacts.ts && hardhat test

Compiled 14 Solidity files successfully


  Feedback
    # joinGroup
      ✔ Should allow users to join the group (925ms)
    # sendFeedback
      ✔ Should allow users to send feedback anonymously (2358ms)


  2 passing (6s)

chaomi@chaomideMBP contracts % npm run test:coverage

> monorepo-ethers-contracts@1.0.0 test:coverage
> hardhat coverage


Version
=======
> solidity-coverage: v0.7.22

Instrumenting for coverage...
=============================

> Feedback.sol

Compilation:
============

Generating typings for: 12 artifacts in dir: ./build/typechain for target: ethers-v5
Successfully generated 40 typings!
Compiled 14 Solidity files successfully
Error in plugin solidity-coverage: TypeError: provider.send is not a function

For more info run Hardhat with --show-stack-traces
npm ERR! Lifecycle script `test:coverage` failed with error: 
npm ERR! Error: command failed 
npm ERR!   in workspace: monorepo-ethers-contracts@1.0.0 
npm ERR!   at location: /Users/chaomi/zkwork/my-app/apps/contracts 
```
