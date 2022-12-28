#networking 

- Stack of protocols used by the internet
- Four abstraction layers
- Is **descriptive**: describes the scopes of protocols used by the internet (unlike [[zk/OSI Model]])
- Developed mid-1970s by Defence Advanced Research Projects Agency at the US Department of Defence
- Maintained by the [[zk/IETF]]

| Layer | Data | Description |
| -     | -    | -           |
| Application | Data | Information created by an application, including session data |
| Transport | [[zk/TCP]]/[[zk/UDP]] | TCP/UDP [[zk/Segments]] |
| Internet | [[zk/IP]] | IP [[zk/Packet]] between interconnected independent networks |
| Link | Frame | TCP/IP sets no standards for media-level frames and assumes a working network |