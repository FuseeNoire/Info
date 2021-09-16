# Currency
In a standard Minecraft server, the usage of a user-defined, centralized currency is infeasible. It is tedious to make verifiable currency, and the overhead required to do so often leads communities to rely on simple bartering, using hard-to-obtain items in its place.
## Approach
The following proposed guidelines utilize the previously described [Tagging](../spec/Tagging.md) function in order to simulate promissory notes, cheques, bonds, & resource-standardized currency. It will be up to the in-game organizations that provide currency to create their own economic systems.

For this example, we will assume a nation creates a central bank, which will mint currency and manage transactions. For their currency to function, they must;
* Have the trust of multiple individuals that attribute value to the currency.
  * This can be attained multiple ways, such as forcing your populous to trade using your currency internally, or tying your currency to a sought after item, such as diamonds.
* Employ counterfeit mitigation strategies.
  * This is described in-depth [here](#Counterfeit).
* Manage inflation, deflation, and other economic policy.

The application of this policy would allow a government to use its populace's combined wealth to give loans and create long-term profit.

### Counterfeit
A major flaw of creating currency in vanilla Minecraft is counterfeit. If a player simply makes more notes without the authority of the bank, they have access to more wealth.

This is resolved by [Tagging](../spec/Tagging.md). The bank can tag wealth (whether by tagging a registered account, the specific deposit, or the promise of future returns) using a private variable, and then having the note, cheque, or bond be tagged with another correlating private variable. A signed price can be the result of a shared secret between the two variables.

More traditional cryptography can be employed to further secure the authenticity of the currency. It is reasonably possible to tie a note's key to an external database and log transactions outside the server itself.