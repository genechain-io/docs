# Common Errors

## REPLACEMENT\_UNDERPRICED

The error message may be `replacement transaction underpriced` or `replacement fee too low`.

The error message implies that you're trying to replace a pending transaction. That's because the raw transaction you're trying to send has the same `nonce` as another transaction that you have pending. And the Gas Price of pending transaction is greater than or equal to the transaction you just sent.

If your goal is to replace pending transactions, you must use a gas price that is higher than the `gasPrice` of the pending transaction.

If replacing a transaction is not your goal, simply increase the nonce to be one higher than your last pending transaction.

## nonce too low

This error message means that the newly sent transaction uses a `nonce` that has already been used. You can check your `nonce` by reviewing your last confirmed transaction in the [blockchain explorer](https://scan.genechain.io).

## transferFrom failed

This error message usually means that the amount of ERC20 token passed exceeds the number you have. Reducing the amount of ERC20 token passed may solve the problem.

## out of gas

If you see the message "out of gas", your transaction was executed but failed. In other words, there was an error completing the transaction because it requires more gas than you attach to the transaction. It's similar to running out of gas when driving a car, except imagine that you reached your destination without being able to get _out_ of the car.

To avoid another "out of gas" error, you will need to increase the gas limit of your next transaction. This can be done just before sending your next transaction. Learn more about gas, gas price and gas limit [here](../basics-of-blockchain-and-genechain.md#what-is-gas).

