# The Update Framework Governance

## Project Types

* Core: the core of The Update Framework (TUF) project is the TUF specification
  of a framework for securing software update system, and the TUF Augmentation
  Proposals (TAPs) process that is used to provide additional information about
  TUF or describe a new feature for TUF or for its processes or environment.
  Included with the core projects are ancillary projects such as the website
  (theupdateframework.io) and artwork repositories.
* Subprojects: are closely related, but semi-independent, projects such as
  implementations of the TUF specification (notary, go-tuf, tuf, etc).

## Contributor Ladder

* Participant: any person that contributes their time and thoughts to The
  Update Framework.
* Contributor: someone who contributes directly to the project, such as
  submitting Pull Requests, engaging in discussions on Issues or in Slack,
  attending meetings, etc.
* Subproject member: a recognised contributor who has been granted additional
  capabilities (including closing/reopening and assigning issues and pull
  requests)
* Subproject Maintainer: a maintainer can also review and merge pull requests.
* TAP Editor: maintainers of the specification and TAPs.
* Consensus Builder: the project's founder and consensus builder, is able to
  veto any issues put to the Steering Committee vote.

Contributors who have not actively contributed to the project, through PRs and
Issues, or communicated on project forums (GitHub, Slack, Mailing list) for
longer than 12 months may be involuntarily moved down the contributor ladder,
or asked to move to an emeritus status.

## Individual Subproject Governance

All active Maintainers of each subproject, as defined in the Contributor
Ladder, are members of that subproject's Maintainer Committee, which governs
that subproject. The subproject's Maintainer Committee is responsible for the
following subproject governance activities:

* Ensuring that the subproject creates and publishes regular releases;
* Holding regular, subproject-wide discussions on issues and planning;
* Periodic review of subproject contributors for advancement on the Contributor
  Ladder;
* Making final decisions on subproject changes that involve controversial
  trade-offs;
* Responding to security compromise reports;
* Supporting the Code of Conduct within their subproject and referring
  violations to the Code  of Conduct Committee.

Additionally, the subproject's Maintainer Committee will select one
representative to the Steering Committee.

## Steering Committee
The overall TUF umbrella project is governed by a Steering Committee, which is
selected as follows:
* One Maintainer representative from each member subproject
* All of the TAP Editors
* The Consensus Builder

## Steering Committee Duties

The Steering Committee is responsible for the following tasks, any of which may
be delegated to a person or group selected by the committee:

* Reviewing and deciding on new subprojects to add to The Update Framework
* Arbitrating inter-subproject disagreements
* Selecting the Code of Conduct Committee and ratifying CoC judgements
* Removing subprojects which have become inactive
* Acting on escalated security or code quality issues
* Resolving issues that individual subprojects are unable to resolve
* Administering project infrastructure, intellectual property, and resources
* Determining overall direction for advocacy and marketing
* Issuing statements on behalf of The Update Framework and its subprojects
* Reviewing and approving Contributor Ladder advancement for participants who
  work on the overall umbrella project

In performance of these duties, the Steering Committee will hold a quarterly
meeting that is open to all contributors. The Committee may hold additional,
closed meetings in order to discuss non-public issues such as security exploits,
CoC enforcement, and legal questions.

Steering Committee members are expected to advocate for all of The Update
Framework, not just certain subprojects or corporate sponsors, comply with and
support the Code of Conduct, and be professional and compassionate in all of
their dealings with project participants.

## Code of Conduct Committee

In order to review and enforce the Code of Conduct, the Steering Committee
selects 3 people to be on the Code of Conduct Committee.

These individuals will be chosen based on their community management and code of
conduct experience, with diverse representation across the committee, including
employer, gender, race, background, and region of the world. To avoid fatigue,
the Steering Committee will replace at least 1 member of the CoC Committee each
year. Members of the committee do not need to be members of The Update Framework
if they have sufficient other expertise.

The CoC Committee will receive reports of conduct violations confidentially, and
will discuss them in closed meetings. If a report is determined to be a
violation, they will recommend action on it appropriate to the scale, nature,
and context of the violation, from requiring an apology, up to expulsion of an
individual from the project. In the event that a contributor is to be demoted or
expelled, the CoC Committee will forward this recommendation to the Steering
Committee who will ratify it in a closed meeting. Should a member of the
Steering Committee be the offender or the reporter, this recommendation will
instead be forwarded to the CNCF staff for final arbitration.

## Adding Subprojects

During the quarterly Steering meeting, any project Member may recommend
subprojects to become part of The Update Framework. These subprojects should
have the following characteristics:

* Have a mission of securing software update systems;
* Are appropriately licensed and governed or willing to become so;
* Are under active development;
* Consist of high quality code and designs.

Before submitting an application to the Steering Committee, the applying
subproject must hold an internal consensus vote of all major subproject
contributors to join The Update Framework. The Steering Committee will then
review the application, and decide whether or not to accept it. If it is
accepted, the Committee will assign one person to assist the subproject in their
integration.

In some cases, promising but incomplete subprojects may be accepted as
Experimental Subprojects. Such Experimental Subprojects will be considered part
of The Update Framework, but will be marked as Experimental on the website and
in code repositories, in order to inform users. Experimental subproject Members
are considered Members of The Update Framework, but the subproject is not
entitled to a representative on the Steering Committee. Steering will review
Experimental Subprojects at least twice per year to determine if they have
matured to full subproject status.

## Removing Subprojects

In some cases, subprojects will become inactive or unmaintainable, or wish to
separate from The Update Framework. Any Steering Committee member may propose
removal of a subproject on these grounds, and Steering can confirm this with a
majority vote.

Subprojects which still have contributors will then be moved to a repository in
their own namespace. Subprojects which have ceased all activity are moved to a
theupdateframework-archive namespace. Note that any subproject assets, such as
trademarks, may be legally required to remain in the possession of the Linux
Foundation in some form.