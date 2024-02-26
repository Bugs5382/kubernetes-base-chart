# Kubernetes Base Chart
> This is a helm chart the setups my preferred applications on empty kubernetes image.

## Table of Contents

1. [Summary](#summary)
2. [Keyword Definitions](#Keyword-Definitions)
3. [Basic Install](#install)
4. [License](#license)

## Summary

When I am setting up Kubernetes cluster, I always want the base installation to be done correctly.
I use Helm, as the primary way I setup my kubernetes applications,
etc. So I created this chart that helps me setup an emtpty kubernetes cluster with my default apps that I like to use.

You might like to use them too, so here they are for your use as well. I made this really simple to use.

The default charts I use for the base of my applications is:

* Traefik - Proxy
* Cert\ Manager — Certificate Manager
* ArgoCD - GitOps
* MetalLB - Load Balancer
* Longhorn - Storage CSI

By no means does this do the full setup of each of the applications,
but gets you to a point where you should be comfortable.

Additionally, I use Cloudflare and Let's Encrypt (as Cert Manager's issuer) as part of the Cert Manager.

All the options can help you customize your base instance really quickly and uniformly.

### Notice

This has been tested only on on bare metal k0s instance(s). In theory, excluding MetalLB and Longhorn, this should work on Cloud based Kubernetes environment without issue.

## Keyword Definitions

This NPM is designed to support medical applications with potential impact on patient care and diagnoses, this package documentation, and it's peer package [node-hl7-server]() follow these definitions when it comes to the documentation.

Keywords such as "MUST", "MUST NOT", "REQUIRED",
"SHALL", "SHALL NOT", "SHOULD", "SHOULD NOT", "RECOMMENDED", "MAY", and "OPTIONAL".
These are standardized terms for technology documentation interoperability.
These words should have these meaning when you are reading them.
They might be sans uppercase throughout the documentation, but they would have the same meaning regardless.

* **MUST** - This word, or the terms "**REQUIRED**" or "**SHALL**", mean that the definition is an absolute requirement of the specification.
* **MUST NOT** - This phrase, or the phrase "**SHALL NOT**", mean that the definition is an absolute prohibition of the specification.
* **SHOULD** - This word, or the adjective "**RECOMMENDED**", mean that there may exist valid reasons in particular circumstances to ignore a particular item, but the full implications must be understood and carefully weighed before choosing a different course.
* **SHOULD NOT** - This phrase, or the phrase "**NOT RECOMMENDED**", mean that there may exist valid reasons in particular circumstances when the particular behavior is acceptable or even useful. The full implications should be understood and the case carefully weighed before implementing any behavior described with this label.
* **MAY** - This word, or the adjective "**OPTIONAL**", mean that an item is truly optional.  Any implementation which does not include a particular option MUST be prepared to interoperate with another implementation which does include the option, though perhaps with reduced functionality. In the same vein, an implementation which does include a particular option MUST be prepared to interoperate with another implementation, which does not include the option (except, of course, for the feature the option provides.)

## Install

More to come...

## License

Licensed under [MIT](./LICENSE).