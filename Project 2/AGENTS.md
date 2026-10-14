<!-- LOVABLE:BEGIN -->
> [!IMPORTANT]
> This project is connected to [Lovable](https://lovable.dev). Avoid rewriting
> published git history — force pushing, or rebasing/amending/squashing commits
> that are already pushed — as it rewrites history on Lovable's side and the
> user will likely lose their project history.
>
> Commits you push to the connected branch sync back to Lovable and show up in
> the editor, so keep the branch in a working state.
<!-- LOVABLE:END -->

## Portfolio architecture
- Use TanStack file routes with a shared bilingual layout and a single rule-based assistant; this preserves conversation and inquiry state across navigation without unnecessary authentication or database storage.
- Keep bilingual content and project evidence in structured data separate from reusable presentation components; this supports consistent Arabic/English views and accurate project details.
- Store only the language preference in browser storage; inquiry data remains in the shared assistant’s session state to avoid persisting visitor personal information.
- Validate inquiry data with a shared Zod schema and a fixed-recipient server endpoint; sending stays explicitly unavailable until an owned sender domain and the managed email helper are configured.
- Never use AI chat transport or model calls for the rule-based portfolio assistant; deterministic service choices and form review are the required interaction model.
