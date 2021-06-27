# Finding Personally Identifiable Information Leaked viaPublicly Accessible CT Logs
This repository is part of the proof-of-concept research conducted by F.G. van Mourik at the University of Twente on July 2nd, 2021.

## Research Abstract
Certificate Transparency (CT) is a network security standard that includes all public-key certificates in publicly accessible logs. Major browser vendors such as Chrome require certificates to be present in CT logs before accepting them. These logs can be analysed and audited by everyone in the world, adding an extra layer of security on top of the Internet. These certificates, however, might include personally identifiable information (PII) from website creators or administrators, for instance their first and last name. Since CT logs are queryable at a large scale, possibly contain PII, and are non-optional, a privacy issue arises.

This research provides a proof-of-concept approach to find PII in these public logs by looking at the registered domain names within over one billion certificates and characteristics of these domain names in combination with commonly-used Dutch first and last names. Additionally, in this work we aim to find providers of PII in certificate's domain names, focused on the ".nl" DNS zone. Here we found several companies that potentially forward PII of their customers in CT. Finally, this research looks into the amount of PII in domain names over time in order to spot possible increasing and decreasing trends. No significant trends were observed.

## Files
This repository contains the following parts:

- The final paper of the research
- The documented codebase of the research
- The acquired Dutch names dataset needed for the research.
- An MIT license

## Sources of the acquired dataset:

First names: https://www.meertens.knaw.nl/nvb/

Last names: https://www.meertens.knaw.nl/nfb/documenten/top100.pdf

## License
See the added license file to know what can and can't be done with this repository.