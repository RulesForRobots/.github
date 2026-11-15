# Security

Rules for Robots includes guards: hooks that refuse what an agent must never do, such as destructive commands or writes to protected files. A way around a guard is a security problem, as is anything that lets a plugin, a workflow, or a hook run what its user did not intend.

## Reporting

Report privately, through **Security, Report a vulnerability** on the repository concerned (GitHub's private vulnerability reporting). Do not open a public issue or pull request for it.

Include what you did, what happened, the plugin and its version, and the smallest example that shows it. You will hear back within a week.

## Supported versions

The latest release of each plugin. A fix ships as a new release of that plugin; older releases are not patched.

## Known limits

A pattern guard always has another route around it. The guards are one layer; what can be damaged is also limited by the environment an agent runs in (its permissions, its network, its credentials), and each guard's documentation lists what it cannot see.
