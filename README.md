# endjinn - Private Transactions for the Enterprise

This project takes the concepts that are found in Quorum, Pantheon, Hyperledger Fabric and Corda around private transactions and abstracts them.

The core capability that each of these provides is the ability to send private transactions between parties.

Each implements a different mechanism of integrity.

endjinn provides a means to do this which is abstracted from any blockchain or DLT implementation.

This means that you can transact with peers and decide what mechanism of integrity you would like to use.

There are some key issues with existing implementations:

- No ability to choose between "on" or "off" ledger transactions
- Implementations strongly tied to 1 organisation == 1 node (no option for "multi tennancy")
- For Quorum no consensus on private SCs
- For fabric - static config
- For Quorum - immutable smart contract make evolution of logic heavyweight which leads to pushing logic out of smart contracts and reducing integrity
- Dynamic networks - Fabric and Corda have concepts around this but 

endjinn intends to start with these constraints in mind.



