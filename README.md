# Open Community Matrix Issues

## Why are we documenting issues?

The aim of this repository is to track issues that are important to
open communities using Matrix. And from there organise the effort to
fix them.

## What is an open community?

A community that participates in the open Matrix federation with no
secure border gateways.

## Triaging

Triaging is done by assigning 4 labels.

- An actor label to determine _who_ the issue is related to or their role.

- The likelihood that the actor of this type is to experience the issue.

- The impact that the issue has on the actor's experience.

- The priority of the issue in regards to how it makes the actor feel
  about Matrix.

Each of these labels has a weight which is used to calculate a pain
score as a percentage late.

`Pain = Likelihood * Impact * Priority / Max Likelihood * Max Impact * Max Priority`

With this percentage, we can visibility into which issues are the most
painful for Matrix users by sorting issues descending by the pain
score.

This triage process is derived primarily from Avery Pennarun's [epic
treatise on scheduling, bug tracking, and
triage](https://apenwarr.ca/log/20171213). But has been modified
significantly, see [Draupnir's
documentation](https://the-draupnir-project.github.io/draupnir-documentation/contributing/triaging)
and [Gnuxie's blog post on
triage](https://marewolf.me/posts/draupnir/2401.html#triaging) for the
details.

### Actor

#### Contributor

A contributor to Matrix

#### Room/Space moderator

A moderator for a room/space on Matrix

#### Homeserver moderator


A moderator managing resident users, joined rooms

#### System administration

Relates to the workflow of deploying services such as Synapse, Draupnir, or self hosting in general.

#### Community member

Issue relates to the experience of participating in a Matrix community.

### Likelihood

How likely an actor is to encounter the issue.  Scoped to the actor
category, so don't for instance worry that not all users are system
administrators. The liklihood would be whether all system
administrators experiance the issue.

So if there is no documentation for how to setup a homeserver
anywhere, and the actor of the issue is a system administrator. Then
the label for all users would apply.

#### 1. Very Few actors

#### 2. Some actors

#### 3. Most actors

#### 4. All actors

### Impact

#### 1. New Feature

Unrelated to any existing feature (must be used liberally)

#### 2. Rendering or Aesthetic Issue

Visual and Sound Polish: Aesthetic issues

#### 3. Workflow issue

User employs strategies to achieve the task that harm the experience
(use minor first).

#### 4. Minor issue

Impairs usability in secondary scenarios.

#### 5. Major issue

Impairs usability in key scenarios.

#### 6. Critical Issue

The issue causes clients to crash, causes data loss, or represents a
vector for the propagation of abuse. E.g. Being sent images from
unfamiliar users.

### Priority

Follow the questions in the order shown here.

#### 3. Outrageous

Is it possible that an actor will consider leaving the platform
because of this issue (or never join)?

#### 2. Aggravating

Is this issue likely to prevent the actor from recommending Matrix?

#### 1. Nuisance

The issue is a nuisance but it is likely that the actor can still
happily recommend Matrix (in isolation of other problems).
