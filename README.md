# Substrate Cumulus Parachain Template

Polkadot version v0.9.26
Rust version: 1.64-nightly

A new [Cumulus](https://github.com/paritytech/cumulus/)-based Substrate node, ready for hacking ☁️..

This project is originally a fork of the
[Substrate Node Template](https://github.com/substrate-developer-hub/substrate-node-template)
modified to include dependencies required for registering this node as a **parathread** or
**parachain** to a **relay chain**.

The stand-alone version of this template is hosted on the
[Substrate Devhub Parachain Template](https://github.com/substrate-developer-hub/substrate-parachain-template/)
for each release of Polkadot. It is generated directly to the upstream
[Parachain Template in Cumulus](https://github.com/paritytech/cumulus/tree/master/parachain-template)
at each release branch using the
[Substrate Template Generator](https://github.com/paritytech/substrate-template-generator/).

👉 Learn more about parachains [here](https://wiki.polkadot.network/docs/learn-parachains), and
parathreads [here](https://wiki.polkadot.network/docs/learn-parathreads).


🧙 Learn about how to use this template and run your own parachain testnet for it in the
[Devhub Cumulus Tutorial](https://docs.substrate.io/tutorials/v3/cumulus/start-relay/).

👉Create a smart contract using ink and implement

⇢ The first tool we will be installing is cargo-contract, a CLI tool for helping setting up and managing WebAssembly smart contracts written with ink!.
  As a pre-requisite for the tool you need to install the binaryen package, which is used to optimize the WebAssembly bytecode of the contract.

  `cargo install cargo-contract --force --locked`

⇢ The ink! contract requires the specification of two additional dependencies. This is done to alert consumers to potential security risks while accessing, for example, APIs.

   `cargo install cargo-dylint dylint-link`

⇢ Creating an ink! Project

  `cargo contract new xyz`

⇢ Testing Your Contrac

  `cargo +nightly test`

⇢ Compile Your Contract

  `cargo +nightly contract build`

⇢ Run a Substrate Node

⇢ Deploy Your Contract

    1. Click the Add New Contract button in the sidebar.
    2. Click the Upload New Contract Code button in the Add New Contract page.
    3. Choose an Instantiation account (e.g. ALICE).
    4. Give the contract a descriptive Name (e.g. xyz Contract).
    5. Drag the xyz.contract file that contains the bundled Wasm blob and metadata into the drag & drop area. You will see the UI parse the metadata and enabling the button that takes you to the next step.
    6. Click the Next button