# Ledgers

The XRP Ledger is a shared, global ledger that is open to all. Individual participants can trust the integrity of the ledger without having to trust any single institution to manage it. The XRP Ledger protocol accomplishes this by managing a ledger database that can only be updated according to very specific rules. Each server in the peer-to-peer network keeps a full copy of the ledger database, and the network distributes candidate transactions, which are applied in blocks according to the [consensus process](../consensus-protocol/index.md).

"Diagram: Each ledger is the result of applying transactions to the previous ledger version."

The shared global ledger consists of a series of blocks, called ledger versions or simply _ledgers_. Every ledger version has a [Ledger Index][] which identifies the correct order of ledgers. Each permanent, closed ledger also has a unique, identifying hash value.

At any given time, each XRP Ledger server has an in-progress _open_ ledger, a number of pending _closed_ ledgers, and a history of _validated_ ledgers that are immutable.

A single ledger version consists of several parts:
