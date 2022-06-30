The Dependency submission API lets you submit dependencies for a project. This enables you to add dependencies, such as those resolved when software is compiled or built, to {% data variables.product.prodname_dotcom %}'s dependency graph feature, providing a more complete picture of all of your project's dependencies.

The dependency graph shows any dependencies you submit using the API in addition to any dependencies that are identified from manifest or lock files in the repository (for example, a `package-lock.json` file in a JavaScript project). For more information about viewing the dependency graph, see "[Exploring the dependencies of a repository](/code-security/supply-chain-security/understanding-your-software-supply-chain/exploring-the-dependencies-of-a-repository#viewing-the-dependency-graph)."

Submitted dependencies will receive {% data variables.product.prodname_dependabot_alerts %} and {% data variables.product.prodname_dependabot_security_updates %} for any known vulnerabilities. 依存関係に対する{% data variables.product.prodname_dependabot_alerts %}が得られるのは、{% data variables.product.prodname_advisory_database %}の[サポートされているエコシステム](https://github.com/github/advisory-database#supported-ecosystems)のいずれかからのものである場合だけです。 Submitted dependencies will not be surfaced in dependency review or your organization's dependency insights.