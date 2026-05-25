# Key Information Regarding Midsem S1 2026


### Preamble
- The midsemester skills assessment is actually pretty easy;
- For me, it consisted of three routers, one switch and ungraded PCs
- The convenor did NOT post any practice exams for midsemester so I used AI to help create some, they're listed in this same directory.
- The assessment used the OSPF protocol with just a single area and three routable VLANs
- These exams are similar cadence and skill level to the actual midsemester however one thing twisted my mind:


### Shit that got me
- The management VLAN was NOT ID#1 for me, it was on another VLAN ID, therefore had to specify ìnterface vlan36`, set the IP on the switch and create another subinterface for VLAN36 on the closest router, ensuring VLAN1 interface (created by default on the switch) is DISABLED otherwise it results in a MAJOR ERROR. Because its a management VLAN, no switchport should be assigned this VLAN, and therefore the native VLAN (VLAN 1, created by default) just becomes a blackhole since there's no router subinterface for it

### More Rambling
- ACLs were really easy, needed two, and they were both of two rules, nothing too complex to boggle my mind however;
- My tutor said ACLs should cover a HOST not a whole SUBNET - turns out this is entirely wrong and I ended up getting a major error for this failing skills - I argued this since other people had the same issue due to the tutor's bad information, and this was downgraded to a minor issue. To prevent this *ACLs COVER THE ENTIRE SUBNET!* not just a host! This was my only issue, otherwise at great cadence (no hands off the keyboard) it took me about 20 minutes to complete in total with my decent typing speed. I personally do not use a lab journal as I believe its important to passively memorise most commands for efficiency reasons;


### For you
- I advise trying to memorise at least portions of commands you use regularly since it saves a massive amount of time
- I recommend you memorise/utilise/write-down debugging commands too as these will save your ass if something doesn't work. `show ip int brief` `show port-security` `show vlan brief` `show ip route` `show run`