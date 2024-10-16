+++
title = "funding.json - an open manifest for describing financial requirements for FOSS projects"
slug = "funding-manifest"
+++

# funding.json

`funding.json` is an open manifest (JSON schema) that acts as a signaling and discovery mechanism for projects seeking funding. It is a self-contained manifest file that FOSS (Free and Open Source Software) projects, developers, and communities can host on their websites or repositories to describe their financial requirements in a structured, machine-readable manner. It acts like a robots.txt file or a progressive web app manifest, allowing it to be publicly crawled and indexed, to make projects in need of financial assistance discoverable.

See this [example listing](https://dir.floss.fund/view/@example.com) for a demonstration of how a manifest could be parsed and presented.


## Schema

Current version is v1.0.0

```json
{{ read_file(path="static/static/funding.schema.json") }}
```
<a href="#" data-copy-clipboard>Copy</a>

-----------

## Example

Assuming that the manifest is located at `https://example.com/funding.json`
```json
{{ read_file(path="static/static/funding.example.json") }}
```
<a href="#" data-copy-clipboard>Copy</a>

<br />

For repository hosting platforms like GitHub, the manifest can be checked into the project repository directly, eg: `https://github.com/example/coolapp/blob/main/funding.json`

-----------

### wellKnown

If the manifest references URLs, such as a project's webpage, that are not on the same domain as the `funding.json` manifest itself, then the `wellKnown` URL must point to a `/.well-known/funding-manifest-urls` file. This file should contain URL (one or more) of the `funding.json` manifest URLs that reference it. This establishes provenance and verifies that that the publisher of the manifest is authorised to solicit funding on behalf of the URLs (entity, projects) described in the manifest. This follows the [.well-known](https://en.wikipedia.org/wiki/Well-known_URI) convention. An example scenario is described below.

|                                                 |                                                              |
| ------------------------------------------------|--------------------------------------------------------------|
| Manifest location                               | https://example.com/funding.json                             |
| Project URL referenced in the manifest          | https://my-cool-project.net                                  |
| Expected `wellKnown` along with the project URL | https://my-cool-project.net/.well-known/funding-manifest-urls |
| Contents of the `wellKnown` file                | `https://example.com/funding.json`                           |

### tags

While the `tags[]` field under projects is meant for arbitrary lowercase-alphanumeric-dash strings to describe the projects, [project-tags.txt](/static/project-tags.txt) can be used as a reference list for uniformity.

-----------

## Tools

- [Live manifest validator](https://dir.floss.fund/validate)
- [Manifest builder UI](https://vishnukvmd.github.io/funding.json/)
