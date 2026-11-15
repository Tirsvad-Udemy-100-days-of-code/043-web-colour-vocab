# MIL-001: Baseline and framework alignment

## Metadata
| Key | Value |
| --- | --- |
| ID | MIL-001 |
| CrossReference | [BC-001] |
| Language | en |
| Domain | education |

## Version History
| Date | Status | Author | Reviewer | Change | Commit |
| --- | --- | --- | --- | --- | --- |
| 2026-11-16 | Accepted | Jens Tirsvad Nielsen | AI as stand-in for S02 | Initial version; accepted with the Go verdict of the review record (autonomous, not independent) | pending |

---

## Purpose

This gate decides whether Web Colour Vocab has a complete, reviewed baseline: documents, wiki, README and metadata, merged to the default branch with a green build.

## Deliverable

A merged pull request that holds: the accepted Business Case, Stakeholder Analysis, Project Plan and this milestone with their review records; the traceability matrix; the wiki in English, Danish and Malay; the README in the framework template; the manual test checklist; and the framework release adopted by the project.

## Go / No-Go Criteria

| # | Criterion (objectively checkable) | Go | No-Go |
| --- | --- | --- | --- |
| 1 | BC-001, SA-001, PP-001 and MIL-001 each have an `Accepted` Version History row and a review record with the verdict `Go` | All four | Any missing or `Go-with-conditions` |
| 2 | Every item of `tests/manual-checklist.md` passes when `src/index.html` is opened in a browser, and `git diff origin/main -- src` on the pull request branch is empty | 8 of 8 `Pass`, empty diff | Any `Fail` or any change in `src/` |
| 3 | `docs/wiki/` has `_Sidebar.md` and the pages Home, Getting-Started and Project-Documents in en, da and ms | 9 pages and the sidebar | A page or language missing |
| 4 | `framework/scripts/check-readme.sh` and `framework/scripts/check-languages.sh` run | Exit code 0 | Any finding |
| 5 | The README License section names AGPL-3.0 and links `LICENSE`, and `LICENSE` exists | Both | Either missing |
| 6 | All CI (continuous integration) checks of the pull request | Green | Red or pending |

## Dependencies

| Depends on | Reason |
| --- | --- |
| none | This is the first and only gateway of the baseline |

## Traceability

| Business Case objective / KPI / user story | Reference |
| --- | --- |
| O1 | Criteria 2 and 6 |
| O2 | Criteria 1 and 4 |
| O3 | Criterion 3 |
| O4 | Criterion 5 |

## Ownership

| Role | Stakeholder ID (SA) |
| --- | --- |
| Owner | S01 |
| Approving reviewer | S02 |

## Target Date

2026-11-23: one week after the start, as the Business Case constraint requires.

## Tasks

| # | Task | Summary | Needs its own Use Case/User Story? | Reference |
| --- | --- | --- | --- | --- |
| 1 | Adopt the framework release | Track the `framework/` submodule and `.gitmodules`, install the skills and hooks, and track `.env.example` so the project follows the same rules as the other projects of the portfolio. | No | |
| 2 | Write and review the baseline documents | Create the Business Case, Stakeholder Analysis, Project Plan, this milestone and the traceability matrix, review each against its QC checklist and accept them on a `Go`, so the plan-first gate is met. | No | |
| 3 | Publish the wiki in English, Danish and Malay | Write the pages Home, Getting-Started and Project-Documents and the sidebar in `docs/wiki/`, so a visitor can learn what the exercise is and how to run it in their own language. | No | |
| 4 | Restore the README to the framework template | Bring back the original text of the README inside the template's sections and the document appendix, with the project links, so the README is complete and checkable. | No | |
| 5 | Add and run the manual test checklist | Write `tests/manual-checklist.md` for the page and run it in a browser, so the check of the page is repeatable and objectively checkable. | No | |

---

[BC-001]: ../business-case.md
