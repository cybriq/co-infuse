# go-infuse
A Lightning Network monetised, Chaumian voucher driven distributed VPN for payment, messaging and p2p hosting

## About

The transparent and public base layer of internet money, Bitcoin, does not have measures to protect against state level actors from acquiring intelligence on the physical locations correlating with transactions.

As a result, many users rely on the Tor network for protecting their transactions from being detected as originating at or near their real Point of Presence. Many Lightning channels are linked over Tor for similar reasons.

In recent times (as at August 2022) the Tor network is now being heavily attacked via "DDoS" and it is most likely that this is in fact a large scale state level attack by one or several states attempting to capture routing data for Bitcoin transactions.

Bitcoin is now a very valuable asset and payment network, and while it does not need to be faster, it does need to have physical location privacy for the safety of its users.

Coinfuse is the name of the protocol we are proposing in the development of this protocol.

In short, it uses a system of chaumian minted coins that are paid between nodes as private vouchers, to pay relaying fees for users who are sending packets in a prescribed format, the initial format being the classic 3 step onion route, the user is invoiced for a relaying session, and then uses chaumian coins it has received from other routers to pay the fees for a stage in the onion route, eliminating the linking between the client and the endpoint.

It is the lowest priority for this network to be used to tunnel back out to the internet, and likely a high price due to the abuse that this kind of service enables. Instead, the goal of Coinfuse is aimed towards hidden services hosting for messaging and internal network content delivery, a dark-by-default-web, and the most important service, relaying transactions onto the Bitcoin blockchain, which will be a default 3 hop relay destination that exits into the Bitcoin mempool.

Relaying transactions onto the mempool, relaying private messages between users, enabling dynamic point of presence for mobile and intermittently connected connections with a moderate latency requirement for lightweight web applications are the three main purposes of Coinfuse. It is intended to reinforce the censorship resistance of the Bitcoin and Lightning networks, as well as increasing the security of users especially when transacting large amounts of bitcoin to not reveal their physical location to powerful entities with large infrastructure for surveillance.
