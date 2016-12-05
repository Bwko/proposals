# Gitea: Proposals

The Gitea project's development process is design-driven. Significant changes to the projects, applications, or tools must be first discussed, and sometimes formally documented, before they can be implemented. This document describes the process for proposing, documenting, and implementing changes to the Gitea project.

## Proposal Process

### Goals

- Make sure that proposals get a proper, fair, timely, recorded evaluation with a clear answer.
- Make past proposals easy to find, to avoid duplicated effort.
- If a design doc is needed, make sure contributors know how to write a good one.

### Definitions

- A **proposal** is a suggestion filed as a GitHub issue in [Gitea](https://github.com/go-gitea/gitea) repository, identified by having the Proposal label.
- A **design doc** is the expanded form of a proposal, written when the proposal needs more careful explanation and consideration.

### Scope

The proposal process should be used for any notable change or addition to the project, applications and tools. Since proposals begin (and will often end) with the filing of an issue, even small changes can go through the proposal process if appropriate. Deciding what is appropriate is matter of judgment we will refine through experience. If in doubt, file a proposal.

### Compatibility

Gitea 1.x lower version must continue to work after upgrade to 1.x higher version. Any proposed change must not break this promise.

### Process

- [Create an issue](https://github.com/go-gitea/gitea/issues/new) describing the proposal.

- Like any GitHub issue, a Proposal issue is followed by an initial discussion about the suggestion. For Proposal issues:
  - The goal of the initial discussion is to reach agreement on the next step: (1) accept, (2) decline, or (3) ask for a design doc.
  - The discussion is expected to be resolved in a timely manner.
  - If the author wants to write a design doc, then they can write one.
  - In Gitea development historically, a lack of agreement means the author should write a design doc.
  - If there is disagreement about whether there is agreement, [lunny](mailto:lunny@gitea.io) is the arbiter.

- It's always fine to label a suggestion issue with Proposal to opt in to this process.

- It's always fine not to label a suggestion issue with Proposal. If the suggestion needs a design doc or is declined but worth remembering, it is trivial to add the label later.

- If a Proposal issue leads to a design doc:
  - The design doc should be checked in to [the proposal repository](https://github.com/go-gitea/proposals) as `design/NNNN-shortname.md`, where `NNNN` is the GitHub issue number and `shortname` is a short name (a few dash-separated words at most). Clone this repository with `git clone https://github.com/go-gitea/proposals` and follow the github Pull Request document.
  - The design doc should follow [the template](design/TEMPLATE.md).
  - The design doc should address any specific issues asked for during the initial discussion.
  - It is expected that the design doc may go through multiple checked-in revisions.
  - New design doc authors may be paired with a design doc "shepherd" to help work on the doc.

- Once comments and revisions on the design doc wind down, there is a final discussion about the proposal.
  - The goal of the final discussion is to reach agreement on the next step: (1) accept or (2) decline.
  - The discussion is expected to be resolved in a timely manner.
  - If clear agreement cannot be reached, the arbiter ([lunny](mailto:lunny@gitea.io)) reviews the discussion and makes the decision to accept or decline.

- The author (and/or other contributors) do the work as described by the "Implementation" section of the proposal.

## Help

If you need help with this process, please contact the Gitea contributors by posting to the [gitea-develop mailing list](https://groups.google.com/d/forum/gitea-develop). Note that the list is moderated, and that first-time posters should expect a delay while their message is held for moderation. To learn about contributing to Gitea in general, see the [contribution guidelines](https://github.com/go-gitea/gitea/blob/master/CONTRIBUTING.md).

## Contributing

Fork -> Patch -> Push -> Pull Request

## Authors

* [Maintainers](https://github.com/orgs/go-gitea/people)
* [Contributors](https://github.com/go-gitea/proposals/graphs/contributors)

## License

This project is under the Apache-2.0 License. See the [LICENSE](LICENSE) file for the full license text.

## Copyright

```
Copyright (c) 2016 The Gitea Authors <https://gitea.io>
```
