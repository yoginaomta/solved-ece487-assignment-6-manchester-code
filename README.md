Download Link: https://assignmentchef.com/product/solved-ece487-assignment-6-manchester-code
<br>
<ol>

 <li>Give Manchester code for the following data.</li>

</ol>

<ol start="2">

 <li> Consider a wireless LAN consisting of one access point and three stations: Stations A, B, and C. All the stations can hear each other. Each station has one and only one DATA frame to be sent to the access point. The access point does not have DATA frame to be sent. Distributed coordination function, which is based on CSMA-CA, is implemented. At time instant 0 microsecond, the channel becomes idle, and the three stations start to contend for the channel, with contention window being the initial contention window, i.e., [0, 31]. At time instant 0 microsecond, the three stations pick up random backoff timers as 10, 30, and 30, respectively.</li>

</ol>

Assume DIFS=50 microseconds; SIFS=10 microseconds; a backoff time slot=20 microseconds; RTS transmission time=CTS transmission time=ACK transmission time=100 microseconds; A DATA frame transmission time = 2000 microseconds. If a station sends an RTS frame, it will wait for a TIMEOUT duration (which is equal to the duration of CTS plus SIFS) to get the corresponding CTS. If a station hears a collision (i.e., senses a busy channel but cannot decode information), after the channel becomes idle again, the station will also wait for a TIMEOUT duration. Assume the propagation delay is negligible. We also have the following assumption: if Station A needs to pick up a new backoff timer from its contention window denoted [X<sub>1</sub>, Y<sub>1</sub>], it will pick up Y<sub>1</sub>-5; if Station B needs to pick up a new backoff timer from its contention window denoted [X<sub>2</sub>, Y<sub>2</sub>], it will pick up Y<sub>2</sub>-10; if Station C needs to pick up a new backoff timer from its contention window denoted [X<sub>3</sub>, Y<sub>3</sub>], it will pick up Y<sub>3</sub>-15.

In the system, we have transmission events. A transmission event is a <em>successful transmission</em> if only one station transmits, or a <em>collision</em> if two or more stations transmit. <strong>How many transmission events are there in the system? What is the duration for each event?</strong> Here the duration of a successful transmission is the duration from the beginning of DIFS until the end of ACK, and the duration of a collision is the duration from the beginning of DIFS until the end of

TIMEOUT.