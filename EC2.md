## EC2
EC2 provide us the capability to work with work loads. You can think of it as hardware machine. <br>

<br>
It is of four types. <br>
  * On Demand - Fixed rate by hour <br>
  * Reserved - Capacity Reservation <br>
  * Spot - Bidding based <br>
  * Dedicated hosts - physical server <br>

<br>
** EC2 Instance Meta data ** <br>
Used to get info about an EC2 instance. <br>
It is available on http, can provide details like ipv4 address, security groups etc. <br>
curl http://ip/latest/meta-data/local-<metrics you want> <br>
