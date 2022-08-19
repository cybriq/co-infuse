# go-infuse
A Lightning Network monetised, Chaumian voucher driven distributed VPN for payment, messaging and p2p hosting

## About

The transparent and public base layer of internet money, Bitcoin, does not have measures to protect against state level actors from acquiring intelligence on the physical locations correlating with transactions.

As a result, many users rely on the Tor network for protecting their transactions from being detected as originating at or near their real Point of Presence. Many Lightning channels are linked over Tor for similar reasons.

In recent times (as at August 2022) the Tor network is now being heavily attacked via "DDoS" and it is most likely that this is in fact a large scale state level attack by one or several states attempting to capture routing data for Bitcoin transactions.

Bitcoin is now a very valuable asset and payment network, and while it does not need to be faster, it does need to have physical location privacy for the safety of its users.

Coinfuse is the name of the protocol we are proposing in the development of this protocol.

It will use a liquidity pool system where users are able to acquire chaumian coins issued by various router nodes that pay for bandwidth by the session, so each node unwraps the part that is meant for them, they receive the payment, and forward the packet as per the delivery instructions.

One of the delivery destinations will be the Bitcoin mempool, then there will be rendezvous points for hidden services, and tunnel exit will have another delivery mode as well, which will likely be a lot more expensive due to the abuse potential and counterattack that may occur for such proxy exit points.

Coinfuse will be built on the libp2p library, piggybacking on the distributed node database it uses as a means to connecting to services, and service codes will identify what services a node is offering at a given time, relay, addresses they are rendezvous points for, and whether they will allow exit traffic to tunnel out.
