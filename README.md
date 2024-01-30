# ansible-facts
Facts management exercises

I created a playbook.yml which grabs EVERYTHING. I dumped it out to a file
using:

ansible-navigator run -m stdout playbook.yml > facts.txt

To view it, use /usr/bin/more instead of /usr/bin/less so that the special 
characters print correctly. 

Then I looked through facts.txt. Notice that there are facts about everything
from BIOS vendor to IP address and so on.

Next, I created a playbook which only showed a few facts, specifically the
FQDN and the IP address.
