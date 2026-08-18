# API Teams

An API Team is a machine-readable description of the people involved with producing and operating an API—each entry capturing who a team member is, the role they play, and how to reach them. APIs are ultimately produced and consumed by people, and making the team behind an API explicit brings more collaboration, communication, and accountability to the API lifecycle. The teams building block gives producers a common way to attach human context to their APIs so that consumers and stakeholders know who is behind the work.

## API Commons

API Teams are an [API Commons](http://apicommons.org) building block—an open, machine-readable schema for describing the humans who deliver an API, made interoperable as part of the API contract. It is indexed as a `Common` type within its [APIs.json](apis.yml) index, letting it be discovered, referenced, and reused across the APIs.json ecosystem and surfaced through [apis.io](https://apis.io).

## What's in this repo

- [teams-schema.yml](teams-schema.yml) — The JSON Schema that defines a team member.
- [teams-example.yml](teams-example.yml) — A worked example describing a single team member.
- [apis.yml](apis.yml) — The APIs.json index for this building block, referencing the schema and example as `Common` artifacts.

## The Schema

The [teams-schema.yml](teams-schema.yml) defines each team member as an object with the following properties:

- **identifier** — A unique identifier for the team member, allowing them to be easily referenced.
- **name** — A full name for the team member, defining the person who is part of the team.
- **role** — The role the team member plays in the wider organization, and at the team level.
- **gitHub** — The full URL to the GitHub user for a team member.
- **linkedIn** — The full URL to the LinkedIn user for a team member.
- **email** — The email address for a team member, allowing for easy communication.
- **description** — A description of the team member and their contribution as part of the team.

## Example

The [teams-example.yml](teams-example.yml) file describes a single team member:

```yaml
identifier: kin-lane
name: Kin Lane
role: API Evangelist
gitHub: https://github.com/kinlane
linkedIn: https://www.linkedin.com/in/kinlane/
email: kin@apievangelist.com
description: Kin Lane is the API Evangelist helping define all of the common building blocks of API operations.
```

## How It Fits

Teams is one of a growing set of API Commons building blocks that describe the business and technical realities of API operations in a machine-readable way. It cross-links with the [change log](https://github.com/api-commons/change-log), [road map](https://github.com/api-commons/road-map), [use cases](https://github.com/api-commons/use-cases), [plans](https://github.com/api-commons/plans), [guidance](https://github.com/api-commons/guidance), [policies](https://github.com/api-commons/policies), and other building blocks—each a small, reusable schema that can stand alone or be composed together within an APIs.json index.

## Support

This work is in an early stage of development and is rapidly moving as it is applied across a variety of user interfaces and approaches to API operations and governance. If you would like to contribute, have any questions, or would like to inform the work happening, please submit a GitHub issue on this repository or email kin@apievangelist.com.

## Part of API Commons

A machine-readable building block from **[API Commons](https://apicommons.org)** — open specifications and schemas for the APIs you produce and consume. See all building blocks and tools at **[apicommons.org](https://apicommons.org)** and the tools at **[apicommons.org/tools](https://apicommons.org/tools/)**.

**Related building blocks**
- [use-cases](https://github.com/api-commons/use-cases) — how an API is actually put to work, tied to its operations
- [road-map](https://github.com/api-commons/road-map) — publish an API's roadmap in a machine-readable way
- [plans](https://github.com/api-commons/plans) — machine-readable access plans, tiers, and pricing
- [guidance](https://github.com/api-commons/guidance) — the how-to layer that turns governance rules into help
- [policies](https://github.com/api-commons/policies) — the business rules behind API governance

## License

The artifacts in this repository — the schemas, examples, and API descriptions — are
licensed **[CC BY-NC-SA 4.0](LICENSE)** (Attribution–NonCommercial–ShareAlike).

API Commons licenses **artifacts** under CC BY-NC-SA 4.0 and **code** under Apache-2.0.
