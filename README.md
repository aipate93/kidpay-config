# kidpay-config

Signed configuration read by the KidPay mobile app: the list of backend addresses
it may connect to.

- `endpoints.json`: production builds.
- `endpoints-dev.json`: development builds.
- `istoric/`: every published version.

Each file is signed with Ed25519, and the app accepts it only with a valid
signature from a key built into the app. A copy hosted anywhere else, or any
edit to the file, is ignored.

Published with `tools/api-config/kpcfg.py` from the KidPay repository.
Do not edit these files by hand.
