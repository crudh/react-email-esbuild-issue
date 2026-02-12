# react-email-esbuild-issue

This is a simple react email starter with the single addition of `esbuild@0.27.3` in the dev dependencies. That addition breaks the preview server:

<img width="1013" height="239" alt="Screenshot 2026-02-12 at 09 54 05" src="https://github.com/user-attachments/assets/8b9f61b6-03bd-4d15-bb6d-820375942f06" />
<img width="681" height="53" alt="Screenshot 2026-02-12 at 09 54 13" src="https://github.com/user-attachments/assets/70000f91-0765-49a6-af7f-52a4592a07c7" />

Removing the `esbuild` dev dependency fixes it.

This also happens in a pnpm monorepo when another application has the `eslint` dev dependency that mismatches with the one from the preview server (0.25.10).
