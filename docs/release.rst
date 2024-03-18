Release-decision
================

Every week an automatic job will be executed to determine if there is a
potential need for a new release:

* If the number of commits since last release has reached a threshold; AND There is no open “release-decision” discussion:
  * Creates a new "release-decision" discussion to run a poll between all the MAINTAINERS,
    so they will have the opportunity to thumbs up if there is a need for a new release;
  * MAINTAINERS will be mentioned in the discussion, therefore everybody should be notified
    about ongoing votes.;
  * If every MAINTAINER thumbs-up in discussion, the automatic job will be triggered to do the release.
  * The discussion should be closed
* If there is any existing open discussion, the bot job should comment on the
  same discussion with the updated list of commits and ping again the
  MAINTAINERS whose have not voted yet, give them the opportunity to thumbs up based on the new
  status;
