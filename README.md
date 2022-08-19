# co-infuse

A Lightning Network monetised, Chaumian voucher driven distributed VPN for payment, messaging and p2p hosting

## About

The transparent and public base layer of internet money, Bitcoin, does not have measures to protect against state level actors from acquiring intelligence on the physical locations correlating with transactions.

As a result, many users rely on the Tor network for protecting their transactions from being detected as originating at or near their real Point of Presence. Many Lightning channels are linked over Tor for similar reasons.

In recent times (as at August 2022) the Tor network is now being heavily attacked via "DDoS" and it is most likely that this is in fact a large scale state level attack by one or several states attempting to capture routing data for Bitcoin transactions.

Bitcoin is now a very valuable asset and payment network, and while it does not need to be faster, it does need to have physical location privacy for the safety of its users.

Co-infuse will use a liquidity pool system where users are able to acquire chaumian coins issued by various router nodes that pay for bandwidth by the session, so each node unwraps the part that is meant for them, they receive the payment, and forward the packet as per the delivery instructions.

One of the delivery destinations will be the Bitcoin mempool, then there will be rendezvous points for hidden services, and tunnel exit will have another delivery mode as well, which will likely be a lot more expensive due to the abuse potential and counterattack that may occur for such proxy exit points. Nodes will advertise their rate in satoshis per megabyte, users' clients establish the initial channel path with a session payment, receive a session cookie which then is included in each layer of the onion header as data transits.

Co-infuse will be built on the libp2p library, piggybacking on the distributed node database IPFS uses as a means to connecting to services, and service codes will advertise what prices a node is offering at a given time, addresses they are rendezvous points for, and whether they will allow exit traffic to tunnel out.

By making it possible for relay services to be paid for anonymising traffic, it should then enable the network to rapidly scale in complexity and bandwidth capacity to defeat any attack from even the most well funded adversaries.
