# vf-apps: traversing-the-flows

This is not so much an app in itself as an algorithm which could be implemented as one or more modules to be used by different apps.

This is being harvested from https://github.com/valueflows/django-vocabulator/, although it is also used in all the versions of NRP (for example in [planning](https://speakerdeck.com/mikorizal/6-nrp-planning-concepts-and-tutorial) and [value equations](https://speakerdeck.com/mikorizal/10-nrp-value-equation-concepts-and-tutorial)), because the logic was cleaned up a lot for the vocabulator.

This [vocabulator issue](https://github.com/valueflows/django-vocabulator/issues/7) describes the cleanup and links to examples of the code.

Flow traversals would be used in several apps, for example, Provenance

![provenance](https://user-images.githubusercontent.com/117439/50448937-b1820080-08e9-11e9-9e81-e53897715353.png)

Each Resource (Apples, #3 Apples, Cider, Hard Cider) has links to its previous Events and Transformations (VF calls them Processes), so by following the arrows (links) backwards, the source of the apples in the cider can be found. Were this a food contamination problem, then the links from the Orchard to the Retailer and Baker would be followed for recalls. (The diagram leaves out a lot of details about exactly how everything happens, but they are or will be in the VF specs.)

The resource flow graph could be as long as necessary.  And could include equipment/tool usage and work.

See also https://valueflo.ws/appendix/track.html

*This README is a placeholder. The actual spec will evolve in issues, and then summarized here.*
