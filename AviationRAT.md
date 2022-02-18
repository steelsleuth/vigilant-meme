# TA2541: From Tweets to Tactics

Proofpoint has clustered together activity of various RATs targeting crucial industries since 2017. This threat actor, classified as TA2541, has several distinctive TTPs in their delivery methodology. Analysts sharing IoCs on Twitter have uncovered a string of AsyncRAT infections utilizing a new crypter called [“Snip3”](https://blog.morphisec.com/revealing-the-snip3-crypter-a-highly-evasive-rat-loader), which Proofpoint researchers have found TA2541 utilizing in their campaigns. We can retroactively go through these tags and identify any additional activity. 

Hunting through [Twitter for this tag](https://twitter.com/search?q=%23snip3&src=typed_query&f=live), we see various reports related to dcRAT and AsyncRAT. In one [tweet from June](https://twitter.com/BushidoToken/status/1402397157420945412?s=20&t=chKdb1iqnSg3Ap2PD7PWoQ
), BushidoToken noticed Snip3 VBS payloads targeting the Aviation sector. The C2’s for these payloads line up with TA2541 infrastructure observed by Proofpoint. 

The above VirusTotal link has multiple collections and graphs associated with it, giving some additional insight into the relations between infrastructure used. 

Reviewing the emails released by Proofpoint, there is a clear pattern behind their design. The use of PDF/XLS icon’s linking to a legitimate business file name is distinct when combined with the RFQ / business lures and detailed emails. 

While a breadth of RATs have been observed from this campaign by Proofpoint since 2017, AsyncRAT has been the dominant payload in 2021. In a common tactic seen by other email-based campaigns, TA2541 utilizes Google Drive URLs to download the VBS payloads. This is the first clear indicator to cut off their infection chain. 

Now that analysts know what to hunt for, organizations can also double down their security training programs for these new threats.

## [Return to Blog](https://steelsleuth.github.io/vigilant-meme/)
