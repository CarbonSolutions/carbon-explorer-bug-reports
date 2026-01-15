---
name: Bug report
about: Report a bug in Carbon Explorer
title: ''
labels: ''
assignees: ''

---

**What happened?**
<!-- Describe what happened when you encountered the bug -->

**What did you expect to happen?**
<!-- Describe what you expected to happen instead -->

---

## Steps to Reproduce

1.
2.
3.

---

## Impact

Please select the option that best describes the severity of this issue:

- [ ] Blocks usage completely
- [ ] Major feature broken
- [ ] Minor visual or UX issue
- [ ] Performance issue
- [ ] Other

---

## Environment Information

- **Browser:** ${env.browser}
- **Operating System:** ${env.os}
- **Screen Resolution:** ${env.screenResolution}
- **Viewport Size:** ${env.viewportSize}
- **URL:** ${env.url}
- **App Version:** ${env.appVersion || 'Unknown'}
- **Build ID / Commit:** ${env.buildId || 'Unknown'}
- **Timestamp:** ${env.timestamp}

<details>
<summary>User Agent (click to expand)</summary>

\`\`\`
${env.userAgent}
\`\`\`

</details>

${
  errorContext
    ? `
---

## Error Context

- **Error Message:** ${errorContext.message}

<details>
<summary>Stack Trace</summary>

\`\`\`
${errorContext.stack}
\`\`\`

</details>
`
    : ''
}

---

## Screenshots / Console Errors

<!-- Paste any screenshots, console errors, or network errors below -->

`;
