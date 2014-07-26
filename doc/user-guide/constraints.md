- The only way for data to get into or out of Onyx is via HornetQ. Plugins, however, can provided the illusion that this isn't true.
- Only maps may enter Onyx and be emitted internally as segments. The only exception to this rule is the sentinel value.
- Unlike Hadoop and Storm, the Onyx application jar is not transfered to the nodes on the cluster via a command line utility. Configuration management, such as Chef and Puppet, have come far enough to allow for an improved deployment story.