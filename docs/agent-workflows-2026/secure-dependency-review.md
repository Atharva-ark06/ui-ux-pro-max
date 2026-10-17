# Secure Dependency Review Workflow

Before adding or upgrading a dependency, confirm it solves a real need and fits the project's maintenance and security requirements.

## Review steps

1. Check whether existing platform APIs or dependencies already solve the problem.
2. Confirm package identity and official source.
3. Review license, maintenance activity, release history, and known advisories.
4. Inspect transitive dependencies and install scripts when relevant.
5. Check supported runtime versions and bundle impact.
6. Pin or constrain versions according to repository policy.
7. Run tests and inspect lockfile changes.
8. Document why the dependency is needed.

## Red flags

- Similar package names that may be typosquats.
- Obfuscated install scripts or unexplained network calls.
- Unmaintained packages in security-sensitive paths.
- Unexpected changes to lockfiles or package sources.
- Requests for credentials unrelated to the package's purpose.

## After installation

Run the project's tests and dependency/security checks. Keep the dependency only if the value outweighs its maintenance and attack-surface cost.
