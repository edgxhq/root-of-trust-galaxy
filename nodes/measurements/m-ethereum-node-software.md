---
id: m-ethereum-node-software
type: measurement
title: "Ethereum has many client teams, and one consensus client runs on about half of nodes"
description: "Ethereum has more independent node implementations in production than any other network here. One of them runs on about half of consensus nodes."
status: developing
visibility: public
network: net-ethereum
dimension: dim-node-software
value: 1
value_hi: 2
unit: "client implementations"
threshold: "about half of each layer; trackers disagree"
as_of: 2026-11-19
verified: main
tags: [node-software, ethereum]
links:
  - rel: derived-from
    to: src-clientdiversity-data
  - rel: derived-from
    to: src-clientdiversity
created: 2026-11-19
updated: 2026-11-19
---

Ethereum is ahead of every other network here on the number of independent implementations in production: at
least six consensus clients and five execution clients, from different teams.

The question is how evenly they are used. Counting consensus nodes on 18 November 2026, Lighthouse ran on 5,981
of about 11,800, which is 51%. Prysm had 20%, Nimbus 10%, Teku 7%. Other trackers measure by validators and
disagree: one put Teku above half. On the execution side a source the tracking site itself calls unreliable put
Geth at 50%.

If one client is above half, the count is 1; just below, it is 2. Counted by nodes, not by stake.
