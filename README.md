Babylon
===

Measurements data for the paper [Bitcoin-Enhanced Proof-of-Stake Security: Possibilities and Impossibilities](https://eprint.iacr.org/2022/932) accepted to [IEEE S&P 2023](https://www.ieee-security.org/TC/SP2023/).

### Babylon Experiment Setup

OP_RETURN code for the first BTC transaction (tx1) of a checkpoint (op1): OP_RETURN 42424e5402f7eca772cbea19d73f96e2e46a5d8110ec1d47a9dc8545590c1ab4d660976accb3bad8acc494be825617be80a325659666e8a962d8f9bccf504a7bbfa468cfc959ade26352 


OP_RETURN code for the second BTC transaction (tx2) of a checkpoint (op1): OP_RETURN 42424e54538176e4da5deb1262aaf9136926152b7255bfa4b35bfa7841178afc8316d2b6cc5a214aa05ec2549af70341f06e562c3c2d0b9795d253f890fa

op1 size: 70 bytes

op2 size: 58 bytes

tx1 size: 195 bytes

tx2 size: 183 bytes

During the experiment, we sent checkpoints hourly in two different fee levels.
The transactions are sent at the beginning of each hour starting from Aug. 18, 1:00 a.m. to Aug. 19 1:00 a.m. PT.
Transactions of the same checkpoint with different fee levels are sent simultaneously.

The confirmation duration is measured from the time the transactions are sent, to the time both the transactions are included in a block on blockchain.
The six-deep time is measured from the transaction sending time to the time the relevant block is confirmed 6 times.
The twenty-deep time is measured from the transaction sending time to the time the relevant block is confirmed 20 times.
To check the transactions sent during the experiment, please use the txid in [measurements.json](https://github.com/gitferry/Babylon-checkpoints/blob/main/measurements.txt) and an BTC explorer, e.g., [https://live.blockcypher.com/](https://live.blockcypher.com/).
