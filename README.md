# Network-Access-Smart-Detection-And-QoE-based-selection-NASDAQ-
Software component
## Summary 
In the context of heterogeneous and coexisting networks, the introduction of context-aware and
cognitive mechanisms may allow the final user to optimize 1) the detection of surrounding access
networks, and 2) the selection of the best one, thus improving Quality of Experience (QoE). The
present proposal investigates this approach, by introducing the use of 1) MAC layer parameters for
the detection of surrounding networks, and 2) application layer QoE parameters, namely Key
Performance Indicators (KPIs), for optimizing the access network selection, respectively. MAC
parameters and KPIs will be defined for different traffic types, and then used to 1) detect and
recognize the access networks in the user surrounding area, 2) rank them, and select the one with
highest estimated QoE, for each considered traffic type.

NASDAQ is a tool for QoE-based network selection, in the form of an Android app. At its
present implementation, it allows the analysis of the radio environment, in order to
detect, identify and rank the WiFi Access Points (APs) available in the area. The app
makes possible:

* the collection (via direct measurement) of QoE parameters, allowing the
evaluation of Key Performance Indicators (KPIs), relative to two different traffic
types: VoIP and video streaming. At this step, a connection is established with each
candidate APs, and the ping utility is used to send test packets (Internet Control
Message Protocol echo requests) to a website server. Ping utility offers as a result
statistics about the link such as average delay, jitter and packet loss; KPIs are
computed using these measured values, together with the link estimated
bandwidth.
* the ranking of the candidate WiFi APs, from the one with highest estimated
performance to the one with lowest performance, assigning a score in the 0 – 100
range, obtained as a linear combination of the measured KPIs.

