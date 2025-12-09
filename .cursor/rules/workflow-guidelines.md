# Workflow Guidelines

1. **Always check `/truth/TC.vX.md` before making assumptions** - This is the authoritative source for all project decisions.

2. **When requirements are ambiguous, document in `/requirements/SRS.ambiguities.md`** - Do not invent requirements; log ambiguities for resolution.

3. **Maintain traceability using `origin:` and `derived-from:` tags** - Every artifact should reference its source.

4. **Follow the command sequence:** TC → SRS → BR → Flows → ERD → API → Components
   - This ensures proper traceability and alignment with authoritative sources.

