---
description: A project checklist to walk through for Curated projects.
---

# Checklist for Curated Projects

❗❗❗Before proceeding to mainnet upload, please verify that your script behaves as expected across all major web browsers (e.g. Chrome, Firefox, Safari, etc.) ❗❗❗

## Upload

1. Ensure your wallet is funded with enough ETH to pay the gas fees for the upload and unpausing process. For more information on the estimated cost of these steps, [click here.](https://docs.artblocks.io/creator-docs/creator-onboarding/readme#cost)
2. Submit one field at a time. Wait for that transaction to clear before attempting the next field.
3. When you upload your script, please copy it exactly from testnet.
4. Include the following in the Project Base URI field: `https://api.artblocks.io/token/`
5. As [noted in the main documentation overview](../#token), please ensure that you are only setting a currency address if you are using some custom ERC20-compatible token (e.g., DAI) for the sale of your work. This field **should not** be set if you are accepting ETH as your payment type.
6. Please double-check, triple-check, and then check again the generated [features script](./readme/features.md) results on staging to ensure they are 100% accurate. This is **extremely important** to get right, as it changes to fix any bugs you may introduce in this script may have massive impact on how the artwork is perceived by collectors and may cause confusion in the secondary market. It is **your responsibility** to guarantee that your features script is properly verified in the artist staging environment.

## Scheduling

* Art Blocks will work with you to schedule your curated release.

## Mint #0

1. **Before** minting mint #0, ensure that your "additional payee wallet" has been set for the same configuration that you will use it for in your project release. E.g., if you are using the "additional payee wallet" field to donate to charity at the time of mint, you must set this before minting your #0. This is done to ensure that this full functionality is tested end-to-end as part of the mint #0 process, and that there are no issues with the wallet selected for the additional payee.
2. Once your project information has been uploaded, please confirm that you're ready for mint #0.
3. Mint #0 should occur at least 48 hours in advance of your scheduled release.

## Features

1. Please see [FEATURES.md](./readme/features.md) for full details on how you set your project features as an artist.
2. The features script for your project should first be tested on the Ropsten testnet ([https://artist-staging.artblocks.io/](https://artist-staging.artblocks.io)), alongside your art script. Ensure that your features are being displayed as expected on testnet before proceeding to project deployment to mainnet.
3. When uploading your feature script to mainnet ([https://beta.artblocks.io/](https://beta.artblocks.io)), please ensure that you are uploading the exact same features script, taking the same care that you would with your art script itself.
4. While the features script _is not_ stored on-chain like the art script is, bugs in your features script will cause meaningful disruptions for collectors trying to explore your work on a per-feature basis.

## Unpausing

* When it's time, you'll click the Unpause button under the Danger tab.
* Once the transaction clears, your project will be live for minting.

## Rarities

* Do not discuss odds or feature rarities about your project until it is completely sold out.

## Finishing Steps

1. Once your project is completely sold out, please reset the Additional Payee Percentage to 0% for any charitable giving that was conducted during minting.
2. You may also remove any language from your Project Description that was specifically included to describe sales mechanics.
3. We would also appreciate it if you could report back once your charity donations have been completed so that we can log the results.
4. Finally, please fill out the appropriate form to add bot-support to your Discord channel for your completed project: [https://github.com/ArtBlocks/artbot/issues/new/choose](https://github.com/ArtBlocks/artbot/issues/new/choose)
